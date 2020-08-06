# EFI for OpenCore-debugging

The following repository will be used for debugging purposes, providing lots of functionalities such as:

-Checking MAT support with OpenRuntime though OpenCore log
-Checking the need of slide values or the necessity of the "ProvideCustomSlide" quirk (found on OpenCore log) or though the MmapDump.efi tool
-Checking if CFG-Lock MSR0xE2 register is unlocked though OpenCore log or VerifyMSRE2.efi tool.
-Dumping ACPI tables (DSDT, SSDTs) and SMBIOS with SysReport set to True.

-Even more which I forgot to mention

# Credits:

-Acidanthera team, Download-Fritz and vit9696 in particular
-Dreamwhite
-a23ss4ndro
