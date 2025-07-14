

- RegexBuilder
- Capture
-  init(\_:as:) 

Initializer

# init(\_:as:)

Creates a capture for the given component using the specified reference.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(
    _ component: some RegexComponent,
    as reference: Reference
) where Output == (Substring, W)
```

## Parameters 

`component`  

The regex component to capture.

`reference`  

The reference to use for anything captured by `component`.

