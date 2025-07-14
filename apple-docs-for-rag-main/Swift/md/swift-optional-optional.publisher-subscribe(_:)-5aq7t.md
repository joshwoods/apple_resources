

- Swift
- Optional
- Optional.Publisher
-  subscribe(\_:) 

Instance Method

# subscribe(\_:)

Attaches the specified subject to this publisher.

SwiftCombineiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func subscribe(_ subject: S) -> AnyCancellable where S : Subject, Self.Failure == S.Failure, Self.Output == S.Output
```

## Parameters 

`subject`  

The subject to attach to this publisher.

