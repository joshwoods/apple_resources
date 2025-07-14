

- RegexBuilder
- Capture
-  init(\_:) 

Initializer

# init(\_:)

Creates a capture for the given component.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(_ component: some RegexComponent) where Output == (Substring, W, C1, C2, C3, C4)
```

## Parameters 

`component`  

The regex component to capture.

