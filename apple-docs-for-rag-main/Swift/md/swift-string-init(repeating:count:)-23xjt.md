

- Swift
- String
-  init(repeating:count:) 

Initializer

# init(repeating:count:)

Creates a new string representing the given string repeated the specified number of times.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    repeating repeatedValue: String,
    count: Int
)
```

## Parameters 

`repeatedValue`  

The string to repeat.

`count`  

The number of times to repeat `repeatedValue` in the resulting string.

## Discussion

For example, you can use this initializer to create a string with ten `"ab"` strings in a row.

```
let s = String(repeating: "ab", count: 10)
print(s)
// Prints "abababababababababab"
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

init&lt;S>(S)

Creates a new string containing the characters in the given sequence.

init(Substring)

Creates a new string from the given substring.

init(repeating: Character, count: Int)

Creates a string representing the given character repeated the specified number of times.

init(unsafeUninitializedCapacity: Int, initializingUTF8With: (UnsafeMutableBufferPointer&lt;UInt8>) throws -> Int) rethrows

Creates a new string with the specified capacity in UTF-8 code units, and then calls the given closure with a buffer covering the string’s uninitialized memory.

