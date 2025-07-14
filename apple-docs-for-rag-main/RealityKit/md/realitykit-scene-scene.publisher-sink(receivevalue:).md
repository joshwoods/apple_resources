

- RealityKit
- Scene
- Scene.Publisher
-  sink(receiveValue:) 

Instance Method

# sink(receiveValue:)

Attaches a subscriber with closure-based behavior to a publisher that never fails.

RealityKitCombineiOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
func sink(receiveValue: @escaping (Self.Output) -> Void) -> AnyCancellable
```

Available when `Failure` is `Never`.

## Parameters 

`receiveValue`  

The closure to execute on receipt of a value.

## Return Value

A cancellable instance, which you use when you end assignment of the received value. Deallocation of the result will tear down the subscription stream.

## Discussion

Use sink(receiveValue:) to observe values received by the publisher and print them to the console. This operator can only be used when the stream doesn’t fail, that is, when the publisher’s Scene.Publisher.Failure type is Never.

In this example, a Range publisher publishes integers to a sink(receiveValue:) operator’s `receiveValue` closure that prints them to the console:

```
let integers = (0...3)
integers.publisher
    .sink { print("Received \($0)") }

// Prints:
//  Received 0
//  Received 1
//  Received 2
//  Received 3
```

This method creates the subscriber and immediately requests an unlimited number of values, prior to returning the subscriber. The return value should be held, otherwise the stream will be canceled.

## See Also

### Connecting simple subscribers

func assign&lt;Root>(to: ReferenceWritableKeyPath&lt;Root, Self.Output>, on: Root) -> AnyCancellable

Assigns each element from a publisher to a property on an object.

func sink(receiveCompletion: (Subscribers.Completion&lt;Self.Failure>) -> Void, receiveValue: (Self.Output) -> Void) -> AnyCancellable

Attaches a subscriber with closure-based behavior.

