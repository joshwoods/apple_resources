

- Foundation
- NSCharacterSet
-  inverted 

Instance Property

# inverted

A character set containing only characters that don’t exist in the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var inverted: CharacterSet { get }
```

## Discussion

Using the inverse of an immutable character set is much more efficient than inverting a mutable character set.

## See Also

### Related Documentation

func invert()

Replaces all the characters in the receiver with all the characters it didn’t previously contain.

