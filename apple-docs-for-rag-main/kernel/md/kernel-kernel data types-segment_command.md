

- Kernel
- Kernel Data Types
-  segment_command 

# segment_command

macOS 10.6+

``` source
struct segment_command {
    ...
};
```

## Topics

### Instance Properties

cmd

Common to all load command structures. Set to `LC_SEGMENT` for this structure.

cmdsize

fileoff

Indicates the offset in this file of the data to be mapped at `vmaddr`.

filesize

flags

initprot

maxprot

nsects

segname

vmaddr

vmsize

Indicates the number of bytes of virtual memory occupied by this segment. See also the description of `filesize`, below.

