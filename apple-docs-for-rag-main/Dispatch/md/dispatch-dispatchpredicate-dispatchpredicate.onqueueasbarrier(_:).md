

- Dispatch
- DispatchPredicate
-  DispatchPredicate.onQueueAsBarrier(\_:) 

Case

# DispatchPredicate.onQueueAsBarrier(\_:)

A predicate that indicates the evaluated context is the associated dispatch queue as part of a barrier operation.

iOS 10.0+iPadOS 10.0+Mac CatalystmacOS 10.12+tvOS 10.0+visionOSwatchOS 3.0+

``` source
case onQueueAsBarrier(DispatchQueue)
```

## Discussion

For more information about barrier operations, see \`barrier\`.

## See Also

### Predicates

case onQueue(DispatchQueue)

A predicate that indicates the evaluated context is the associated dispatch queue.

case notOnQueue(DispatchQueue)

A predicate that indicates the evaluated context is not the associated dispatch queue.

