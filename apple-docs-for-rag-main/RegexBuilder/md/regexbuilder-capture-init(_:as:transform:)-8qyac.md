

- RegexBuilder
- Capture
-  init(\_:as:transform:) 

Initializer

# init(\_:as:transform:)

Creates a capture for the given component using the specified reference, transforming with the given closure.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(
    _ component: some RegexComponent,
    as reference: Reference,
    transform: @escaping (W) throws -> NewCapture
) where Output == (Substring, NewCapture, C1, C2)
```

## Parameters 

`component`  

The regex component to capture.

`reference`  

The reference to use for anything captured by `component`.

`transform`  

A closure that takes the substring matched by `component` and returns a new value to capture. If `transform` throws an error, matching is abandoned and the error is returned to the caller.

