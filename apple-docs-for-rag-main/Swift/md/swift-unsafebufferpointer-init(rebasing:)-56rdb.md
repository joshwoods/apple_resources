

- Swift
- UnsafeBufferPointer
-  init(rebasing:) 

Initializer

# init(rebasing:)

Creates a buffer over the same memory as the given buffer slice.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(rebasing slice: Slice>)
```

## Parameters 

`slice`  

The buffer slice to rebase.

## Discussion

The new buffer represents the same region of memory as `slice`, but is indexed starting at zero instead of sharing indices with the original buffer. For example:

```
let buffer = returnsABuffer()
let n = 5
let slice = buffer[n...]
let rebased = UnsafeBufferPointer(rebasing: slice)
```

After rebasing `slice` as the `rebased` buffer, the following are true:

- `rebased.startIndex == 0`

- `rebased[0] == slice[n]`

- `rebased[0] == buffer[n]`

- `rebased.count == slice.count`

