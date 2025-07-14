

- MusicKit
- MusicItemCollection
-  joined() 

Instance Method

# joined()

Returns the elements of this sequence of sequences, concatenated.

MusicKitSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

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

