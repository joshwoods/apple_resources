

- Kernel
- Kernel Data Types
- relocation_info
-  r_address 

Instance Property

# r_address

In `MH_OBJECT` files, an offset from the start of the section to the item containing the address requiring relocation.

macOS 10.8+

``` source
int32_t r_address;
```

## Discussion

In images used by the dynamic linker, this is an offset from the virtual memory address of the data of the first `segment_command` that appears in the file (not necessarily the one with the lowest address). For images with the `MH_SPLIT_SEGS` flag set, this is an offset from the virtual memory address of data of the first read/write `segment_command`.

If the high bit of this field is set (which you can check using the `R_SCATTERED` bit mask), the relocation_info structure is actually a scattered_relocation_info structure.

