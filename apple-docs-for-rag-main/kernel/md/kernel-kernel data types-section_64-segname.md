

- Kernel
- Kernel Data Types
- section_64
-  segname 

Instance Property

# segname

A string specifying the name of the segment that should eventually contain this section. For compactness, intermediate object files—files of type `MH_OBJECT`—contain only one segment, in which all sections are placed. The static linker places each section in the named segment when building the final product (any file that is not of type `MH_OBJECT`).

macOS 10.6+

``` source
char segname[16];
```

