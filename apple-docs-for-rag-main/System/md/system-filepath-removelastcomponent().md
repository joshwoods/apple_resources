

- System
- FilePath
-  removeLastComponent() 

Instance Method

# removeLastComponent()

In-place mutating variant of `removingLastComponent`.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@discardableResult
mutating func removeLastComponent() -> Bool
```

## Discussion

If `self` only contains a root, does nothing and returns `false`. Otherwise removes `lastComponent` and returns `true`.

Example:

```
var path = "/usr/bin"
path.removeLastComponent() == true  // path is "/usr"
path.removeLastComponent() == true  // path is "/"
path.removeLastComponent() == false // path is "/"
```

