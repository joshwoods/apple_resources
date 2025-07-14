

- Core Animation
- CAAnimation
-  shouldArchiveValue(forKey:) 

Instance Method

# shouldArchiveValue(forKey:)

Specifies whether the value of the property for a given key is archived.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func shouldArchiveValue(forKey key: String) -> Bool
```

## Parameters 

`key`  

The name of one of the receiver’s properties.

## Return Value

true if the specified property should be archived, otherwise false.

## Discussion

Called by the object’s implementation of `encodeWithCoder:`. The object must implement keyed archiving.

The default implementation returns true.

## See Also

### Related Documentation

Core Animation Programming Guide

