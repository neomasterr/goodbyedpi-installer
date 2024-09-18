# Установка GoodbyeDPI

## Запустить консоль (CMD)
`Win + R` -> `cmd`

## Вставить

```
del /F /Q goodbyedpi-installer.zip && \
curl -L https://github.com/neomasterr/goodbyedpi-installer/archive/refs/tags/v1.0.1.zip -o goodbyedpi-installer.zip && \
powershell -Command "Expand-Archive goodbyedpi-installer.zip -DestinationPath goodbyedpi-installer" && \
start goodbyedpi-installer\goodbyedpi-installer-1.0.1\install.bat && \
del /F /S /Q goodbyedpi-installer && \
echo Done
```