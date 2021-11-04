# How to make a pretty prompt in Windows
![](https://github.com/oliversteidel/prettyprompt/blob/main/images/prettyprompt.jpg)

## Step 1

<br>

- Get Windows Terminal
- I recommend to install it from the Microsoft Store to get updates automatically

---

## Step 2

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
