

- Foundation
- NSUniqueIDSpecifier
-  init(containerClassDescription:containerSpecifier:key:uniqueID:) 

Initializer

# init(containerClassDescription:containerSpecifier:key:uniqueID:)

Returns an `NSUniqueIDSpecifier` object, initialized with the given arguments.

Mac Catalyst 13.0+macOS 10.0+

``` source
init(
    containerClassDescription classDesc: NSScriptClassDescription,
    containerSpecifier container: NSScriptObjectSpecifier?,
    key property: String,
    uniqueID: Any
)
```

## Parameters 

`classDesc`  

The class description for the new object.

`container`  

The container for the new object.

`property`  

The property for the new object.

`uniqueID`  

The unique ID for the new object.

`uniqueID` must be an instance of `NSNumber` or `NSString`. The type should match the declared type of the attribute of the specified scriptable class whose four-character code is `'ID '`.

## Return Value

An `NSUniqueIDSpecifier` object, initialized with the given arguments.

## Discussion

Invokes the super class’s init(containerClassDescription:containerSpecifier:key:) method and sets the ID to `uniqueID`.

## See Also

### Related Documentation

Cocoa Scripting Guide

