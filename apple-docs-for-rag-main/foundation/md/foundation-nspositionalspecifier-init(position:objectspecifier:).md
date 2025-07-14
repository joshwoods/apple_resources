

- Foundation
- NSPositionalSpecifier
-  init(position:objectSpecifier:) 

Initializer

# init(position:objectSpecifier:)

Initializes a positional specifier with a given position relative to another given specifier.

Mac Catalyst 13.0+macOS 10.0+

``` source
init(
    position: NSPositionalSpecifier.InsertionPosition,
    objectSpecifier specifier: NSScriptObjectSpecifier
)
```

## Parameters 

`position`  

The position for the new specifier relative to `specifier`.

`specifier`  

The reference specifier.

## Return Value

An initialized positional specifier with the position specified by `position` relative to the object specified by `specifier`.

## See Also

### Related Documentation

Cocoa Scripting Guide

