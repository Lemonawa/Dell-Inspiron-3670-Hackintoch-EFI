![Dell-Inspiron-3670-Hackintoch-EFI](https://socialify.git.ci/Lemonawa/Dell-Inspiron-3670-Hackintoch-EFI/image?description=1&forks=1&issues=1&language=1&name=1&pulls=1&stargazers=1&theme=Light)

## Version: 0.9.0
## Info:
* CPU: Intel(R) Core(TM) i5-9400 CPU @ 2.90GHz
* Display: Intel(R) UHD Graphics 630 | NVIDIA GeForce GT 710
* Wireless: Atheros AR9565 802.11b/g/n Wireless Network Adapter (NOT AVAILABLE YET)
* Ethernet: Realtek RTL8168/8111 PCI-E Gigabit Ethernet Adapter
## BIOS Configuation
### Disable
* Fast Boot
* Secure Boot
* Serial/COM Port
* Parallel Port
* VT-d (can be enabled if you set `DisableIoMapper` to YES)
* Compatibility Support Module (CSM) (**Must be off in most cases, GPU errors/stalls like `gIO` are common when this option is enabled**)
* Thunderbolt (For initial install, as Thunderbolt can cause issues if not setup correctly)
* Intel SGX
* Intel Platform Trust
* CFG Lock (MSR 0xE2 write protection)(**This must be off, if you can't find the option then enable `AppleXcpmCfgLock` under Kernel -> Quirks. Your hack will not boot with CFG-Lock enabled**)
### Enable
* VT-x
* Above 4G Decoding
* Hyper-Threading
* Execute Disable Bit
* EHCI/XHCI Hand-off
* OS type: Windows 8.1/10 UEFI Mode (some motherboards may require "Other OS" instead)
* DVMT Pre-Allocated(iGPU Memory): 64MB or higher
* SATA Mode: AHCI
