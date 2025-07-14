

- Swift
- Regex
-  dotMatchesNewlines(\_:) 

Instance Method

# dotMatchesNewlines(\_:)

Returns a regular expression where the “any” metacharacter (`.`) also matches against the start and end of a line.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func dotMatchesNewlines(_ dotMatchesNewlines: Bool = true) -> Regex.RegexOutput>
```

## Parameters 

`dotMatchesNewlines`  

A Boolean value indicating whether `.` should match a newline character.

## Return Value

The modified regular expression.

