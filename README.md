# Initial-Windows-Apps-Installation
Install with chocolatey automatically all important apps for development

## [Chocolatey](https://chocolatey.org/)

1. Install chocolatey in windows powershell as administrator - https://chocolatey.org/install

```sh
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
```

2. Install choco packages using packages.config ( change with your path of packages config file )

```sh
choco install c:\shared\packages.config -y
```

3. Wait until finish installation and you are ready for 👨‍💻👨‍💻👨‍💻👨‍💻!!! 

**If you want to export from existing choco machine then :**
<br/>
<ins>change folderName</ins>
```sh 
choco export -o="'c:\{folderName}\packages.config'"
```

**Update choco packages**
```sh 
choco update all -y
```

## Usefull Links
* [Choco Install](https://chocolatey.org/install)
* [Choco Packages](https://community.chocolatey.org/packages)
* [Choco Cli](https://docs.chocolatey.org/en-us/choco/)

