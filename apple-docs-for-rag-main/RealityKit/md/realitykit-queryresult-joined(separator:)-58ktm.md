

- RealityKit
- QueryResult
-  joined(separator:) 

Instance Method

# joined(separator:)

Returns a new string by concatenating the elements of the sequence, adding the given separator between each element.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
func joined(separator: String = "") -> String
```

Available when `Element` conforms to `StringProtocol`.

## Parameters 

`separator`  

A string to insert between each of the elements in this sequence. The default separator is an empty string.

## Return Value

A single, concatenated string.

## Discussion

The following example shows how an array of strings can be joined to a single, comma-separated string:

```
let cast = ["Vivien", "Marlon", "Kim", "Karl"]
let list = cast.joined(separator: ", ")
print(list)
// Prints "Vivien, Marlon, Kim, Karl"
```

## See Also

### Splitting and joining elements

func split(maxSplits: Int, omittingEmptySubsequences: Bool, whereSeparator: (Self.Element) throws -> Bool) rethrows -> [ArraySlice&lt;Self.Element>]

Returns the longest possible subsequences of the sequence, in order, that don’t contain elements satisfying the given predicate. Elements that are used to split the sequence are not returned as part of any subsequence.

func split(separator: Self.Element, maxSplits: Int, omittingEmptySubsequences: Bool) -> [ArraySlice&lt;Self.Element>]

Returns the longest possible subsequences of the sequence, in order, around elements equal to the given element.

func joined() -> FlattenSequence&lt;Self>

Returns the elements of this sequence of sequences, concatenated.

func joined&lt;Separator>(separator: Separator) -> JoinedSequence&lt;Self>

Returns the concatenated elements of this sequence of sequences, inserting the given separator between each element.

