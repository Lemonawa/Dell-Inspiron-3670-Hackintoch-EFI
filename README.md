![Dell-Inspiron-3670-Hackintoch-EFI](https://user-images.githubusercontent.com/69106050/210545049-ca3bd112-88fc-43b2-940d-3b9278b27857.png)

## Version: 0.8.7
## Info:
* CPU: Intel(R) Core(TM) i5-9400 CPU @ 2.90GHz
* Display: Intel(R) UHD Graphics 630 | NVIDIA GeForce GT 710
* Wireless: Atheros AR9565 802.11b/g/n Wireless Network Adapter
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
## Update Logs
2023/01/04 Rebuild all files;Update README.
