# Ragnarok Revisited — Client Releases

Full client builds and incremental patches for [Ragnarok Revisited](https://ragnarokrevisited.com).

## How to Download & Install

### Step 1: Download the release

Go to the [Releases](https://github.com/ragnarokrevisited/releases/releases) page and download the latest version.

If the client is split into multiple parts (GitHub's 2 GB file limit), download **all parts** to the same folder.

**You'll need:**
- All `.part-*` files from the release
- A computer running Windows, Mac, or Linux

### Step 2: Recombine the parts

**Windows:**
Open Command Prompt (press Win+R, type `cmd`, press Enter), then navigate to your download folder:

```cmd
cd C:\Users\YourName\Downloads
copy /b RO-Full-v0.1.0.zip.part-aa + RO-Full-v0.1.0.zip.part-ab + RO-Full-v0.1.0.zip.part-ac RO-Full-v0.1.0.zip
```

Replace `YourName` with your Windows username. Wait for the message `1 file(s) copied`.

**Mac / Linux:**
Open Terminal, navigate to your Downloads folder:

```bash
cd ~/Downloads
cat RO-Full-v0.1.0.zip.part-* > RO-Full-v0.1.0.zip
```

### Step 3: Extract the ZIP

Right-click `RO-Full-v0.1.0.zip` → **Extract All** (Windows) or double-click to extract (Mac/Linux). You can also use [7-Zip](https://www.7-zip.org/) (free).

### Step 4: Prerequisites

Before launching, install these (one-time):

| Required | Download |
|----------|----------|
| Visual C++ Redistributable | [Download](https://github.com/abbodi1406/vcredist/releases/latest/download/VisualCppRedist_AIO_x86_x64.exe) |
| DirectX Runtime | [Download](https://download.microsoft.com/download/1/7/1/1718CCC4-6315-4D8E-9543-8E28A4E18C4C/dxwebsetup.exe) |
| kRO Full Client (fresh installs) | [Download](https://download.ragnarok.com/download/webclient/) |

**Already have kRO installed?** You can skip the kRO download — just extract this release's ZIP into your existing kRO folder, overwriting when prompted.

**Fresh install?** Download and install kRO first, then extract this release on top of it.

### Step 5: Configure & Play

1. Run **`opensetup.exe`** in the client folder
2. Set your screen resolution
3. Set **Graphics API** to **DirectX 7** (important — DirectX 9 can cause issues)
4. Check **"Restrict mouse to window"** if desired
5. Click Save
6. Run **`Ragnarok Revisited Client.exe`** to launch the game
7. Log in with:
   - **Username:** `admin_M`
   - **Password:** `password`
   - (The `_M` suffix auto-creates your account)

### Keeping Updated

Launch **`Ragnarok Revisited.exe`** instead of the game EXE directly. This patcher will:

1. Check for new updates on launch
2. Download and apply any patches automatically
3. Start the game for you

That's it! You only ever need to download the full client once — patches are small and automatic.

## Troubleshooting

| Problem | Solution |
|---------|----------|
| "Application not found" on recombine | Make sure all 3 `.part-*` files are in the same folder and you're running the command from that folder |
| Crash on launch | Install VC++ Redist and DirectX Runtime (Step 4) |
| Black screen / no display | Run `opensetup.exe` and set Graphics API to DirectX 7 |
| Korean / garbled text | The `SystemEN` folder wasn't extracted properly — re-extract the ZIP |
| "Disconnected" immediately | Server may be down for maintenance — check the Discord |
