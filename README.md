<picture><img align="left" src="/Img/Logo.png" width="20%"/></picture>
<h1>UXTU4Mac (WIP)</h1>
<h3>Based on RyzenAdj and Python</h3>

![GitHub Downloads (all assets, latest release)](https://img.shields.io/github/downloads/AppleOSX/UXTU4Mac/total)

---

## Supported APU
> [!NOTE]
> - AMD Zen-based processors that are supported [NootedRed](https://github.com/ChefKissInc/NootedRed) **or** [UXTU](https://github.com/JamesCJ60/Universal-x86-Tuning-Utility) **Premade Preset** section (or just simply support RyzenAdj)

## Usage
- Download the official build from Releases.
- Run `UXTU4Mac.command`.
- Follow the instructions.
- [Optional] Disable `Core Performance Boost` in BIOS using [Smokeless_UMAF](https://github.com/DavidS95/Smokeless_UMAF) to chieve better temperature but sacrifice a lot of CPU performance.

## FAQ
### 1. Why do we have to disable SIP in macOS?
- Honestly, the binary file (ryzenAdj and DirectHW) is recognized in macOS as untrusted kexts. So, in order to get it working, we have to disable SIP including the flag `ALLOW_UNTRUSTED_KEXTS` (0x1).
### 2. Why does `UXTU4Mac` lack CPU support?
- When I ported a bunch of AMD APU presets from `UXTU` to `UXTU4Mac`, some commands were not compatible with ryzenAdj (because `UXTU` uses lots of methods to change CPU/APU settings besides ryzenAdj), especially the CPU presets. So, I could only keep some commands as a `work-around`.
### 3. GUI wen eta?
- `idk` - NotchApple1703 said to me, but we will release it soon.

## For advanced users, please visit [Custom.md](Custom.md).
## Comparison 

|  | UXTU | UXTU4Mac |  
|    :---:     |    :---:   |    :---:   |
| GUI | ✅ | ❌ No, currently only for CLI |
| Adjust power management settings | ✅ | ✅ |
| Premade presets | ✅ | ✅ |
| Custom presets | ✅ | ❓ |
| Adaptive mode tracking | ✅ | ✅ |
| Game mode tracking | ✅ | ❓ |
| Support for many hardware | ✅ | ❌ Only for some AMD Ryzen APU/CPU models, [see here](#supported-cpuapu) |

# Preview
> [!NOTE]
> The `Dynamic Mode` logic results in better power management, providing 2:30 hours of battery usage
> - The `Extreme` or `AC` presets yields the full potential performance that my Ryzen 5 4500U (Renoir) can handle, but it only lasts for 1:30 hours of battery usage. To achieve maximum performance, please use the device with AC power.

<p align="left">
  <img src="/Img/main_menu.png">
  <img src="/Img/apply_preset.png">
  <img src="/Img/preset.png">
  <img src="/Img/preset_setting.png">
  <img src="/Img/settings.png">
</p>

### Extreme Preset
![Screenshot 2024-02-12 at 15 52 16](https://github.com/AppleOSX/UXTU4Mac/assets/98001973/19e1481a-07ae-4efb-9b50-fac0cf137e0a)
### Special thanks to
- [corpnewt](https://github.com/corpnewt) for command file
- [NotchApple1703](https://github.com/NotchApple1703) for the GUI (starting from version `0.3.x` or `0.4.x`)
- [b00t0x](https://github.com/b00t0x) for the guide to build ryzenAdj based on DirectHW and pciutils-osx
- [JamesCJ60](https://github.com/JamesCJ60) for [UXTU](https://github.com/JamesCJ60/Universal-x86-Tuning-Utility)
