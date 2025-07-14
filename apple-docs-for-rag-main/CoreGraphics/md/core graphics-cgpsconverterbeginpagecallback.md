

- Core Graphics
-  CGPSConverterBeginPageCallback 

Type Alias

# CGPSConverterBeginPageCallback

Performs custom tasks at the beginning of each page in a PostScript conversion process.

Mac CatalystmacOS

``` source
typealias CGPSConverterBeginPageCallback = (UnsafeMutableRawPointer?, Int, CFDictionary) -> Void
```

## Parameters 

`info`  

A generic pointer to private data shared among your callback functions. This is the same pointer you supplied to init(info:callbacks:options:).

`pageNumber`  

The current page number. Page numbers start at `1`.

`pageInfo`  

A dictionary that contains contextual information about the page. This parameter is reserved for future API expansion, and is currently unused.

