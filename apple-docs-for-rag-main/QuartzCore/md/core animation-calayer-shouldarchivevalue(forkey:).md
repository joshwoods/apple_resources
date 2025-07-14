

- Core Animation
- CALayer
-  shouldArchiveValue(forKey:) 

Instance Method

# shouldArchiveValue(forKey:)

Returns a Boolean indicating whether the value of the specified key should be archived.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func shouldArchiveValue(forKey key: String) -> Bool
```

## Parameters 

`key`  

The name of one of the receiver’s properties.

## Return Value

true if the specified property should be archived or false if it should not.

## Discussion

The default implementation returns true.

## See Also

### Key-Value Coding Extensions

class func defaultValue(forKey: String) -> Any?

Specifies the default value associated with the specified key.

