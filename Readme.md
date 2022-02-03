## install powerShell 7 from microsoft store
## install phmyposh 
```
winget install janDeDobbeleer.OhMyPosh
```

## create powershell config file 
documents/powerShell/Microsoft.PowerShell_profile.ps1
### drop that line in the file
```
oh-my-posh --init --shell pwsh --config ~/jandedobbeleer.omp.json | Invoke-Expression
```
## set as default profile 
```
. $PROFILE
```
## search for 
```
dir jandedobbeleer.omp.json /s
```
then go to directory outputted
## download the theme 
```
https://gist.github.com/shanselman/1f69b28bfcc4f7716e49eb5bb34d7b2c?WT.mc_id=-blog-scottha
```
put it in the theme directory folder
## change the default theme 
edit the Microsoft.PowerShell_profile.ps1 => oh-my-posh --init --shell pwsh --config C:\Users\rredo\Documents\GitHub\prompt\ohmyposhv3.json | Invoke-Expression

## install terminal icon 
```
install-Module -Name Terminal-Icons -Repository PSGallery
```
### then
```
Import-Module -Name Terminal-Icons
```
## install ps prediction 
```
Install-Module PSReadLine -RequiredVersion 2.2.0-beta1 -AllowPrerelease
```
## enable it 
```
Set-PSReadLineOption -PredictionSource History
```

## install module z 
```
install-Module z -AllowClobber
```

## useful links
https://www.hanselman.com/blog/powershell-720-could-not-load-type-systemmanagementautomationsubsystempredictionresult
https://www.hanselman.com/blog/how-to-make-a-pretty-prompt-in-windows-terminal-with-powerline-nerd-fonts-cascadia-code-wsl-and-ohmyposh
