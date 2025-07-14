

- Dispatch
- DispatchPredicate
-  DispatchPredicate.onQueue(\_:) 

Case

# DispatchPredicate.onQueue(\_:)

A predicate that indicates the evaluated context is the associated dispatch queue.

iOS 10.0+iPadOS 10.0+Mac CatalystmacOS 10.12+tvOS 10.0+visionOSwatchOS 3.0+

``` source
case onQueue(DispatchQueue)
```

## See Also

### Predicates

case onQueueAsBarrier(DispatchQueue)

A predicate that indicates the evaluated context is the associated dispatch queue as part of a barrier operation.

case notOnQueue(DispatchQueue)

A predicate that indicates the evaluated context is not the associated dispatch queue.

