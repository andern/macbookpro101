# MacBook Pro Retina February 2013
On a working system:
```
$ lspci
00:00.0 Host bridge: Intel Corporation 3rd Gen Core processor DRAM Controller (rev 09)
00:01.0 PCI bridge: Intel Corporation Xeon E3-1200 v2/3rd Gen Core processor PCI Express Root Port (rev 09)
00:01.1 PCI bridge: Intel Corporation Xeon E3-1200 v2/3rd Gen Core processor PCI Express Root Port (rev 09)
00:01.2 PCI bridge: Intel Corporation Xeon E3-1200 v2/3rd Gen Core processor PCI Express Root Port (rev 09)
00:02.0 VGA compatible controller: Intel Corporation 3rd Gen Core processor Graphics Controller (rev 09)
00:14.0 USB controller: Intel Corporation 7 Series/C210 Series Chipset Family USB xHCI Host Controller (rev 04)
00:16.0 Communication controller: Intel Corporation 7 Series/C210 Series Chipset Family MEI Controller #1 (rev 04)
00:1a.0 USB controller: Intel Corporation 7 Series/C210 Series Chipset Family USB Enhanced Host Controller #2 (rev 04)
00:1b.0 Audio device: Intel Corporation 7 Series/C210 Series Chipset Family High Definition Audio Controller (rev 04)
00:1c.0 PCI bridge: Intel Corporation 7 Series/C210 Series Chipset Family PCI Express Root Port 1 (rev c4)
00:1c.1 PCI bridge: Intel Corporation 7 Series/C210 Series Chipset Family PCI Express Root Port 2 (rev c4)
00:1d.0 USB controller: Intel Corporation 7 Series/C210 Series Chipset Family USB Enhanced Host Controller #1 (rev 04)
00:1f.0 ISA bridge: Intel Corporation HM77 Express Chipset LPC Controller (rev 04)
00:1f.2 SATA controller: Intel Corporation 7 Series Chipset Family 6-port SATA Controller [AHCI mode] (rev 04)
00:1f.3 SMBus: Intel Corporation 7 Series/C210 Series Chipset Family SMBus Controller (rev 04)
01:00.0 VGA compatible controller: NVIDIA Corporation GK107M [GeForce GT 650M Mac Edition] (rev a1)
01:00.1 Audio device: NVIDIA Corporation GK107 HDMI Audio Controller (rev a1)
03:00.0 Ethernet controller: Broadcom Corporation Device 16a3 (rev 10)
03:00.1 SD Host controller: Broadcom Corporation NetXtreme BCM57765 Memory Card Reader (rev 10)
04:00.0 Network controller: Broadcom Corporation BCM4331 802.11a/b/g/n (rev 02)
05:00.0 PCI bridge: Intel Corporation DSL3510 Thunderbolt Port [Cactus Ridge] (rev 03)
06:00.0 PCI bridge: Intel Corporation DSL3510 Thunderbolt Port [Cactus Ridge] (rev 03)
06:03.0 PCI bridge: Intel Corporation DSL3510 Thunderbolt Port [Cactus Ridge] (rev 03)
06:04.0 PCI bridge: Intel Corporation DSL3510 Thunderbolt Port [Cactus Ridge] (rev 03)
06:05.0 PCI bridge: Intel Corporation DSL3510 Thunderbolt Port [Cactus Ridge] (rev 03)
06:06.0 PCI bridge: Intel Corporation DSL3510 Thunderbolt Port [Cactus Ridge] (rev 03)
07:00.0 System peripheral: Intel Corporation DSL3510 Thunderbolt Port [Cactus Ridge] (rev 03)
08:00.0 PCI bridge: Intel Corporation DSL3510 Thunderbolt Controller [Cactus Ridge]
09:00.0 PCI bridge: Intel Corporation DSL3510 Thunderbolt Controller [Cactus Ridge]
0a:00.0 Ethernet controller: Broadcom Corporation NetXtreme BCM57762 Gigabit Ethernet PCIe
```

```
$ lsmod
Module Size Used by
vboxnetflt 14802 2
vboxnetadp 17542 0
vboxdrv 1776879 6 vboxnetadp,vboxnetflt
snd_hda_codec_hdmi 28105 1
asix 20387 0
usbnet 19005 1 asix
snd_hda_codec_cirrus 7148 1
nouveau 943350 2
mxm_wmi 1323 1 nouveau
i915 491290 1
wmi 7723 2 mxm_wmi,nouveau
ttm 60207 1 nouveau
intel_agp 10504 1 i915
tg3 147978 0
intel_gtt 11974 2 i915,intel_agp
ptp 7724 1 tg3
drm_kms_helper 27023 2 i915,nouveau
pps_core 6521 1 ptp
snd_hda_intel 29000 7
drm 216578 6 ttm,i915,drm_kms_helper,nouveau
libphy 18582 2 tg3,asix
snd_hda_codec 119695 3 snd_hda_codec_hdmi,snd_hda_intel,snd_hda_codec_cirrus
agpgart 25916 4 drm,ttm,intel_agp,intel_gtt
ehci_pci 3776 0
ehci_hcd 46125 1 ehci_pci
xhci_hcd 86023 0
snd_hwdep 5900 1 snd_hda_codec
apple_gmux 5171 0
apple_bl 2800 1 apple_gmux
video 11024 3 i915,nouveau,apple_gmux
```
