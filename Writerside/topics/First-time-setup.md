# First time setup
<primary-label ref="tutorial"/>
<secondary-label ref="wip"/>
<secondary-label ref="totsudo"/>
<secondary-label ref="admin"/>
<include from="library.md" element-id="wip"/>

This article will walk you through the first-time setup of Tot!Sudo. We won't be using any other mods for now, as we'll start at the core and slowly expand outward as we get familiar with things.

You'll learn the following:
- How to set up Tot!Sudo on a fresh server.
- What Super Admin is.
- What Roles & Permissions are.

## Before you start

Make sure that you:
- Have installed [Tot!Sudo from the Steam Workshop](https://steamcommunity.com/sharedfiles/filedetails/?id=3036057084) and enabled it in your modlist as your only mod.
- Are on a fresh dedicated server without an existing Tot!Sudo configuration.

<include from="library.md" element-id="warning-singleplayer"/>

## Accessing the Tot!Sudo Admin Panel

The Admin panel is your go-to dashboard for all admin configuration for Tot!Sudo and any mods that use its framework. 

1. Enable vanilla Admin mode through the standard <shortcut key="$conan"/> menu. You will only need this for initial setup.

2. Press <shortcut key="$admin"/> to open the Tot!Sudo Admin Panel.

> **Keybinds**
>
> <shortcut key="$admin"/> inconvenient for you? You can also open it via the <shortcut key="$conan"/> menu, or change the default keybind via the Sudo Client Panel (<shortcut key="$client"/>).
>
{style="tip"}

## Setting your Super Admin Password

If all's well, you'll be met with the following screen. This is where you'll configure your Super Admin Password.
The screen will also explain how we can allow access based on Steam ID, but we'll skip that in this tutorial. 
You are free to configure this on your end, however.

![Sudo admin password screen](sudo-setup-1.png){ thumbnail="true" width="500"}

<chapter title="What is Super Admin?" id="what_is_super_admin" collapsible="true">
In Tot!Sudo, access to features is granular and handled on an individual level (more on this below). 
Enabling Super Admin grants someone FULL ACCESS, regardless of their roles and permissions.
Sounds convenient? Don't fall for it! Super Admin should only be used to perform actions you wouldn't otherwise be able to.
For everything else, it's best to configure your roles according to your needs.
</chapter>

<procedure title="Setting a password">
<step>Think of a <a href="https://imgs.xkcd.com/comics/password_strength.png">secure and unique passphrase.</a></step>
<step>Store your password somewhere safe.</step>
<step>Enter your password twice.</step>
<step>Hit Set Password.</step>
<video src="sudo-setup-2.mp4" preview-src="sudo-setup-2.png" width="500"/>
</procedure>

> **Keep your password safe!**
> 
> Your Super Admin Password is used to unlock a full-access toggle, so make sure to use a secure, unique password and not to share it with anyone. Always store it in a safe location in case you forget it.
>
{style="note"}

> **Lost your password?**
>
> [You can reset your password by editing your database.](https://apiconan.totchinuko.fr/#/tips?id=reset-super-admin-password) Make sure to use the correct .db file if you play with custom maps.
>
{style="tip"}

## Configuring the Everyone role

Next, we'll be asked to configure the 'Everyone' role with some Permissions. The 'Everyone' role is a default one that's automatically added to every player. In short, it applies to... everyone!

If you're following along and only have Tot!Sudo installed, we could just save permissions and continue: 
these permissions are largely intended for administration, and we don't really want everyone to have access to this stuff! But, for the sake of practice, let's add a harmless one.

We'll start configuring our roles when we add a mod that has features more suited for players and administration both.

<chapter title="What are roles and permissions?" id="what_are_roles_and_permissions" collapsible="true">

- A permission determines whether you have access to a certain feature in compatible mods.
- A role is effectively a group of permissions that you can customise and assign to your players.

Roles and Permissions are how access to features from compatible mods are handled. In the vanilla Conan Exiles system, you're either an admin with full access, or you're not.
Via Sudo, access can be handled individually, letting you choose exactly who has access to what. 

For example, you might want to allow moderators to kick players, but not teleport around the map.
</chapter>

<procedure title="Assigning a permission to Everyone">
<step>Explore the permissions available to you.</step>
<step>Check the "Use /act command" permission.</step>
<step>Hit "Save Permissions".</step>

<video src="sudo-setup-4.mp4" preview-src="sudo-setup-4.png" width="500"/>
</procedure>

> **No chat system installed?**
>
> You likely saw a message that we don't have a chat system installed yet. Don't worry, we'll take care of that later.
>
{style="tip"}

## Wrap-up

You've just set up Sudo, congratulations! We've learned how to lock Super Admin access behind a password, and you learned the core concept of roles and permissions.
What we ended up with is a very basic configuration that we can build off.

### What's next?
Now that we have our basic setup, let's explore it. You'll learn more about how to navigate the Sudo admin panel in the next section.


