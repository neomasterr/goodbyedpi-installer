# Установка GoodbyeDPI
## Запустить консоль (терминал)

`Win + R` -> `cmd`
или
`Win + X` -> `Терминал`

## Вставить

### Если CMD

```
del /F /Q goodbyedpi-installer.zip && curl -L https://github.com/neomasterr/goodbyedpi-installer/archive/refs/tags/v1.0.1.zip -o goodbyedpi-installer.zip && powershell -Command "Expand-Archive goodbyedpi-installer.zip -DestinationPath goodbyedpi-installer" && start /wait goodbyedpi-installer\goodbyedpi-installer-1.0.1\install.bat && del /F /S /Q goodbyedpi-installer && echo Done && cls

```

### Если PowerShell

```
Remove-Item -Force goodbyedpi-installer.zip; `
Invoke-WebRequest -Uri "https://github.com/neomasterr/goodbyedpi-installer/archive/refs/tags/v1.0.1.zip" -OutFile "goodbyedpi-installer.zip"; `
Expand-Archive -Path "goodbyedpi-installer.zip" -DestinationPath "goodbyedpi-installer"; `
Start-Process -FilePath "goodbyedpi-installer\goodbyedpi-installer-1.0.1\install.bat" -Wait; `
Remove-Item -Force -Recurse "goodbyedpi-installer"; `
Write-Host "Done"; `
Clear-Host

```

https://github.com/ValdikSS/GoodbyeDPI