

- Foundation
- NSLogicalTest
-  init(andTestWith:) 

Initializer

# init(andTestWith:)

Returns an `NSLogicalTest` object initialized to perform an `AND` operation with the `NSSpecifierTest` objects in a given array.

Mac Catalyst 13.0+macOS 10.0+

``` source
init(andTestWith subTests: [NSSpecifierTest])
```

## Parameters 

`subTests`  

An array of `NSSpecifierTest` objects representing Boolean expressions.

## Return Value

An `NSLogicalTest` object initialized to perform an `AND` operation with the `NSSpecifierTest` objects in `subTests`.

## See Also

### Related Documentation

Cocoa Scripting Guide

### Initializing a logical test

init(notTestWith: NSScriptWhoseTest)

Returns an `NSLogicalTest` object initialized to perform a `NOT` operation on the given `NSScriptWhoseTest` object.

init(orTestWith: [NSSpecifierTest])

Returns an `NSLogicalTest` object initialized to perform an `OR` operation with the `NSSpecifierTest` objects in a given array.

