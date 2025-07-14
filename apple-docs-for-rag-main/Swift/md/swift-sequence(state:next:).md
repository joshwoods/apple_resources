

- Swift
-  sequence(state:next:) 

Function

# sequence(state:next:)

Returns a sequence formed from repeated lazy applications of `next` to a mutable `state`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func sequence(
    state: State,
    next: @escaping (inout State) -> T?
) -> UnfoldSequence
```

## Parameters 

`state`  

The initial state that will be passed to the closure.

`next`  

A closure that accepts an `inout` state and returns the next element of the sequence.

## Return Value

A sequence that yields each successive value from `next`.

## Discussion

The elements of the sequence are obtained by invoking `next` with a mutable state. The same state is passed to all invocations of `next`, so subsequent calls will see any mutations made by previous calls. The sequence ends when `next` returns `nil`. If `next` never returns `nil`, the sequence is infinite.

This function can be used to replace many instances of `AnyIterator` that wrap a closure.

Example:

```
// Interleave two sequences that yield the same element type
sequence(state: (false, seq1.makeIterator(), seq2.makeIterator()), next: { iters in
  iters.0 = !iters.0
  return iters.0 ? iters.1.next() : iters.2.next()
})
```

## See Also

### Dynamic Sequences

func sequence&lt;T>(first: T, next: (T) -> T?) -> UnfoldFirstSequence&lt;T>

Returns a sequence formed from `first` and repeated lazy applications of `next`.

