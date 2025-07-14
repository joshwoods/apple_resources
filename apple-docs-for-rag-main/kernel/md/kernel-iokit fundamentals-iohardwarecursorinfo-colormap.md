

- Kernel
- IOKit Fundamentals
- IOHardwareCursorInfo
-  colorMap 

Instance Property

# colorMap

Pointer to array of IOColorEntry structures, with the number of elements set by the numColors field of the IOHardwareCursorDescriptor. Zero should be passed for direct pixel formats.

macOS 10.0+

``` source
IOColorEntry *colorMap;
```

