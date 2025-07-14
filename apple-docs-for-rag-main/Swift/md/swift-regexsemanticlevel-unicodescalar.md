

- Swift
- RegexSemanticLevel
-  unicodeScalar 

Type Property

# unicodeScalar

Match at the Unicode scalar level.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var unicodeScalar: RegexSemanticLevel { get }
```

## Discussion

At this semantic level, the string’s `UnicodeScalarView` is used for matching, and each matched element is a `UnicodeScalar` value.

