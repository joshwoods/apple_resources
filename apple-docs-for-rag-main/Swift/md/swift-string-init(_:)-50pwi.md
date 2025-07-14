

- Swift
- String
-  init(\_:) 

Initializer

# init(\_:)

Creates a new string containing the characters in the given sequence.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ other: S) where S : LosslessStringConvertible, S : Sequence, S.Element == Character
```

## Parameters 

`other`  

A string instance or another sequence of characters.

## Discussion

You can use this initializer to create a new string from the result of one or more collection operations on a string’s characters. For example:

```
let str = "The rain in Spain stays mainly in the plain."

let vowels: Set = ["a", "e", "i", "o", "u"]
let disemvoweled = String(str.lazy.filter { !vowels.contains($0) })

print(disemvoweled)
// Prints "Th rn n Spn stys mnly n th pln."
```

## See Also

### Creating a String

init(decoding: FilePath)

Creates a string by interpreting the file path’s content as UTF-8 on Unix and UTF-16 on Windows.

init()

Creates an empty string.

init(Character)

Creates a string containing the given character.

init&lt;S>(S)

Creates a new string containing the characters in the given sequence.

init&lt;S>(S)

Creates a new instance of a collection containing the elements of a sequence.

init(Substring)

Creates a new string from the given substring.

init(repeating: String, count: Int)

Creates a new string representing the given string repeated the specified number of times.

init(repeating: Character, count: Int)

Creates a string representing the given character repeated the specified number of times.

init(unsafeUninitializedCapacity: Int, initializingUTF8With: (UnsafeMutableBufferPointer&lt;UInt8>) throws -> Int) rethrows

Creates a new string with the specified capacity in UTF-8 code units, and then calls the given closure with a buffer covering the string’s uninitialized memory.

