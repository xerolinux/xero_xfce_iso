# XeroXFCE ISO Repo

Repo for the **XeroXFCE** Project. Feel free to go through files and learn how it's all done. To build ISO need to use **ABS** Script via guide below.

<p align="center">
    <img width="300" src="https://i.imgur.com/QWqMIsr.png" alt="logo">
</p>

<h1 align="center">Must be on an *Arch* based Distro to build ISO.</h1>

<h3 align="center">||| Note |||<br />
Not all *Arch* based Distros are supported.<br />
Tool was tested on <a href="https://archlinux.org">Arch</a>/<a href="https://xerolinux.xyz">XeroLinux</a>/<a href="https://https://arcolinux.com/">ArcoLinux</a> & <a href="https://endeavouros.com/">EndeavourOS</a>.<br />
Please report any issues with **ABS** tool on dev's Github over <a href="https://github.com/keyaedisa/abs/issues">Here</a>.
</h3>

## How to get ISO

> This here, is a Spin, not to be confused with the KDE flagship. A Spin is a side-project not main one. Building it yourselves, is currently the *only* way to get it following the guide below, that way you always have the latest version available as of build time. However, we still need your help & support to keep project alive, so if you can please, show the project some love, scroll down for more info on how you can help.

<p align="center">
    <img width="100%" src="https://i.imgur.com/86Q3kVf.jpg" alt="logo">
</p>

<h1 align="center">Skip to Step 2 if you are on XeroLinux</h1>

## Step 1 - Get Repo in to build :

Before we get started we will need to get the **ABS** repo in, that's where the new build tool is located. To do so need to edit the "pacman.conf". Here's how to do so :

Type the following command in terminal done !

```
sudo bash -c "$(curl -fsSL https://raw.githubusercontent.com/keyaedisa/valen_repo/trunk/install/addRepo2PacmanConf.sh)"
```

Now install the tool via,
```
sudo pacman -S abs
```
## Step 2 - Clone Build Repo :

Once you got Repos in, time to grab the build environment that you will be building from. Just note that you will need Git installed in order to do that.

**Install Git with :**
```
sudo pacman -S git
```
**Grab Build Env.**
```
cd ~ && git clone https://github.com/xerolinux/xero_xfce_iso.git
```

## Step 3 - Building the XeroXFCE ISO :

Now that we have build environment on our system, it's time to build it.

**Build ISO :**
```
cd ~/xero_xfce_iso/ && abs -xf
```

Follow the prompts, answer with either `y` or `n` when asked if you want to keep build/source directory, and `n` when aksed if you want to modify profile settings as this is intended for me, finally just input the date you are building ISO on, as I will ask about this in case of issues...

## Support

A lot of hard work, and sleepless nights went into the creation of this awesome Ditro/Spin & build tool, with the current situation, in **Lebanon**, not being so great, geting only 4 hours of Government provided electricity, and 98% currency devaluation, among many other problems, I am limited on time & reources, with no other means of income to keep the Generator power running for longer than absolutely necessary as well as to cover server fees for hosting the sites and repos, I solely rely on your generous contributions. Any amount will go a long way making sure the project continues to thrive. So if you can please show me, the main Dev/Maintainer some love on [**Ko-Fi**](https://ko-fi.com/xerolinux) or [**Patreon**](https://patreon.com/xerolinux) or by becoming a [**Github Sponsor**](https://github.com/sponsors/xerolinux).

Also if you can, also show the rest of team the same love, you would the project, that would be highly appreaciated, by buying [**Keyaedisa**](https://github.com/keyaedisa/) the creator & maintainer of the awesome **ABS** build tool we use to give birth to all our ISOs, a [**Coffee**](https://www.buymeacoffee.com/keyaedisa) or two. As well as [**TeddyBearKilla**](https://github.com/TeddyBearKilla) our resident UI/UX specialist, on [**Ko-Fi**](https://ko-fi.com/teddybearkilla).. Thank you much.

*May You Live Long & Prosper*...

I hope this helps.. In case of other issues kindly find me on [**Discord**](https://discord.gg/Xg6T78ahtK)

Happy building
