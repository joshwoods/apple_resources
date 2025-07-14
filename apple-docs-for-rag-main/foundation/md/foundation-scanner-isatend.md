

- Foundation
- Scanner
-  isAtEnd 

Instance Property

# isAtEnd

Flag that indicates whether the receiver has exhausted all significant characters.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isAtEnd: Bool { get }
```

## Discussion

true if the receiver has exhausted all significant characters in its string, otherwise false.

If only characters from the set to be skipped remain, returns true.

## See Also

### Related Documentation

var charactersToBeSkipped: CharacterSet?

Character set containing the characters the scanner ignores when looking for a scannable element.

