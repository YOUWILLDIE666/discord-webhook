```bat
@REM Building:
vcpkg install curlpp nlohmann-json
git clone https://github.com/YOUWILLDIE666/discord-webhook.git && CD discord-webhook
mkdir build && cd build
cmake .. -DCMAKE_TOOLCHAIN_FILE=%VCPKG_ROOT%/scripts/buildsystems/vcpkg.cmake
cmake --build .
```
```bat
@REM Arguments that can be passed:
DiscordWebhook.exe --delete webhookl_url
DiscordWebhook.exe --json input.json
```