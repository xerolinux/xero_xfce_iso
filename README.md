# XeroXFCE ISO Dev Repo

<p align="center">
    <img width="300" src="https://i.imgur.com/QWqMIsr.png" alt="logo">
</p>

<h1 align="center">You must be on an *Arch* based Distro to build ISO.</h1>

> The following are not supported Distros to build on since they
> don't use Arch repos which will result in errors building the ISO.
> - Garuda Linux (Fails to build)
> - Manjaro (Own Repos)
> - CachyOS (Arch v3)
> - KaOS (Limited Repos)
> - Artix (No Systemd)

<p align="center">
    <img width="600" src="https://i.imgur.com/ZRV75N6.png" alt="logo">
</p>

### Step 1 - Get Repo in to build :

Before we get started we will need to get the **ABS** repo in, that's where the new build tool is located. To do so need to edit the "pacman.conf". Use either methods to do so :

**- Method 1 :**

```
sudo nano /etc/pacman.conf
```

Now we need to add the repo at the end of the file, so add this,
```
# Valen Repository
[valen_repo]
SigLevel = Never
Server = https://keyaedisa.github.io/$repo/$arch
```

**- Method 2 :**

Type the following command using `sudo` in terminal done !

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
cd ~/xero_x_iso/ && abs -c
```

When prompted for profile type `XeroCE`... Then follow rest of prompts..

I hope this helps.. In case of other issues kindly find me on [**Discord**](https://discord.gg/Xg6T78ahtK)

Happy building
