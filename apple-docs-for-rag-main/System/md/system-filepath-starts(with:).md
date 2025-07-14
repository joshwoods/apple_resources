

- System
- FilePath
-  starts(with:) 

Instance Method

# starts(with:)

Returns whether `other` is a prefix of `self`, only considering whole path components.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func starts(with other: FilePath) -> Bool
```

## Discussion

Example:

```
let path: FilePath = "/usr/bin/ls"
path.starts(with: "/")              // true
path.starts(with: "/usr/bin")       // true
path.starts(with: "/usr/bin/ls")    // true
path.starts(with: "/usr/bin/ls///") // true
path.starts(with: "/us")            // false
```

