# Extras-in-Termux

## Installation Dependecies

> **Attention!**
>
> - [Termux must be **F-Droid** Version](https://f-droid.org/en/packages/com.termux/) because Termux from Playstore no longer maintained because there are some problems with the Playstore publishing

  <details open>
  <summary><strong>Update Repository & Upgrade Package</strong></summary>

```bash
pkg update && pkg upgrade
```

  </details>

  <details>
  <summary><strong>git & wget & proot</strong></summary>

- Package `git` for cloning or downloading repository

```bash
pkg i -y git
```

- Package `wget` is required in Ubuntu installation

```bash
pkg I -y wget
```
  
- `proot` to run Ubuntu

```bash
pkg install proot
```

  </details>

## Installation Ubuntu ##

<details open>
  <summary><strong>Clone or Download This Repository</strong></summary>

```bash
git clone https://github.com/MFDGaming/ubuntu-in-termux.git
```

  </details>

  <details>
  <summary><strong>Run Script Installer</strong></summary>

- Move to Folder

```bash
cd ubuntu-in-termux
```

- Give execution permission

```bash
  chmod +x ubuntu.sh
```

- Execute Installer

```bash
  ./ubuntu.sh -y
```

- Now just start ubuntu

```bash
  ./startubuntu.sh
```

</details>

## Installation Dependecies in Ubuntu

<details>
  <summary><strong>Update Ubuntu</strong></summary>

```bash
apt update && apt upgrade -y
```

</details>

<details>
  <summary><strong>Install Python3 & pip packegs</strong></summary>

```bash
apt install python3 && apt update && apt install python3-pip
```

</details>

<details>
  <summary><strong>Install nano</strong></summary>

```bash
apt install nano
```

</details>

<details>
  <summary><strong>Install git </strong></summary>

```bash
apt install git -y
```

</details>
