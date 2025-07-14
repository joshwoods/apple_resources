

- Swift
- AnyRegexOutput
- AnyRegexOutput.Element
-  range 

Instance Property

# range

The range over which a value was captured, if there was a capture.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var range: Range? { get }
```

## Discussion

If nothing was captured, `range` is `nil`.

