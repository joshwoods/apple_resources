

- Swift
- Dictionary
-  init(dictionaryLiteral:) 

Initializer

# init(dictionaryLiteral:)

Creates a dictionary initialized with a dictionary literal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(dictionaryLiteral elements: (Key, Value)...)
```

Available when `Key` conforms to `Hashable`.

## Parameters 

`elements`  

The key-value pairs that will make up the new dictionary. Each key in `elements` must be unique.

## Discussion

Do not call this initializer directly. It is called by the compiler to handle dictionary literals. To use a dictionary literal as the initial value of a dictionary, enclose a comma-separated list of key-value pairs in square brackets.

For example, the code sample below creates a dictionary with string keys and values.

```
let countryCodes = ["BR": "Brazil", "GH": "Ghana", "JP": "Japan"]
print(countryCodes)
// Prints "["BR": "Brazil", "JP": "Japan", "GH": "Ghana"]"
```

## See Also

### Infrequently Used Functionality

var hashValue: Int

The hash value.

