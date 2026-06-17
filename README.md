# Ragnarok Revisited — Client Releases

Full client builds and incremental patches for [Ragnarok Revisited](https://ragnarokrevisited.com).

## Quick Install

### Step 1: Download

Go to the [Releases](https://github.com/ragnarokrevisited/releases/releases) page and download **all 4 files** from the latest release:

- `Combine-Parts.bat`
- `RO-Full-v*.zip.part-aa`
- `RO-Full-v*.zip.part-ab`
- `RO-Full-v*.zip.part-ac`

Put them all in the **same folder** on your computer.

### Step 2: Double-click Combine-Parts.bat

That's it. The tool will merge the parts back into a single ZIP file automatically. No command prompt, no typing.

### Step 3: Extract

Right-click the resulting `.zip` file → **Extract All** (or use 7-Zip / WinRAR).

### Step 4: Play

1. Run **`opensetup.exe`** — set Graphics API to DirectX 7
2. Run **`Ragnarok Revisited Client.exe`** to launch
3. Log in with **`admin_M`** / **`password`**

---

## Prerequisites (one-time)

| Required | Download |
|----------|----------|
| Visual C++ Redistributable | [Download](https://github.com/abbodi1406/vcredist/releases/latest/download/VisualCppRedist_AIO_x86_x64.exe) |
| DirectX Runtime | [Download](https://download.microsoft.com/download/1/7/1/1718CCC4-6315-4D8E-9543-8E28A4E18C4C/dxwebsetup.exe) |
| kRO Full Client (fresh installs only) | [Download](https://download.ragnarok.com/download/webclient/) |

**Already have kRO installed?** Just extract this release on top of your existing kRO folder.
**Fresh install?** Download and install kRO first, then extract this release on top.

## Updates

Launch **`Ragnarok Revisited.exe`** instead of the game EXE directly. The patcher automatically checks for updates, downloads them, and applies them before starting the game.

## Troubleshooting

| Problem | Solution |
|---------|----------|
| Combine-Parts.bat says no files found | Make sure all `.part-*` files are in the same folder as the `.bat` file |
| Crash on launch | Install VC++ Redist and DirectX Runtime (see Prerequisites) |
| Black screen | Run `opensetup.exe` and set Graphics API to **DirectX 7** |
| Korean / garbled text | Re-extract — the `SystemEN` folder may be missing |
| "Disconnected" immediately | Server may be down — check Discord |
