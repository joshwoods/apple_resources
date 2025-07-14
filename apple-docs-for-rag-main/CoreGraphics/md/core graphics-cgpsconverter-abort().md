

- Core Graphics
- CGPSConverter
-  abort() 

Instance Method

# abort()

Tells a PostScript converter to abort a conversion at the next available opportunity.

Mac Catalyst 13.1+macOS 10.3+

``` source
func abort() -> Bool
```

## Return Value

A Boolean value that indicates whether the converter is currently converting data (`true` if it is).

## See Also

### Instance Methods

func convert(CGDataProvider, consumer: CGDataConsumer, options: CFDictionary?) -> Bool

Uses a PostScript converter to convert PostScript data to PDF data.

