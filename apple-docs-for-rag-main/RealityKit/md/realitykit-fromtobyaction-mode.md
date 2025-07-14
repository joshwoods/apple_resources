

- RealityKit
- FromToByAction
-  mode 

Instance Property

# mode

Determines the entities transform from and to are relative to.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var mode: FromToByAction.TransformMode? { get }
```

Available when `Value` is `Transform`.

## Discussion

Note

The expection to this mode is `by`. This property is relative to the starting value, Set this to `nil` if only `by` is specified.

