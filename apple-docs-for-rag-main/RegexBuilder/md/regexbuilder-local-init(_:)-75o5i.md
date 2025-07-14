

- RegexBuilder
- Local
-  init(\_:) 

Initializer

# init(\_:)

Creates an atomic group with the given regex component.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(@RegexComponentBuilder _ componentBuilder: () -> some RegexComponent) where Output == Substring
```

## Parameters 

`componentBuilder`  

A builder closure that generates a regex component to wrap in an atomic group.

