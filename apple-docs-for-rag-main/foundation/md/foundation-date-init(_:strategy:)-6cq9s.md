

- Foundation
- Date
-  init(\_:strategy:) 

Initializer

# init(\_:strategy:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    _ value: Value,
    strategy: T
) throws where T : ParseStrategy, Value : StringProtocol, T.ParseInput == String, T.ParseOutput == Date
```

