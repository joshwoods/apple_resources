

- Foundation
- AttributedStringProtocol
-  index(beforeRun:) 

Instance Method

# index(beforeRun:)

Returns the position of the run immediately before a run indicated by an index.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func index(beforeRun i: AttributedString.Index) -> AttributedString.Index
```

## Parameters 

`i`  

The index of a run in the attributed string.

## Return Value

The position of the first run immediately before the beginning of the `i`-th run.

## See Also

### Accessing Indices

var startIndex: AttributedString.Index

The position of the first character in a nonempty attributed string.

**Required**

var endIndex: AttributedString.Index

A string’s past-the-end position — the position one greater than the last valid subscript argument.

**Required**

func index(AttributedString.Index, offsetByCharacters: Int) -> AttributedString.Index

Returns the position of the character offset a given distance, measured in characters, from a given string index.

func index(AttributedString.Index, offsetByRuns: Int) -> AttributedString.Index

Returns the position of the run offset a given number of runs from a given string index.

func index(AttributedString.Index, offsetByUnicodeScalars: Int) -> AttributedString.Index

Returns the position of the Unicode scalar offset a given distance, measured in Unicode scalars, from a given string index.

func index(afterCharacter: AttributedString.Index) -> AttributedString.Index

Returns the position of the character immediately after another charcter indicated by an index.

func index(afterRun: AttributedString.Index) -> AttributedString.Index

Returns the position of the run immediately after a run indicated by an index.

func index(afterUnicodeScalar: AttributedString.Index) -> AttributedString.Index

Returns the position of the Unicode scalar immediately after a Unicode scalar indicated by an index.

func index(beforeCharacter: AttributedString.Index) -> AttributedString.Index

Returns the position of the character immediately before another charcter indicated by an index.

func index(beforeUnicodeScalar: AttributedString.Index) -> AttributedString.Index

Returns the position of the Unicode scalar immediately before a Unicode scalar indicated by an index.

struct Index

A type that represents the position of a character or code unit within an attributed string.

