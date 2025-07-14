

- SwiftUI
- UIHostingConfiguration
-  minSize(width:height:) 

Instance Method

# minSize(width:height:)

Sets the minimum size for the configuration.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
func minSize(
    width: CGFloat? = nil,
    height: CGFloat? = nil
) -> UIHostingConfiguration
```

## Parameters 

`width`  

The value to use for the width dimension. A value of `nil` indicates that the system default should be used.

`height`  

The value to use for the height dimension. A value of `nil` indicates that the system default should be used.

## Discussion

Use this modifier to indicate that a configuration’s associated cell can be resized to a specific minimum. The following example allows the cell to be compressed to zero size:

```
UIHostingConfiguration {
    Text("My Contents")
}
.minSize(width: 0, height: 0)
```

## See Also

### Setting a size

func minSize() -> UIHostingConfiguration&lt;Content, Background>

Sets the minimum size for the configuration.

Deprecated

