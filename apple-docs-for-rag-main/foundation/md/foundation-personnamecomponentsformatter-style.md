

- Foundation
- PersonNameComponentsFormatter
-  style 

Instance Property

# style

The formatting style of the receiver.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var style: PersonNameComponentsFormatter.Style { get set }
```

## Discussion

Styles specify which name components are used to create a string representation, and how. Examples of name components formatter styles include `long` and `abbreviated`.

## See Also

### Configuring Formatter Behavior

var isPhonetic: Bool

A Boolean value that specifies whether the receiver should use only the phonetic representations of name components. false by default.

