

- RegexBuilder
- Capture
-  init(as:\_:) 

Initializer

# init(as:\_:)

Creates a capture for the given component using the specified reference.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(
    as reference: Reference,
    @RegexComponentBuilder _ componentBuilder: () -> some RegexComponent
) where Output == (Substring, W, C1, C2, C3)
```

## Parameters 

`reference`  

The reference to use for anything captured by `component`.

`componentBuilder`  

A builder closure that generates a regex component to capture.

