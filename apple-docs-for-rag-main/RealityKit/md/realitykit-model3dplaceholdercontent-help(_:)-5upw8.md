

- RealityKit
- Model3DPlaceholderContent
-  help(\_:) 

Instance Method

# help(\_:)

Adds help text to a view using a localized string that you provide.

RealityKitSwiftUIiOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
nonisolated
func help(_ textKey: LocalizedStringKey) -> some View
```

## Parameters 

`textKey`  

The key for the localized text to use as help.

## Discussion

Adding help to a view configures the view’s accessibility hint and its help tag (also called a *tooltip*) in macOS or visionOS. For more information on using help tags, see Offering help in the Human Interface Guidelines.

```
Button(action: composeMessage) {
    Image(systemName: "square.and.pencil")
}
.help("Compose a new message")
```

