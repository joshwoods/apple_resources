

- Foundation
- URL
-  formatted(\_:) 

Instance Method

# formatted(\_:)

Formats the URL, using the provided format style.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func formatted(_ format: F) -> F.FormatOutput where F : FormatStyle, F.FormatInput == URL
```

## Parameters 

`format`  

The format style to apply when formatting the URL.

## Return Value

A formatted string representation of the URL.

## Discussion

Use this method when you want to format a single URL value with a specific format style, or call it repeatedly with different format styles. The following example uses the static accessor `URL/FormatStyle/url-4fry3` to get a default style, then modifies its behavior to include or omit different URL components when formatted(_:) creates the string:

```
let url = URL(string:"https://www.example.com:8080/path/to/endpoint?key=value")!
let formatted = url.formatted(.url
    .scheme(.never)
    .host(.always)
    .port(.never)
    .path(.always)
    .query(.never)) // "www.example.com/path/to/endpoint"

```

## See Also

### Formatting a URL

func formatted() -> String

Formats the URL using a default format style.

struct FormatStyle

A structure that converts between URL instances and their textual representations.

