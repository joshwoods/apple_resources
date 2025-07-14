

- Swift
- AnyRegexOutput
-  AnyRegexOutput.Element 

Structure

# AnyRegexOutput.Element

An individual match output value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Element
```

## Topics

### Instance Properties

var name: String?

The name of this capture, if the capture is named.

var range: Range&lt;String.Index>?

The range over which a value was captured, if there was a capture.

var substring: Substring?

The slice of the input which was captured, if there was a capture.

var type: any Any.Type

The type of this capture.

var value: Any?

The captured value, if there was a capture.

