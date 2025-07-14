

- Core Animation
- CATransaction
-  setValue(\_:forKey:) 

Type Method

# setValue(\_:forKey:)

Sets the arbitrary keyed-data for the specified key.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
class func setValue(
    _ anObject: Any?,
    forKey key: String
)
```

## Parameters 

`anObject`  

The value for the key identified by `key`.

`key`  

The name of one of the receiver’s properties.

## Discussion

Nested transactions have nested data scope; setting a key always sets it in the innermost scope.

## See Also

### Getting and Setting Transaction Properties

class func value(forKey: String) -> Any?

Returns the arbitrary keyed-data specified by the given key.

