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

## Cloning SillyTavern-extras repository and making some changes 

<details>
  <summary><strong>Clone the Extras repository</strong></summary>

```bash
git clone https://github.com/Cohee1207/TavernAI-extras
```

</details>

<details>
  <summary><strong>Move to SillyTavern-extras folder</strong></summary>

```bash
cd TavernAI-extras
```

</details>

<details>
  <summary><strong>Edite requirements-complete.txt</strong></summary>

```bash
nano requirements-complete.txt
```

- Search for "torch==2.0.0+cu117" and remove the "+cu117".
- search for "torchaudio==2.0.1+cu117" and also remove the "+cu117".
- To save the changes made, just press the Ctrl button and the x key. Confirm the changes by pressing the y key and finally press enter.

  </details>

## Install requirements-complete.txt

- Depending on your device and internet speed, this process may take some time. 

```bash
pip install -r requirements-complete.txt
```
</details>

##  Fixing Host address error

<details>
  <summary><strong>Accessing and Editing the Hosts File</strong></summary>

  
- If you want to use the chromadb module, you need to do some simple steps. Otherwise, you will receive the following error: Name or service not known 

```bash
nano /etc/hosts
```

- When running the above command you probably got an empty screen/file, this is what causes the error. Copy the address below and just paste it on the empty screen/file given by "nano /etc/hosts" earlier. Save and exit, as before. 

```bash
127.0.0.1 localhost
```

</details>

##  Run chromadb module

<details>
  <summary><strong>Running chromadb module, the Smart Context</strong></summary>

- Now, you should be able to run the chromadb module and others. Just use the command below and wait for the necessary requirements for chromadb to download and start it. 


```bash
python3 server.py --enable-module=chromadb
```

</details>
