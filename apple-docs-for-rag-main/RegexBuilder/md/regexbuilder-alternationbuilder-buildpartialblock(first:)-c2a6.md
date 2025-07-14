

- RegexBuilder
- AlternationBuilder
-  buildPartialBlock(first:) 

Type Method

# buildPartialBlock(first:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
static func buildPartialBlock(first regex: R) -> ChoiceOf where R : RegexComponent, R.RegexOutput == (W, C1, C2, C3)
```

