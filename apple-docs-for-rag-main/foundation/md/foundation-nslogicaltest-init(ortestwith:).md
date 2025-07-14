

- Foundation
- NSLogicalTest
-  init(orTestWith:) 

Initializer

# init(orTestWith:)

Returns an `NSLogicalTest` object initialized to perform an `OR` operation with the `NSSpecifierTest` objects in a given array.

Mac Catalyst 13.0+macOS 10.0+

``` source
init(orTestWith subTests: [NSSpecifierTest])
```

## Parameters 

`subTests`  

An array of `NSSpecifierTest` objects representing Boolean expressions.

## Return Value

An `NSLogicalTest` object initialized to perform an `OR` operation with the `NSSpecifierTest` objects in `subTests`.

## See Also

### Initializing a logical test

init(andTestWith: [NSSpecifierTest])

Returns an `NSLogicalTest` object initialized to perform an `AND` operation with the `NSSpecifierTest` objects in a given array.

init(notTestWith: NSScriptWhoseTest)

Returns an `NSLogicalTest` object initialized to perform a `NOT` operation on the given `NSScriptWhoseTest` object.

