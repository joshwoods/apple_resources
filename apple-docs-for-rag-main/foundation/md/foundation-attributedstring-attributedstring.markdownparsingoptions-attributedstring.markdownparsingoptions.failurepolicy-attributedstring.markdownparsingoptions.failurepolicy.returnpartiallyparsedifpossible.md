

- Foundation
- AttributedString
- AttributedString.MarkdownParsingOptions
- AttributedString.MarkdownParsingOptions.FailurePolicy
-  AttributedString.MarkdownParsingOptions.FailurePolicy.returnPartiallyParsedIfPossible 

Case

# AttributedString.MarkdownParsingOptions.FailurePolicy.returnPartiallyParsedIfPossible

A policy to return a partially-parsed string, if possible.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case returnPartiallyParsedIfPossible
```

## Discussion

With this policy, the returned string may include unparsed markup. If returning a partially parsed string isn’t possible, the parser may throw an error anyway.

## See Also

### Declaring Failure Policies

case throwError

A policy to throw an error from the initializer if parsing fails.

