

- Combine
- Just
-  setFailureType(to:) 

Instance Method

# setFailureType(to:)

Changes the failure type declared by the upstream publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func setFailureType(to failureType: E.Type) -> Publishers.SetFailureType where E : Error
```

Available when `Failure` is `Never`.

## Parameters 

`failureType`  

The `Failure` type presented by this publisher.

## Return Value

A publisher that appears to send the specified failure type.

## Discussion

Use setFailureType(to:) when you need set the error type of a publisher that cannot fail.

Conversely, if the upstream can fail, you would use mapError(_:) to provide instructions on converting the error types to needed by the downstream publisher’s inputs.

The following example has two publishers with mismatched error types: `pub1`’s error type is Never, and `pub2`’s error type is Error. Because of the mismatch, the combineLatest(_:) operator requires that `pub1` use setFailureType(to:) to make it appear that `pub1` can produce the Error type, like `pub2` can.

```
let pub1 = [0, 1, 2, 3, 4, 5].publisher
let pub2 = CurrentValueSubject(0)
let cancellable = pub1
    .setFailureType(to: Error.self)
    .combineLatest(pub2)
    .sink(
        receiveCompletion: { print ("completed: \($0)") },
        receiveValue: { print ("value: \($0)")}
     )

// Prints: "value: (5, 0)".
```

