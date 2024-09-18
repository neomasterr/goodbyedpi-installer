# Установка GoodbyeDPI
## Запустить консоль (терминал)

`Win + R` -> `cmd`
или
`Win + X` -> `Терминал`

## Вставить

### Если CMD

```
del /F /Q install.bat && curl -L https://raw.githubusercontent.com/neomasterr/goodbyedpi-installer/refs/heads/master/install.bat -o install.bat && start /wait install.bat && del /F /Q install.bat && echo Done && cls

```

### Если PowerShell

```
Remove-Item -Force install.bat; `
Invoke-WebRequest -Uri "https://raw.githubusercontent.com/neomasterr/goodbyedpi-installer/refs/heads/master/install.bat" -OutFile "install.bat"; `
Start-Process -FilePath "install.bat" -Wait; `
Remove-Item -Force -Recurse "install.bat"; `
Write-Host "Done"; `
Clear-Host

```

https://github.com/ValdikSS/GoodbyeDPI