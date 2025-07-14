

- RealityKit
- LoadRequest
-  subscribe(\_:) 

Instance Method

# subscribe(\_:)

Attaches the specified subject to this publisher.

RealityKitCombineiOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
func subscribe(_ subject: S) -> AnyCancellable where S : Subject, Self.Failure == S.Failure, Self.Output == S.Output
```

## Parameters 

`subject`  

The subject to attach to this publisher.

## See Also

### Working with subscribers

func receive&lt;S>(subscriber: S)

Attaches the specified subscriber to this publisher.

Deprecated

func subscribe&lt;S>(S)

Attaches the specified subscriber to this publisher.

Deprecated

func subscribe&lt;S>(S)

Attaches the specified subscriber to this publisher.

