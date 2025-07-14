

- Foundation
- NSMutableCharacterSet
-  invert() 

Instance Method

# invert()

Replaces all the characters in the receiver with all the characters it didn’t previously contain.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func invert()
```

## Discussion

Inverting a mutable character set, whether by invert() or by inverted, is much less efficient than inverting an immutable character set with inverted.

## See Also

### Related Documentation

var inverted: CharacterSet

A character set containing only characters that don’t exist in the receiver.

