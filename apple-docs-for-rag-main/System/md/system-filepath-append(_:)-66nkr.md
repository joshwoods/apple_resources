

- System
- FilePath
-  append(\_:) 

Instance Method

# append(\_:)

Append `components` on to the end of this path.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func append(_ components: C) where C : Collection, C.Element == FilePath.Component
```

## Discussion

Example:

```
var path: FilePath = "/"
path.append(["usr", "local"])     // path is "/usr/local"
let otherPath: FilePath = "/bin/ls"
path.append(otherPath.components) // path is "/usr/local/bin/ls"
```

