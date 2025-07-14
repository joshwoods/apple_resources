

- Foundation
- URL
-  formatted() 

Instance Method

# formatted()

Formats the URL using a default format style.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func formatted() -> String
```

## Return Value

A string representation of the URL, formatted according to the default format style.

## Discussion

Use this method to create a string representation of a URL using the default URL.FormatStyle configuration. As seen in the following example, the default style creates a string with the scheme, host, and path, but not the port or query.

```
let url = URL(string:"https://www.example.com:8080/path/to/endpoint?key=value")!
let formatted = url.formatted() // "https://www.example.com/path/to/endpoint"
```

To customize formatting of the URL, use formatted(_:), passing in a customized URL.FormatStyle.

## See Also

### Formatting a URL

func formatted&lt;F>(F) -> F.FormatOutput

Formats the URL, using the provided format style.

struct FormatStyle

A structure that converts between URL instances and their textual representations.

