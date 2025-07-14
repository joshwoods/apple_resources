

- Swift
- Regex
-  asciiOnlyCharacterClasses(\_:) 

Instance Method

# asciiOnlyCharacterClasses(\_:)

Returns a regular expression that matches only ASCII characters when matching character classes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func asciiOnlyCharacterClasses(_ useASCII: Bool = true) -> Regex.RegexOutput>
```

## Parameters 

`useASCII`  

A Boolean value indicating whether to match only ASCII characters when matching character classes.

## Return Value

The modified regular expression.

