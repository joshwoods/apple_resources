

- Foundation
- NSAttributedString
- NSAttributedString.EnumerationOptions
-  init(rawValue:) 

Initializer

# init(rawValue:)

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(rawValue: UInt)
```

## See Also

### Creating an enumeration option

static var reverse: NSAttributedString.EnumerationOptions

Causes the enumeration to occur in reverse.

static var longestEffectiveRangeNotRequired: NSAttributedString.EnumerationOptions

If `NSAttributedStringEnumerationLongestEffectiveRangeNotRequired` option is supplied, then the longest effective range computation is not performed; the blocks may be invoked with consecutive attribute runs that have the same value.

