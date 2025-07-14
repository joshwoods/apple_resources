

- Swift
- String
-  lowercased() 

Instance Method

# lowercased()

Returns a lowercase version of the string.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func lowercased() -> String
```

## Return Value

A lowercase copy of the string.

## Discussion

Here’s an example of transforming a string to all lowercase letters.

```
let cafe = "BBQ Café 🍵"
print(cafe.lowercased())
// Prints "bbq café 🍵"
```

Complexity

O(*n*)

## See Also

### Changing Case

func uppercased() -> String

Returns an uppercase version of the string.

