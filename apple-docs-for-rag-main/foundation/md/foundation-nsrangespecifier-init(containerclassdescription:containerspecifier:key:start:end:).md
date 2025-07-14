

- Foundation
- NSRangeSpecifier
-  init(containerClassDescription:containerSpecifier:key:start:end:) 

Initializer

# init(containerClassDescription:containerSpecifier:key:start:end:)

Returns a range specifier initialized with the given properties.

Mac Catalyst 13.0+macOS 10.0+

``` source
init(
    containerClassDescription classDesc: NSScriptClassDescription,
    containerSpecifier container: NSScriptObjectSpecifier?,
    key property: String,
    start startSpec: NSScriptObjectSpecifier?,
    end endSpec: NSScriptObjectSpecifier?
)
```

## Parameters 

`classDesc`  

The class description.

`container`  

The container.

`property`  

The property.

`startSpec`  

The object specifier representing the first object of the range.

`endSpec`  

The object specifier representing the last object of the range.

## Return Value

A range specifier initialized with the given properties.

## Discussion

Invokes the super class’s init(containerClassDescription:containerSpecifier:key:) method and initializes the instance with the object specifiers representing the starting element, `startSpec`, and the ending element, `endSpec`, of a range of elements in the container.

## See Also

### Related Documentation

Cocoa Scripting Guide

