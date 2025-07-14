

- Combine
- Publishers
- Publishers.CombineLatest4
-  sink(receiveCompletion:receiveValue:) 

Instance Method

# sink(receiveCompletion:receiveValue:)

Attaches a subscriber with closure-based behavior.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func sink(
    receiveCompletion: @escaping (Subscribers.Completion) -> Void,
    receiveValue: @escaping (Self.Output) -> Void
) -> AnyCancellable
```

## Parameters 

`receiveValue`  

The closure to execute on receipt of a value.

## Return Value

A cancellable instance, which you use when you end assignment of the received value. Deallocation of the result will tear down the subscription stream.

## Discussion

Use sink(receiveCompletion:receiveValue:) to observe values received by the publisher and process them using a closure you specify.

In this example, a Range publisher publishes integers to a sink(receiveCompletion:receiveValue:) operator’s `receiveValue` closure that prints them to the console. Upon completion the sink(receiveCompletion:receiveValue:) operator’s `receiveCompletion` closure indicates the successful termination of the stream.

```
let myRange = (0...3)
cancellable = myRange.publisher
    .sink(receiveCompletion: { print ("completion: \($0)") },
          receiveValue: { print ("value: \($0)") })

// Prints:
//  value: 0
//  value: 1
//  value: 2
//  value: 3
//  completion: finished
```

This method creates the subscriber and immediately requests an unlimited number of values, prior to returning the subscriber. The return value should be held, otherwise the stream will be canceled.

## See Also

### Connecting Simple Subscribers

func assign&lt;Root>(to: ReferenceWritableKeyPath&lt;Root, Self.Output>, on: Root) -> AnyCancellable

Assigns each element from a publisher to a property on an object.

func assign(to: inout Published&lt;Self.Output>.Publisher)

Republishes elements received from a publisher, by assigning them to a property marked as a publisher.

func sink(receiveValue: (Self.Output) -> Void) -> AnyCancellable

Attaches a subscriber with closure-based behavior to a publisher that never fails.

