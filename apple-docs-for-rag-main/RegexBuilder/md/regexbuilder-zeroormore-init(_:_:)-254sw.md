

- RegexBuilder
- ZeroOrMore
-  init(\_:\_:) 

Initializer

# init(\_:\_:)

Creates a regex component that matches the given component zero or more times.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(
    _ component: some RegexComponent,
    _ behavior: RegexRepetitionBehavior? = nil
) where Output == (Substring, C1?, C2?, C3?, C4?)
```

## Parameters 

`component`  

The regex component.

`behavior`  

The repetition behavior to use when repeating `component` in the match. If `behavior` is `nil`, the default repetition behavior is used, which can be changed from `eager` by calling `repetitionBehavior(_:)` on the resulting `Regex`.

