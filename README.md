<picture><img align="left" src="/Img/Logo.png" width="20%"/></picture>
<h1>RielUXTU4Mac - Project AppleOSX</h1>
<h3>UXTU but for macOS</h3></h3>
<h4>Supported for AMD Ryzen APUs (hackintosh)</h4>

#

## Usage

- Add kext
- Disable SIP ( <7F080000> )
- Add `debug=0x44` to boot-args
- [OPTIONAL] Disable CPS in BIOS using UMAF to get better temp but will sacrifice a lot of performance
- Run `start-macOS.command`
  

### Auto preset results in better power management (2:30 hours of my battery usage)
### The Extreme preset yields the full potential performance that my Ryzen 5 4500U (Renoir) can handle but only lasts for 1:30 hours of my battery usage, to achieve maximum performance please plug in with AC.
### [Removed] ECO Preset
![IMG_0124](https://github.com/gorouflex/RielUXTU4Mac/assets/98001973/1d67984a-1166-4551-a1b6-04865b72c53b)

### [Replaced with another args] Extreme Preset
![IMG_0123](https://github.com/gorouflex/RielUXTU4Mac/assets/98001973/46565c9a-8abd-4b9f-ad2e-5bde5c39a4c1)

### Special thanks to
- [NotchApple1703](https://github.com/NotchApple1703) for GUI ( after ver 0.1.x )
- [b00t0x](https://github.com/b00t0x) for guide
- [JamesCJ60](https://github.com/JamesCJ60) for [UXTU](https://github.com/JamesCJ60/Universal-x86-Tuning-Utility)
