

- AppKit
- NSTextAlternatives
-  init(primaryString:alternativeStrings:) 

Initializer

# init(primaryString:alternativeStrings:)

Initializes an `NSTextAlternatives` instance.

macOS 10.8+

``` source
init(
    primaryString: String,
    alternativeStrings: [String]
)
```

## Parameters 

`primaryString`  

The string that is initially chosen as the input string.

`alternativeStrings`  

An array of alternative possible interpretations that the user might select.

## Return Value

An initialized `NSTextAlternatives` instance.

