

- Foundation
- NSLogicalTest
-  init(notTestWith:) 

Initializer

# init(notTestWith:)

Returns an `NSLogicalTest` object initialized to perform a `NOT` operation on the given `NSScriptWhoseTest` object.

Mac Catalyst 13.0+macOS 10.0+

``` source
init(notTestWith subTest: NSScriptWhoseTest)
```

## Parameters 

`subTest`  

The `NSScriptWhoseTest` object to invert.

## Return Value

An `NSLogicalTest` object initialized to perform a `NOT` operation on `subTest`.

## See Also

### Initializing a logical test

init(andTestWith: [NSSpecifierTest])

Returns an `NSLogicalTest` object initialized to perform an `AND` operation with the `NSSpecifierTest` objects in a given array.

init(orTestWith: [NSSpecifierTest])

Returns an `NSLogicalTest` object initialized to perform an `OR` operation with the `NSSpecifierTest` objects in a given array.

