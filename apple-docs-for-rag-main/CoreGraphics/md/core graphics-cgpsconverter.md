

- Core Graphics
-  CGPSConverter 

Class

# CGPSConverter

An opaque data type used to convert PostScript data to PDF data.

Mac CatalystmacOS

``` source
class CGPSConverter
```

## Overview

The PostScript data is supplied by a data provider and written into a data consumer. When you create a PostScript converter object, you can supply callback functions to invoke at various stages of the conversion process.

## Topics

### Initializers

init?(info: UnsafeMutableRawPointer?, callbacks: UnsafePointer&lt;CGPSConverterCallbacks>, options: CFDictionary?)

Creates a new PostScript converter.

### Instance Properties

var isConverting: Bool

Checks whether the converter is currently converting data.

### Type Properties

class var typeID: CFTypeID

Returns the Core Foundation type identifier for PostScript converters.

### Instance Methods

func abort() -> Bool

Tells a PostScript converter to abort a conversion at the next available opportunity.

func convert(CGDataProvider, consumer: CGDataConsumer, options: CFDictionary?) -> Bool

Uses a PostScript converter to convert PostScript data to PDF data.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

Quartz 2D Programming Guide

