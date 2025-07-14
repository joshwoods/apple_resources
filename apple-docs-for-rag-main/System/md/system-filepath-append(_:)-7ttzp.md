

- System
- FilePath
-  append(\_:) 

Instance Method

# append(\_:)

Append the contents of `other`, ignoring any spurious leading separators.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func append(_ other: String)
```

## Discussion

A leading separator is spurious if `self` is non-empty.

Example:

```
var path: FilePath = ""
path.append("/var/www/website") // "/var/www/website"
path.append("static/assets") // "/var/www/website/static/assets"
path.append("/main.css") // "/var/www/website/static/assets/main.css"
```

