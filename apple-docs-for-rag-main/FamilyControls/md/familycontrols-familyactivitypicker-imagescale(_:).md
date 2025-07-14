

- FamilyControls
- FamilyActivityPicker
-  imageScale(\_:) 

Instance Method

# imageScale(\_:)

Scales images within the view according to one of the relative sizes available including small, medium, and large images sizes.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 11.0+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func imageScale(_ scale: Image.Scale) -> some View
```

## Parameters 

`scale`  

One of the relative sizes provided by the image scale enumeration.

## Discussion

The example below shows the relative scaling effect. The system renders the image at a relative size based on the available space and configuration options of the image it is scaling.

```
VStack {
    HStack {
        Image(systemName: "heart.fill")
            .imageScale(.small)
        Text("Small")
    }
    HStack {
        Image(systemName: "heart.fill")
            .imageScale(.medium)
        Text("Medium")
    }

    HStack {
        Image(systemName: "heart.fill")
            .imageScale(.large)
        Text("Large")
    }
}
```

## See Also

### Scale

func scaledToFill() -> some View

Scales this view to fill its parent.

func scaledToFit() -> some View

Scales this view to fit its parent.

func scaleEffect(CGSize, anchor: UnitPoint) -> some View

Scales this view’s rendered output by the given vertical and horizontal size amounts, relative to an anchor point.

func scaleEffect(x: CGFloat, y: CGFloat, anchor: UnitPoint) -> some View

Scales this view’s rendered output by the given horizontal and vertical amounts, relative to an anchor point.

func aspectRatio(CGSize, contentMode: ContentMode) -> some View

Constrains this view’s dimensions to the aspect ratio of the given size.

