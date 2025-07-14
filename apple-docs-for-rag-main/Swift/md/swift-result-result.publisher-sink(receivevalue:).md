

- Swift
- Result
- Result.Publisher
-  sink(receiveValue:) 

Instance Method

# sink(receiveValue:)

Attaches a subscriber with closure-based behavior to a publisher that never fails.

SwiftCombineiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

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

Use sink(receiveValue:) to observe values received by the publisher and print them to the console. This operator can only be used when the stream doesn’t fail, that is, when the publisher’s `Publisher/Failure` type is Never.

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

