# What is this?

With the help of [@dreamwhite](https://github.com/dreamwhite) we thought that it would be useful to have a generic EFI with just the minumum requirements needed to obtain the most debugging logs from most motherboards as possible. Here we provide both the .zip file which can be extracted and copied to an ESP partition on a thumb drive, as well as the possibility to explore the files 

# Debugging features

The following repository will be used for debugging purposes, providing lots of functionalities such as:

- Checking `MAT` (Memory Attributes Table) support with OpenRuntime through OpenCore log
- Controlling `MSR 0xE2` writable status through OpenCore log  or `ControlMsrE2.efi` loadable from `OpenShell` 
- Checking the need of slide values or the necessity of the `ProvideCustomSlide` quirk (found on OpenCore log) or though the MmapDump.efi tool
- Checking CFG-Lock (`MSR 0xE2` register write lock) status though OpenCore log
- Custom grub shell to use when `setup_var` is needed to change hidden bios options
- `RtcRw.efi` tool to dump the RTC memory regions
- Dumping with `SysReport` set to `True` by default:
    - ACPI tables (DSDT, SSDTs) 
    - Audio Codec info
    - CPU features
    - PCI `vendor-id` and `device-id` with the respective PCI paths
    - SMBIOS with `SysReport` set to `True`.

# Credits:

- [Acidanthera](https://github.com/acidanthera) team, [mhaeuser](https://github.com/mhaeuser) and [vit9696](https://github.com/vit9696) in particular
- [datastone](https://github.com/datastone) for the modifiedgrubshell tool
- [derbrumbaer](https://github.com/derbrumbaer) and [zhen-zen](https://github.com/zhen-zen) for ControlMsrE2.efi
- [khronokernel](https://github.com/khronokernel) and dortania for their guides
- [dreamwhite](https://github.com/dreamwhite) for his costant commitment and maintaining the releases in sync
- [a23ss4ndro](https://github.com/1alessandro1) for some random fixes

# P.S.

Dear clowns at [HackintoshLifeIT](https://github.com/hackintoshlifeit), instead of stealing other's work, why don't you try linking this repo and giving credits where it's due?
