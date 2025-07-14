

- SwiftUI
- PreviewProvider
-  previews 

Type Property

# previews

A collection of views to preview.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@ViewBuilder @MainActor @preconcurrency
static var previews: Self.Previews { get }
```

**Required**

## Discussion

Implement a computed `previews` property to indicate the content to preview. Xcode generates a preview for each view that you list. You can apply View modifiers to the views, like you do when creating a custom view. For a preview, you can also use various preview-specific modifiers that customize the preview. For example, you can choose a specific device for the preview by adding the previewDevice(_:) modifier:

```
struct CircleImage_Previews: PreviewProvider {
    static var previews: some View {
        CircleImage()
            .previewDevice(PreviewDevice(rawValue: "iPad Pro (11-inch)"))
    }
}
```

For the full list of preview-specific modifiers, see Previews in Xcode.

## See Also

### Creating a preview

associatedtype Previews : View

The type to preview.

**Required**

