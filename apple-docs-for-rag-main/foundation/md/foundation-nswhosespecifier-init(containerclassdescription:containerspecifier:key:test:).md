

- Foundation
- NSWhoseSpecifier
-  init(containerClassDescription:containerSpecifier:key:test:) 

Initializer

# init(containerClassDescription:containerSpecifier:key:test:)

Returns an `NSWhoseSpecifier` object initialized with the given attributes.

Mac Catalyst 13.0+macOS 10.0+

``` source
init(
    containerClassDescription classDesc: NSScriptClassDescription,
    containerSpecifier container: NSScriptObjectSpecifier?,
    key property: String,
    test: NSScriptWhoseTest
)
```

## Parameters 

`classDesc`  

Class description for the receiver’s container object.

`container`  

An object specifier for the receiver’s container object.

`property`  

The key for the property for which to test.

`test`  

The test condition.

## Return Value

An `NSWhoseSpecifier` object initialized with the given attributes.

## Discussion

Invokes the super class’s init(containerClassDescription:containerSpecifier:key:) and sets the whose test condition to `test`.

## See Also

### Related Documentation

Cocoa Scripting Guide

