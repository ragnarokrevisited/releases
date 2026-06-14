# Ragnarok Revisited — Client Releases

Full client builds and incremental patches for [Ragnarok Revisited](https://github.com/ragnarokrevisited).

## Download

### Prerequisites

- [kRO Full Client](https://download.ragnarok.com/download/webclient/) (~4 GB) — extract to a folder
- [Visual C++ Redistributable AIO](https://github.com/abbodi1406/vcredist/releases/latest/download/VisualCppRedist_AIO_x86_x64.exe)
- [DirectX Runtime](https://download.microsoft.com/download/1/7/1/1718CCC4-6315-4D8E-9543-8E28A4E18C4C/dxwebsetup.exe)

### Full Client

Download from the [Releases](https://github.com/ragnarokrevisited/releases/releases) page.

If the client is split into multiple parts (GitHub's 2 GB limit), recombine them:

```cmd
copy /b RO-Full-v*.zip.part-* RO-Full-v*.zip
```

Then extract all contents into your kRO folder, overwriting existing files.

### Configuration

1. Run `opensetup.exe` — set resolution, choose **DirectX 7**
2. Run `Ragnarok Revisited Client.exe` to launch the game
3. Log in with `admin_M` / `password` (the `_M` suffix auto-creates your account)

### Updates

Incremental patches are delivered automatically via `Ragnarok Revisited.exe` (the patcher).
On each launch it checks for new patches and applies them before starting the game.
