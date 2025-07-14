

- SwiftUI
- UIHostingConfiguration
-  background(\_:) 

Instance Method

# background(\_:)

Sets the background contents for the hosting configuration’s enclosing cell.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
func background(_ style: S) -> UIHostingConfiguration> where S : ShapeStyle
```

## Parameters 

`style`  

The shape style to be used as the background of the cell.

## Discussion

The following example sets a custom view to the background of the cell:

```
UIHostingConfiguration {
    Text("My Contents")
}
.background(Color.blue)
```

## See Also

### Setting the background

func background&lt;B>(content: () -> B) -> UIHostingConfiguration&lt;Content, B>

Sets the background contents for the hosting configuration’s enclosing cell.

