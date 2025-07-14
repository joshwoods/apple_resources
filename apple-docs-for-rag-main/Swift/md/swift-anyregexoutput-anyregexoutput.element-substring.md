

- Swift
- AnyRegexOutput
- AnyRegexOutput.Element
-  substring 

Instance Property

# substring

The slice of the input which was captured, if there was a capture.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var substring: Substring? { get }
```

## Discussion

If nothing was captured, `substring` is `nil`.

