

- SwiftUI
- UIHostingConfiguration
-  margins(\_:\_:) 

Instance Method

# margins(\_:\_:)

Sets the margins around the content of the configuration.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
func margins(
    _ edges: Edge.Set = .all,
    _ insets: EdgeInsets
) -> UIHostingConfiguration
```

Show all declarations

## Parameters 

`edges`  

The edges to apply the insets. Any edges not specified will use the system default values. The default value is all.

`insets`  

The insets to apply.

## Discussion

Use this modifier to replace the default margins applied to the root of the configuration. The following example creates 10 points of space between the content and the background on the leading edge and 20 points of space on the trailing edge:

```
UIHostingConfiguration {
    Text("My Contents")
}
.margins(.horizontal, 20.0)
```

