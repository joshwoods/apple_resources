

- RegexBuilder
- Repeat
-  init(\_:count:) 

Initializer

# init(\_:count:)

Creates a regex component that matches the given component repeated the specified number of times.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(
    _ component: some RegexComponent,
    count: Int
) where Output == (Substring, C1?, C2?, C3?, C4?, C5?, C6?)
```

## Parameters 

`component`  

The regex component to repeat.

`count`  

The number of times to repeat `component`. `count` must be greater than or equal to zero.

