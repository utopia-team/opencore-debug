With the help of [@dreamwhite](https://github.com/dreamwhite) we thought that it would be useful to have a generic EFI with just the minumum requirements needed to obtain the most debugging logs from most motherboards as possible. Here we provide both the .zip file which can be extracted and copied to an ESP partition on a thumb drive, as well as the possibility to expore the files 

# EFI for OpenCore Debugging

The following repository will be used for debugging purposes, providing lots of functionalities such as:

- Checking MAT (Memory Attributes Table) support with OpenRuntime though OpenCore log
- Checking the need of slide values or the necessity of the "ProvideCustomSlide" quirk (found on OpenCore log) or though the MmapDump.efi tool
- Checking if CFG-Lock MSR0xE2 register is unlocked though OpenCore log or VerifyMSRE2.efi tool.
- Original OpenCore EFI Shell (bundled with OC, also known as OpenShell.efi)
- Custom grub shell to use when setup_var is needed to change hidden bios options
- RtcRw.efi tool to dump the RTC memory regions
- Dumping ACPI tables (DSDT, SSDTs) and SMBIOS with SysReport set to True.

- Even more which I forgot to mention

# Credits:

- Acidanthera team, Download-Fritz and vit9696 in particular
- datastone for the modifiedgrubshell tool
- khronokernel and dortania for their guides
- dreamwhite for his costant commitment 
- a23ss4ndro for some random fixes
