# How to make a pretty prompt in Windows

![](https://github.com/oliversteidel/prettyprompt/blob/main/images/prettyprompt.jpg)

## Step 1 - Get Windows Terminal

<br>

- Get Windows Terminal
- I recommend to install it from the Microsoft Store to get updates automatically

---

## Step 2 - Install Posh-Git & Oh-My-Posh

<br>

- This assumes you've installed Git for Windows
- Per these directions, install Posh-Git and Oh-My-Posh

```
    Install-Module posh-git -Scope CurrentUser
    Install-Module oh-my-posh -Scope CurrentUser
```

<br>

- Then run <strong>"notepad $profile"</strong> and add the following lines to the end:

```
    Import-Module posh-git
    Import-Module oh-my-posh
    Set-PoshPrompt -Theme Paradox
```

---

## Step 3 - Allow Powershell scripts

<br>
When you start your terminal, there might be an error, if running scripts is disabled on your system (which is the default).<br>
To fix this run powershell as administrator and set ExecutionPolicy to RemoteSigned:

```
    Set-ExecutionPolicy RemoteSigned
```

Find further information about Powershell ExecutionPolicy in the [Documentation](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.security/set-executionpolicy?view=powershell-7.2).

---

## Step 4 - Get a Nerd Font

<br>

- go to the [this GitHub repo](https://github.com/ryanoasis/nerd-fonts/tree/master/patched-fonts) and download a nerd font
- the nerd font **Meslo LGM NF** is recommended which includes all the icons you will need for the themes
- extract the downloaded ZIP-file and paste it into your windows fonts folder

---

## Step 5 - Choose a theme

<br>

- have a look at all the availible themes on [Oh My Posh Docs - themes](https://ohmyposh.dev/docs/themes)
- to change your theme in your terminal run <strong>"notepad $profile"</strong> and change the name to the theme of your choise

```
    Set-PoshPrompt -Theme [name of the theme]
```

---

If you like to customize a theme or create your own theme, you find information on <br> https://ohmyposh.dev/docs/config-overview
