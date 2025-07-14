

- Core Services
- File Metadata
- MDItem
- Common Metadata Attribute Keys
-  kMDItemCoverage 

Global Variable

# kMDItemCoverage

The extent or scope of the content of the resource. A CFString.

macOS 10.4+

``` source
let kMDItemCoverage: CFString!
```

## Discussion

Coverage will typically include spatial location (a place name or geographic co-ordinates), temporal period (a period label, date, or date range) or jurisdiction (such as a named administrative entity).

Recommended best practice is to select a value from a controlled vocabulary, and that, where appropriate, named places or time periods be used in preference to numeric identifiers such as sets of co-ordinates or date ranges.

