

- SwiftUI
- View fundamentals
- View
-  Appearance modifiers 

API Collection

# Appearance modifiers

Configure a view’s foreground and background styles, controls, and visibility.

## Overview

Use these modifiers to configure the appearance of a view, including the use of color and tint, and the application of overlays and background elements. Control the visibility of a view and specific elements within a view. Manage the shape and size of various controls.

For information about configuring views, see View configuration.

## Topics

### Colors and patterns

func backgroundStyle&lt;S>(S) -> some View

Sets the specified style to render backgrounds within the view.

func foregroundStyle&lt;S>(S) -> some View

Sets a view’s foreground elements to use a given style.

func foregroundStyle&lt;S1, S2>(S1, S2) -> some View

Sets the primary and secondary levels of the foreground style in the child view.

func foregroundStyle&lt;S1, S2, S3>(S1, S2, S3) -> some View

Sets the primary, secondary, and tertiary levels of the foreground style.

func allowedDynamicRange(Image.DynamicRange?) -> some View

Returns a new view configured with the specified allowed dynamic range.

### Tint

func tint(_:)

Sets the tint color within this view.

func listRowSeparatorTint(Color?, edges: VerticalEdge.Set) -> some View

Sets the tint color associated with a row.

func listSectionSeparatorTint(Color?, edges: VerticalEdge.Set) -> some View

Sets the tint color associated with a section.

func listItemTint(_:)

Sets a fixed tint color for content in a list.

### Light and dark appearance

func preferredColorScheme(ColorScheme?) -> some View

Sets the preferred color scheme for this presentation.

func preferredSurroundingsEffect(SurroundingsEffect?) -> some View

Applies an effect to passthrough video.

### Foreground elements

func border&lt;S>(S, width: CGFloat) -> some View

Adds a border to this view with the specified style and width.

func overlay&lt;V>(alignment: Alignment, content: () -> V) -> some View

Layers the views that you specify in front of this view.

func overlay&lt;S>(S, ignoresSafeAreaEdges: Edge.Set) -> some View

Layers the specified style in front of this view.

func overlay&lt;S, T>(S, in: T, fillStyle: FillStyle) -> some View

Layers a shape that you specify in front of this view.

### Background elements

func background&lt;V>(alignment: Alignment, content: () -> V) -> some View

Layers the views that you specify behind this view.

func background&lt;S>(S, ignoresSafeAreaEdges: Edge.Set) -> some View

Sets the view’s background to a style.

func background(ignoresSafeAreaEdges: Edge.Set) -> some View

Sets the view’s background to the default background style.

func background(_:in:fillStyle:)

Sets the view’s background to an insettable shape filled with a style.

func background(in:fillStyle:)

Sets the view’s background to an insettable shape filled with the default background style.

func alternatingRowBackgrounds(AlternatingRowBackgroundBehavior) -> some View

Overrides whether lists and tables in this view have alternating row backgrounds.

func listRowBackground&lt;V>(V?) -> some View

Places a custom background view behind a list row item.

func scrollContentBackground(Visibility) -> some View

Specifies the visibility of the background for scrollable views within this view.

func containerBackground&lt;S>(S, for: ContainerBackgroundPlacement) -> some View

Sets the container background of the enclosing container using a view.

func containerBackground&lt;V>(for: ContainerBackgroundPlacement, alignment: Alignment, content: () -> V) -> some View

Sets the container background of the enclosing container using a view.

func glassBackgroundEffect(displayMode: GlassBackgroundDisplayMode) -> some View

Fills the view’s background with an automatic glass background effect and container-relative rounded rectangle shape.

func glassBackgroundEffect&lt;S>(in: S, displayMode: GlassBackgroundDisplayMode) -> some View

Fills the view’s background with an automatic glass background effect and a shape that you specify.

### Control configuration

func defaultWheelPickerItemHeight(CGFloat) -> some View

Sets the default wheel-style picker item height.

func horizontalRadioGroupLayout() -> some View

Sets the style for radio group style pickers within this view to be horizontally positioned with the radio buttons inside the layout.

func controlSize(ControlSize) -> some View

Sets the size for controls within this view.

func buttonBorderShape(ButtonBorderShape) -> some View

Sets the border shape for buttons in this view.

func buttonRepeatBehavior(ButtonRepeatBehavior) -> some View

Sets whether buttons in this view should repeatedly trigger their actions on prolonged interactions.

func headerProminence(Prominence) -> some View

Sets the header prominence for this view.

func scrollDisabled(Bool) -> some View

Disables or enables scrolling in scrollable views.

func scrollBounceBehavior(ScrollBounceBehavior, axes: Axis.Set) -> some View

Configures the bounce behavior of scrollable views along the specified axis.

func scrollIndicatorsFlash(onAppear: Bool) -> some View

Flashes the scroll indicators of a scrollable view when it appears.

func scrollIndicatorsFlash(trigger: some Equatable) -> some View

Flashes the scroll indicators of scrollable views when a value changes.

func menuOrder(MenuOrder) -> some View

Sets the preferred order of items for menus presented from this view.

func menuActionDismissBehavior(MenuActionDismissBehavior) -> some View

Tells a menu whether to dismiss after performing an action.

func paletteSelectionEffect(PaletteSelectionEffect) -> some View

Specifies the selection effect to apply to a palette item.

func typeSelectEquivalent(_:)

Sets an explicit type select equivalent text in a collection, such as a list or table.

### Symbol effects

func symbolEffect&lt;T>(T, options: SymbolEffectOptions, isActive: Bool) -> some View

Returns a new view with a symbol effect added to it.

func symbolEffect&lt;T, U>(T, options: SymbolEffectOptions, value: U) -> some View

Returns a new view with a symbol effect added to it.

func symbolEffectsRemoved(Bool) -> some View

Returns a new view with its inherited symbol image effects either removed or left unchanged.

### Privacy and redaction

func privacySensitive(Bool) -> some View

Marks the view as containing sensitive, private user data.

func redacted(reason: RedactionReasons) -> some View

Adds a reason to apply a redaction to this view hierarchy.

func unredacted() -> some View

Removes any reason to apply a redaction to this view hierarchy.

func invalidatableContent(Bool) -> some View

Mark the receiver as their content might be invalidated.

### Visibility

func hidden() -> some View

Hides this view unconditionally.

func labelsHidden() -> some View

Hides the labels of any controls contained within this view.

func menuIndicator(Visibility) -> some View

Sets the menu indicator visibility for controls within this view.

func listRowSeparator(Visibility, edges: VerticalEdge.Set) -> some View

Sets the display mode for the separator associated with this specific row.

func listSectionSeparator(Visibility, edges: VerticalEdge.Set) -> some View

Sets whether to hide the separator associated with a list section.

func persistentSystemOverlays(Visibility) -> some View

Sets the preferred visibility of the non-transient system views overlaying the app.

func scrollIndicators(ScrollIndicatorVisibility, axes: Axis.Set) -> some View

Sets the visibility of scroll indicators within this view.

func scrollClipDisabled(Bool) -> some View

Sets whether a scroll view clips its content to its bounds.

func tableColumnHeaders(Visibility) -> some View

Controls the visibility of a `Table`’s column header views.

func upperLimbVisibility(Visibility) -> some View

Sets the preferred visibility of the user’s upper limbs, while an ImmersiveSpace scene is presented.

func volumeBaseplateVisibility(Visibility) -> some View

Sets the visibility of the baseplate of a volume, which appears when a user looks towards the ‘floor’ of a volume and during resize. Both `automatic` and `visible` will show the baseplate. `hidden` will never show it.

### Sensory feedback

func sensoryFeedback&lt;T>(SensoryFeedback, trigger: T) -> some View

Plays the specified `feedback` when the provided `trigger` value changes.

func sensoryFeedback&lt;T>(trigger: T, (T, T) -> SensoryFeedback?) -> some View

Plays feedback when returned from the `feedback` closure after the provided `trigger` value changes.

func sensoryFeedback&lt;T>(SensoryFeedback, trigger: T, condition: (T, T) -> Bool) -> some View

Plays the specified `feedback` when the provided `trigger` value changes and the `condition` closure returns `true`.

### Widget configuration

func widgetAccentable(Bool) -> some View

Adds the view and all of its subviews to the accented group.

func widgetCurvesContent(Bool) -> some View

Displays the widget’s content along a curve if the context allows it.

func widgetLabel(_:)

Returns a localized text label that displays additional content outside the accessory family widget’s main SwiftUI view.

func widgetLabel&lt;Label>(label: () -> Label) -> some View

Creates a label for displaying additional content outside an accessory family widget’s main SwiftUI view.

func dynamicIsland(verticalPlacement: DynamicIslandExpandedRegionVerticalPlacement) -> some View

Specifies the vertical placement for a view of an expanded Live Activity that appears in the Dynamic Island.

### Window behaviors

func windowDismissBehavior(WindowInteractionBehavior) -> some View

Configures the dismiss functionality for the window enclosing `self`.

func windowFullScreenBehavior(WindowInteractionBehavior) -> some View

Configures the full screen functionality for the window enclosing `self`.

func windowMinimizeBehavior(WindowInteractionBehavior) -> some View

Configures the minimize functionality for the window enclosing `self`.

func windowResizeBehavior(WindowInteractionBehavior) -> some View

Configures the resize functionality for the window enclosing `self`.

## See Also

### Configuring view elements

Accessibility modifiers

Make your SwiftUI apps accessible to everyone, including people with disabilities.

Text and symbol modifiers

Manage the rendering, selection, and entry of text in your view.

Auxiliary view modifiers

Add and configure supporting views, like toolbars and context menus.

Chart view modifiers

Configure charts that you declare with Swift Charts.

