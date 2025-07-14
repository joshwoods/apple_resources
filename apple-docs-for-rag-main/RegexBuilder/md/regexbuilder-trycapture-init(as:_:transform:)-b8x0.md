

- RegexBuilder
- TryCapture
-  init(as:\_:transform:) 

Initializer

# init(as:\_:transform:)

Creates a capture for the given component using the specified reference, attempting to transform with the given closure.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(
    as reference: Reference,
    @RegexComponentBuilder _ componentBuilder: () -> some RegexComponent,
    transform: @escaping (W) throws -> NewCapture?
) where Output == (Substring, NewCapture, C1, C2, C3, C4, C5)
```

## Parameters 

`reference`  

The reference to use for anything captured by `component`.

`componentBuilder`  

A builder closure that generates a regex component to capture.

`transform`  

A closure that takes the substring matched by `component` and returns a new value to capture, or `nil` if matching should proceed, backtracking if allowed. If `transform` throws an error, matching is abandoned and the error is returned to the caller.

