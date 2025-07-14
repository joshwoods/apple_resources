

- RegexBuilder
- Repeat
-  init(count:\_:) 

Initializer

# init(count:\_:)

Creates a regex component that matches the given component repeated the specified number of times.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(
    count: Int,
    @RegexComponentBuilder _ componentBuilder: () -> some RegexComponent
) where Output == (Substring, C1?, C2?, C3?, C4?, C5?, C6?, C7?, C8?, C9?)
```

## Parameters 

`count`  

The number of times to repeat `component`. `count` must be greater than or equal to zero.

`componentBuilder`  

A builder closure that creates the regex component to repeat.

