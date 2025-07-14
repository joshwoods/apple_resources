

- RealityKit
- UnsafeForceEffectBuffer
-  joined() 

Instance Method

# joined()

Returns the elements of this sequence of sequences, concatenated.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

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

