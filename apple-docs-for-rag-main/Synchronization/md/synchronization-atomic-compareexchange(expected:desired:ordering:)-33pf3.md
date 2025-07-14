

- Synchronization
- Atomic
-  compareExchange(expected:desired:ordering:) 

Instance Method

# compareExchange(expected:desired:ordering:)

Perform an atomic compare and exchange operation on the current value, applying the specified memory ordering.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func compareExchange(
    expected: consuming Value,
    desired: consuming Value,
    ordering: AtomicUpdateOrdering
) -> (exchanged: Bool, original: Value)
```

Available when `Value` conforms to `AtomicRepresentable` and `Value.AtomicRepresentation` is `_Atomic128BitStorage`.

## Parameters 

`expected`  

The expected current value.

`desired`  

The desired new value.

`ordering`  

The memory ordering to apply on this operation.

## Return Value

A tuple `(exchanged, original)`, where `exchanged` is true if the exchange was successful, and `original` is the original value.

## Discussion

This operation performs the following algorithm as a single atomic transaction:

```
```

Note

This method implements a “strong” compare and exchange operation that does not permit spurious failures.

