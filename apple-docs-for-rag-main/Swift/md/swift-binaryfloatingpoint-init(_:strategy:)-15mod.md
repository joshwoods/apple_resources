

- Swift
- BinaryFloatingPoint
-  init(\_:strategy:) 

Initializer

# init(\_:strategy:)

Initialize an instance by parsing `value` with the given `strategy`.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    _ value: S.ParseInput,
    strategy: S
) throws where Self == S.ParseOutput, S : ParseStrategy
```

