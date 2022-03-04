# Windows terminal 配置

1. 下载所有依赖（主题、git、代码提示、图标）
    ```
    Install-Module oh-my-posh -Scope CurrentUser -SkipPublisherCheck
    Install-Module posh-git -Scope CurrentUser
    Install-Module -Name PSReadLine -AllowPrerelease -Scope CurrentUser -Force -SkipPublisherCheck
    Install-Module -Name Terminal-Icons -Repository PSGallery
    ```
2. 打开个人配置文件
    ```
    notepad.exe $PROFILE
    ```
3. 配置相关内容
    ```
    Import-Module posh-git
    Import-Module oh-my-posh
    Import-Module -Name Terminal-Icons
    Set-PoshPrompt -Theme robbyrussel
    Set-PSReadlineKeyHandler -Key Tab -Function MenuComplete
    ```
* 杂项
    * oh-my-posh文档 - [前往](https://ohmyposh.dev/docs)
    * oh-my-posh字体 - [oh-my-posh字体](https://www.nerdfonts.com/font-downloads)