# XeroXFCE ISO Repo

<p align="center">
    <img width="300" src="https://i.imgur.com/QWqMIsr.png" alt="logo">
</p>

<h1 align="center">Must be on an *Arch* based Distro to build ISO.</h1>

<h2 align="center">Note :<br /> Not all of them are supported.<br />
Tool was tested on XeroLinux/ArcoLinux and EndeavourOS.
Please do not report it if it doesn't work on the Distro you rare on.<br />
</h2>

### How to get ISO
> This here, is a Spin, not to be confused with the KDE flagship. A Spin is a side-project not main one. Building it yourselves, is currently the *only* way to get it for *Free*. However, an ISO will be made available, to all who donate on any of,
> [**Ko-Fi**](https://ko-fi.com/xerolinux) // [**FundRazr**](https://fnd.us/523mC5) or [**LiberaPay**](https://liberapay.com/DarkXero/). <sup>[**`Why Paid ?`**](https://github.com/xerolinux/xero_xfce_iso/blob/main/support.md)</sup>

<p align="center">
    <img width="100%" src="https://i.imgur.com/raPQ8bJ.jpeg" alt="logo">
</p>

<h1 align="center">Skip to Step 2 if you are on XeroLinux</h1>

### Step 1 - Get Repo in to build :

Before we get started we will need to get the **ABS** repo in, that's where the new build tool is located. To do so need to edit the "pacman.conf". Here's how to do so :

Type the following command in terminal done !

```
sudo bash -c "$(curl -fsSL https://raw.githubusercontent.com/keyaedisa/valen_repo/trunk/install/addRepo2PacmanConf.sh)"
```

Now install the tool via,
```
sudo pacman -S abs
```
### Step 2 - Clone Build Repo :

Once you got Repos in, time to grab the build environment that you will be building from. Just note that you will need Git installed in order to do that.

**Install Git with :**
```
sudo pacman -S git
```
**Grab Build Env.**
```
cd ~ && git clone https://github.com/XeroLinuxDev/xero_xfce_iso.git
```

### Step 3 - Building the XeroXFCE ISO :

Now that we have build environment on our system, it's time to build it.

**Build ISO :**
```
cd ~/xero_x_iso/ && abs -xf
```

Follow the prompts, answer with either `y` or `n` when asked if you want to keep build/source directory, and `n` when aksed if you want to modify profile settings as this is intended for me, finally just input the date you are building ISO on, as I will ask about this in case of issues...

I hope this helps.. In case of other issues kindly find me on [**Discord**](https://discord.gg/Xg6T78ahtK)

Happy building
