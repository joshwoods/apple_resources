

- Kernel
- Kernel Data Types
-  section_64 

# section_64

macOS 10.6+

``` source
struct section_64 {
    ...
};
```

## Topics

### Instance Properties

addr

align

flags

nreloc

offset

reloff

reserved1

reserved2

reserved3

sectname

segname

A string specifying the name of the segment that should eventually contain this section. For compactness, intermediate object files—files of type `MH_OBJECT`—contain only one segment, in which all sections are placed. The static linker places each section in the named segment when building the final product (any file that is not of type `MH_OBJECT`).

size

