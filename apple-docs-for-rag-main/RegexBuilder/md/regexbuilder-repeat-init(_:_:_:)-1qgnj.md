

- RegexBuilder
- Repeat
-  init(\_:\_:\_:) 

Initializer

# init(\_:\_:\_:)

Creates a regex component that matches the given component repeated a number of times specified by the given range expression.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(
    _ expression: some RangeExpression,
    _ behavior: RegexRepetitionBehavior? = nil,
    @RegexComponentBuilder _ componentBuilder: () -> some RegexComponent
) where Output == (Substring, C1?, C2?, C3?, C4?, C5?)
```

## Parameters 

`expression`  

A range expression specifying the number of times that `component` can repeat.

`behavior`  

The repetition behavior to use when repeating `component` in the match. If `behavior` is `nil`, the default repetition behavior is used, which can be changed from `eager` by calling `repetitionBehavior(_:)` on the resulting `Regex`.

`componentBuilder`  

A builder closure that creates the regex component to repeat.

