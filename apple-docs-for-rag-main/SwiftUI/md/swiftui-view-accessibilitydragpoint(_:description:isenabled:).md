

- SwiftUI
- View
-  accessibilityDragPoint(\_:description:isEnabled:) 

Instance Method

# accessibilityDragPoint(\_:description:isEnabled:)

The point an assistive technology should use to begin a drag interaction.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
nonisolated
func accessibilityDragPoint(
    _ point: UnitPoint,
    description: LocalizedStringKey,
    isEnabled: Bool
) -> ModifiedContent
```

Show all declarations

## Parameters 

`point`  

The point the assitive technology will begin a drag interaction.

`description`  

The description of the drag interaction.

`isEnabled`  

If true the accessibility drag point is applied; otherwise the accessibility drag point is unchanged.

## Discussion

Use this modifier when you need to provide a description to users when prompted begin a drag interaction.

```
struct FileView: View {
    var filename: String

    var body: some View {
        FileIcon(filename: filename)
            .accessibilityDragPoint(
                .center, description: Text("Move \(filename)"))
    }
}
```

By default, if an accessible view or its subtree has drag and/or drop interactions, they will be automatically exposed by assistive technologies. However, if there is more than one such interaction, each drag or drop should have a description to disambiguate it and give a good user experience.

Note

An accessibility element can have multiple points for a drag, provided they have different descriptions.

## See Also

### Making gestures accessible

func accessibilityActivationPoint(_:)

The activation point for an element is the location assistive technologies use to initiate gestures.

func accessibilityActivationPoint(_:isEnabled:)

The activation point for an element is the location assistive technologies use to initiate gestures.

func accessibilityDragPoint(_:description:)

The point an assistive technology should use to begin a drag interaction.

func accessibilityDropPoint(_:description:)

The point an assistive technology should use to end a drag interaction.

func accessibilityDropPoint(_:description:isEnabled:)

The point an assistive technology should use to end a drag interaction.

func accessibilityDirectTouch(Bool, options: AccessibilityDirectTouchOptions) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Explicitly set whether this accessibility element is a direct touch area. Direct touch areas passthrough touch events to the app rather than being handled through an assistive technology, such as VoiceOver. The modifier accepts an optional `AccessibilityDirectTouchOptions` option set to customize the functionality of the direct touch area.

func accessibilityZoomAction((AccessibilityZoomGestureAction) -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility zoom action to the view. Actions allow assistive technologies, such as VoiceOver, to interact with the view by invoking the action.

struct AccessibilityDirectTouchOptions

An option set that defines the functionality of a view’s direct touch area.

struct AccessibilityZoomGestureAction

Position and direction information of a zoom gesture that someone performs with an assistive technology like VoiceOver.

