

- RegexBuilder
- Capture
-  init(\_:) 

Initializer

# init(\_:)

Creates a capture for the given component.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(@RegexComponentBuilder _ componentBuilder: () -> some RegexComponent) where Output == (Substring, W)
```

## Parameters 

`componentBuilder`  

A builder closure that generates a regex component to capture.

