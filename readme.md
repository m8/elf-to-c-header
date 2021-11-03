# elf-to-c-header

Split ELF to single C/C++ header file.

Usage:

```
g++ elf-to-c-header.cpp
./elf-to-c-header "file.elf"
```

Output (at `out.h`):

```c
#ifndef vm_elf_h
#define vm_elf_h

unsigned long vm_entry = 120;
unsigned char vm_text_section_data [] = { -1,67,0 ...};
unsigned long vm_text_section_size = 248;
unsigned long vm_text_section_offset = 65536;
unsigned long vm_text_section_start = 1342177280;
unsigned char vm_bss_section_data [] = { 0,0,0,0 };
unsigned long vm_bss_section_size = 4;
unsigned long vm_bss_section_offset = 65784;
unsigned char vm_symtab_section_data [] = { 0,0 ...};
unsigned long vm_symtab_section_size = 408;
unsigned long vm_symtab_section_offset = 65784;
unsigned char vm_strtab_section_data [] = { 0,109 ...};
unsigned long vm_strtab_section_size = 72;
unsigned long vm_strtab_section_offset = 66192;
unsigned char vm_shstrtab_section_data [] = { 0,46 ...};
unsigned long vm_shstrtab_section_size = 38;
unsigned long vm_shstrtab_section_offset = 66264;

#endif

```
