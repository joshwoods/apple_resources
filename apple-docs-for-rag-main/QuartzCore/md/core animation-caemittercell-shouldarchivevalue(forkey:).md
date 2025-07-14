

- Core Animation
- CAEmitterCell
-  shouldArchiveValue(forKey:) 

Instance Method

# shouldArchiveValue(forKey:)

Returns a Boolean value indicating whether the value for a given key should be archived.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
func shouldArchiveValue(forKey key: String) -> Bool
```

## Parameters 

`key`  

The name of one of the receiver’s properties.

## Return Value

true if the specified property should be archived, otherwise false.

## Discussion

The default implementation returns true. This method is called by the object’s implementation of `encodeWithCoder:`.

## See Also

### Using Key-Value Coding Extensions

class func defaultValue(forKey: String) -> Any?

Returns the default value of the property with the specified key.

