

- SwiftUI
- UIHostingConfiguration
-  background(content:) 

Instance Method

# background(content:)

Sets the background contents for the hosting configuration’s enclosing cell.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
func background(@ViewBuilder content: () -> B) -> UIHostingConfiguration where B : View
```

## Discussion

The following example sets a custom view to the background of the cell:

```
UIHostingConfiguration {
    Text("My Contents")
}
.background {
    MyBackgroundView()
}
```

## See Also

### Setting the background

func background&lt;S>(S) -> UIHostingConfiguration&lt;Content, _UIHostingConfigurationBackgroundView&lt;S>>

Sets the background contents for the hosting configuration’s enclosing cell.

