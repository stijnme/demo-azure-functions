# Demo

## Tooling

Installed `Azure Function Core Tools` in `Ubuntu` running in `wsl`:

```
curl https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > microsoft.gpg
sudo mv microsoft.gpg /etc/apt/trusted.gpg.d/microsoft.gpg
sudo sh -c 'echo "deb [arch=amd64] https://packages.microsoft.com/repos/microsoft-ubuntu-$(lsb_release -cs)-prod $(lsb_release -cs) main" > /etc/apt/sources.list.d/dotnetdev.list'
less /etc/apt/sources.list.d/dotnetdev.list
nvim /etc/apt/sources.list.d/dotnetdev.list
uname -v
more /etc/issue
sudo apt-get update
sudo apt-get install azure-functions-core-tools-4
```

## Create project

Created new directory:

```
mkdir demo-azure-functions
cd demo-azure-functions
```

Started Visual Studio code in this directory:

```
code .
```

Followed tutorial to:

- generate the project
- test the project
- deployed to Azure

[First Azure Function with Typescript](https://learn.microsoft.com/en-us/azure/azure-functions/create-first-function-vs-code-typescripth)
