

- Swift
- String
-  uppercased() 

Instance Method

# uppercased()

Returns an uppercase version of the string.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func uppercased() -> String
```

## Return Value

An uppercase copy of the string.

## Discussion

The following example transforms a string to uppercase letters:

```
let cafe = "Café 🍵"
print(cafe.uppercased())
// Prints "CAFÉ 🍵"
```

Complexity

O(*n*)

## See Also

### Changing Case

func lowercased() -> String

Returns a lowercase version of the string.

