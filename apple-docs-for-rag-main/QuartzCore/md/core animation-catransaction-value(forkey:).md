

- Core Animation
- CATransaction
-  value(forKey:) 

Type Method

# value(forKey:)

Returns the arbitrary keyed-data specified by the given key.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
class func value(forKey key: String) -> Any?
```

## Parameters 

`key`  

The name of one of the receiver’s properties.

## Return Value

The value for the data specified by the key.

## Discussion

Nested transactions have nested data scope. Requesting a value for a key first searches the innermost scope, then the enclosing transactions.

## See Also

### Getting and Setting Transaction Properties

class func setValue(Any?, forKey: String)

Sets the arbitrary keyed-data for the specified key.

