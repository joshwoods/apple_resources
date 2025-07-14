

- Swift
- Dictionary
-  compactMapValues(\_:) 

Instance Method

# compactMapValues(\_:)

Returns a new dictionary containing only the key-value pairs that have non-`nil` values as the result of transformation by the given closure.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func compactMapValues(_ transform: (Value) throws -> T?) rethrows -> Dictionary
```

Available when `Key` conforms to `Hashable`.

## Parameters 

`transform`  

A closure that transforms a value. `transform` accepts each value of the dictionary as its parameter and returns an optional transformed value of the same or of a different type.

## Return Value

A dictionary containing the keys and non-`nil` transformed values of this dictionary.

## Discussion

Use this method to receive a dictionary with non-optional values when your transformation produces optional values.

In this example, note the difference in the result of using `mapValues` and `compactMapValues` with a transformation that returns an optional `Int` value.

```
let data = ["a": "1", "b": "three", "c": "///4///"]

let m: [String: Int?] = data.mapValues { str in Int(str) }
// ["a": Optional(1), "b": nil, "c": nil]

let c: [String: Int] = data.compactMapValues { str in Int(str) }
// ["a": 1]
```

Complexity

O(*m* + *n*), where *n* is the length of the original dictionary and *m* is the length of the resulting dictionary.

## See Also

### Transforming a Dictionary

func mapValues&lt;T>((Value) throws -> T) rethrows -> Dictionary&lt;Key, T>

Returns a new dictionary containing the keys of this dictionary with the values transformed by the given closure.

func reduce&lt;Result>(Result, (Result, Self.Element) throws -> Result) rethrows -> Result

Returns the result of combining the elements of the sequence using the given closure.

func reduce&lt;Result>(into: Result, (inout Result, Self.Element) throws -> ()) rethrows -> Result

Returns the result of combining the elements of the sequence using the given closure.

func compactMap&lt;ElementOfResult>((Self.Element) throws -> ElementOfResult?) rethrows -> [ElementOfResult]

Returns an array containing the non-`nil` results of calling the given transformation with each element of this sequence.

func flatMap&lt;SegmentOfResult>((Self.Element) throws -> SegmentOfResult) rethrows -> [SegmentOfResult.Element]

Returns an array containing the concatenated results of calling the given transformation with each element of this sequence.

func flatMap&lt;ElementOfResult>((Self.Element) throws -> ElementOfResult?) rethrows -> [ElementOfResult]

func sorted(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> [Self.Element]

Returns the elements of the sequence, sorted using the given predicate as the comparison between elements.

func shuffled() -> [Self.Element]

Returns the elements of the sequence, shuffled.

func shuffled&lt;T>(using: inout T) -> [Self.Element]

Returns the elements of the sequence, shuffled using the given generator as a source for randomness.

