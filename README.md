# Extras-in-Termux

### :exclamation: **IMPORTANT!**

⚠️ **Disclaimer**: This repository is provided "as is," and I take no responsibility for any problems or damages that may occur when using it. It is recommended to perform proper testing and understand the risks before executing any code from this repository.

⚠️ **Notice**: This repository is licensed under the GNU AFFERO GENERAL PUBLIC LICENSE License. Please read the license carefully before using the code from this repository.

⚠️ **Notice**: This repository was developed for educational e experimental purposes. Make sure to review and adapt the code before using it in a production environment.

⚠️ **Notice**: Support for this repository is limited, and I cannot guarantee immediate responses to issues or support requests. However, feel free to open issues or submit pull requests, and I will do my best to assist you.

⚠️ **Notice**: Contributions are welcome!

## Installation Dependecies

> **Attention!**
>
> - [Termux must be **F-Droid** Version](https://f-droid.org/en/packages/com.termux/) because Termux from Playstore no longer maintained because there are some problems with the Playstore publishing

  <details open>
  <summary><strong>Update Repository & Upgrade Package & install git, wget and proot</strong></summary>

```bash
pkg update && pkg upgrade && pkg i -y git && pkg i -y wget && pkg i proot -y
```

  </details>

- Package `git` for cloning or downloading repository
- Package `wget` is required in Ubuntu installation
- `proot` to run Ubuntu

## Ubuntu Installation and Booting ##

<details open>
  <summary><strong>Clone This Ubuntu Repository</strong></summary>

```bash
git clone https://github.com/MFDGaming/ubuntu-in-termux.git
```

  </details>

  <details>
  <summary><strong>Run Script Installer</strong></summary>

- Move to Folder

- Give execution permission

- Execute Installer

- Now just start ubuntu


```bash
cd ubuntu-in-termux && chmod +x ubuntu.sh && ./ubuntu.sh -y && ./startubuntu.sh
```

</details>

## Installation Dependecies in Ubuntu

<details>
  <summary><strong>Update Ubuntu and install required packages</strong></summary>

```bash
apt update && apt upgrade -y && apt install python3 && apt update && apt install python3-pip && apt install nano && apt install git -y
```

- Install `Python3` & `pip` packegs
- Install `nano`
- Install `git`

</details>

## Install requirements-complete.txt

- Depending on your device and internet speed, this process may take some time. 

```bash
git clone https://github.com/restartxx/Extras-in-Termux.git && cd Extras-in-Termux && pip install -r requirements-complete.txt
```
</details>

## Cloning SillyTavern-extras repository 

<details>
  <summary><strong>Clone the Extras repository</strong></summary>

- Now, with all the requirements already installed, choose which directory you think is most pleasant for the location of SillyTavern-extras. You can leave the current directory using the command `cd ..`

```bash
git clone https://github.com/Cohee1207/TavernAI-extras && cd TavernAI-extras
```

</details>

## Running the modules

- You should already be able to use almost all available modules. The only apparent exception is the module summarize which fails to initialize.
- Only during the first time when running any module, the process will take some time until the module initialization. This is because some required packages are being downloaded, so please wait.
- To run the modules, enter the previously cloned SillyTavern-extras directory and use the following command:

```bash
python3 server.py --enable-module=
```
- Just copy the command and paste it into Termux. Remember to add the name of the module you want to run at the end. For example: `python3 server.py --enable-module=chromadb`

- After the process ends you will probably get something like `http://localhost:5100`
- Copy it and paste it in space "extensions url" at SillyTavern.
- Finally press `connect` and you will be connected to the module.

</details>

##  Fixing Host address error before running the chromadb module ##

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

## Créditos

Este projeto utiliza os seguintes recursos e bibliotecas de terceiros:

- SillyTavern-extras (https://github.com/SillyTavern/SillyTavern-extras): A set of APIs for various SillyTavern extensions.
- Ubuntu-in-termux (https://github.com/MFDGaming/ubuntu-in-termux): This is a script that allows you to install Ubuntu in your termux application without a rooted device.

