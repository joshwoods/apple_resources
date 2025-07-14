

- System
- FilePath
-  removePrefix(\_:) 

Instance Method

# removePrefix(\_:)

If `prefix` is a prefix of `self`, removes it and returns `true`. Otherwise returns `false`.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func removePrefix(_ prefix: FilePath) -> Bool
```

## Discussion

Example:

```
var path: FilePath = "/usr/local/bin"
path.removePrefix("/usr/bin")   // false
path.removePrefix("/us")        // false
path.removePrefix("/usr/local") // true, path is "bin"
```

