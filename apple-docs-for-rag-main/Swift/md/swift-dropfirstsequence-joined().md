

- Swift
- DropFirstSequence
-  joined() 

Instance Method

# joined()

Returns the elements of this sequence of sequences, concatenated.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func joined() -> FlattenSequence
```

Available when `Element` conforms to `Sequence`.

## Return Value

A flattened view of the elements of this sequence of sequences.

## Discussion

In this example, an array of three ranges is flattened so that the elements of each range can be iterated in turn.

```
let ranges = [0..

