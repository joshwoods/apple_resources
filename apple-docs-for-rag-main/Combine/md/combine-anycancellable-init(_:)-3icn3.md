

- Combine
- AnyCancellable
-  init(\_:) 

Initializer

# init(\_:)

Initializes the cancellable object with the given cancel-time closure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(_ cancel: @escaping () -> Void)
```

## Parameters 

`cancel`  

A closure that the `cancel()` method executes.

