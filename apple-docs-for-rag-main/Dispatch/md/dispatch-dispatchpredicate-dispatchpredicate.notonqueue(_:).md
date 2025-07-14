

- Dispatch
- DispatchPredicate
-  DispatchPredicate.notOnQueue(\_:) 

Case

# DispatchPredicate.notOnQueue(\_:)

A predicate that indicates the evaluated context is not the associated dispatch queue.

iOS 10.0+iPadOS 10.0+Mac CatalystmacOS 10.12+tvOS 10.0+visionOSwatchOS 3.0+

``` source
case notOnQueue(DispatchQueue)
```

## See Also

### Predicates

case onQueue(DispatchQueue)

A predicate that indicates the evaluated context is the associated dispatch queue.

case onQueueAsBarrier(DispatchQueue)

A predicate that indicates the evaluated context is the associated dispatch queue as part of a barrier operation.

