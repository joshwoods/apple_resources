

- System
- FilePath
-  ends(with:) 

Instance Method

# ends(with:)

Returns whether `other` is a suffix of `self`, only considering whole path components.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func ends(with other: FilePath) -> Bool
```

## Discussion

Example:

```
let path: FilePath = "/usr/bin/ls"
path.ends(with: "ls")             // true
path.ends(with: "bin/ls")         // true
path.ends(with: "usr/bin/ls")     // true
path.ends(with: "/usr/bin/ls///") // true
path.ends(with: "/ls")            // false
```

