# What is this?

With the help of [@dreamwhite](https://github.com/dreamwhite) we thought that it would be useful to have a generic EFI with just the minumum requirements needed to obtain the most debugging logs from most motherboards as possible. Here we provide both the .zip file which can be extracted and copied to an ESP partition on a thumb drive, as well as the possibility to explore the files 

# Debugging features

The following repository will be used for debugging purposes, providing lots of functionalities such as:

- Checking MAT (Memory Attributes Table) support with OpenRuntime through OpenCore log
- Controlling MSR 0xE2 status through ControlMsrE2.efi interactive UEFI tool (credits [derbrumbaer](https://github.com/derbrumbaer))
- Checking the need of slide values or the necessity of the "ProvideCustomSlide" quirk (found on OpenCore log) or though the MmapDump.efi tool
- Checking if CFG-Lock MSR 0xE2 register is unlocked though OpenCore log, ControlMsrE2 or VerifyMSRE2.efi tool.
- Original OpenCore EFI Shell (bundled with OC, also known as OpenShell.efi)
- Custom grub shell to use when setup_var is needed to change hidden bios options
- RtcRw.efi tool to dump the RTC memory regions
- Dumping ACPI tables (DSDT, SSDTs) and SMBIOS with SysReport set to True.

- Even more which I forgot to mention

# Credits:

- [Acidanthera](https://github.com/acidanthera) team, [mhaeuser](https://github.com/mhaeuser) and [vit9696](https://github.com/vit9696) in particular
- [datastone](https://github.com/datastone) for the modifiedgrubshell tool
- [khronokernel](https://github.com/khronokernel) and dortania for their guides
- [dreamwhite](https://github.com/dreamwhite) for his costant commitment 
- [a23ss4ndro](https://github.com/1alessandro1) for some random fixes
