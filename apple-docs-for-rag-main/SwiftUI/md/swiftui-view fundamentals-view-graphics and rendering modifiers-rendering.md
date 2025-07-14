

- SwiftUI
- View fundamentals
- View
-  Graphics and rendering modifiers 

API Collection

# Graphics and rendering modifiers

Affect the way the system draws a view, for example by scaling or masking a view, or by applying graphical effects.

## Overview

Use these view modifiers to apply many of the rendering effects typically associated with a graphics context, like adding masks and creating composites. You can apply these effects to graphical views, like Shapes, as well as any other SwiftUI view.

When you do need the flexibility of immediate mode drawing in a graphics context, use a Canvas view instead. This can be particularly helpful when you want to draw an extremely large number of dynamic shapes — for example, to create particle effects.

For more information about using these effects in your app, see Drawing and graphics.

## Topics

### Masks and clipping

func mask&lt;Mask>(alignment: Alignment, () -> Mask) -> some View

Masks this view using the alpha channel of the given view.

func clipped(antialiased: Bool) -> some View

Clips this view to its bounding rectangular frame.

func clipShape&lt;S>(S, style: FillStyle) -> some View

Sets a clipping shape for this view.

func containerShape&lt;T>(T) -> some View

Sets the container shape to use for any container relative shape within this view.

### Scale

func scaledToFill() -> some View

Scales this view to fill its parent.

func scaledToFit() -> some View

Scales this view to fit its parent.

func scaleEffect(_:anchor:)

Scales this view’s rendered output by the given amount in both the horizontal and vertical directions, relative to an anchor point.

func scaleEffect(x: CGFloat, y: CGFloat, anchor: UnitPoint) -> some View

Scales this view’s rendered output by the given horizontal and vertical amounts, relative to an anchor point.

func scaleEffect(x: CGFloat, y: CGFloat, z: CGFloat, anchor: UnitPoint3D) -> some View

Scales this view by the specified horizontal, vertical, and depth factors.

func imageScale(Image.Scale) -> some View

Scales images within the view according to one of the relative sizes available including small, medium, and large images sizes.

func aspectRatio(_:contentMode:)

Constrains this view’s dimensions to the specified aspect ratio.

### Rotation and transformation

func rotationEffect(Angle, anchor: UnitPoint) -> some View

Rotates a view’s rendered output in two dimensions around the specified point.

func rotation3DEffect(Rotation3D, anchor: UnitPoint3D) -> some View

Rotates the view’s content by the specified 3D rotation value.

func rotation3DEffect(Angle, axis: (x: CGFloat, y: CGFloat, z: CGFloat), anchor: UnitPoint, anchorZ: CGFloat, perspective: CGFloat) -> some View

Renders a view’s content as if it’s rotated in three dimensions around the specified axis.

func rotation3DEffect(_:axis:anchor:)

Rotates the view’s content by an angle about an axis that you specify as a tuple of elements.

func perspectiveRotationEffect(Angle, axis: (x: CGFloat, y: CGFloat, z: CGFloat), anchor: UnitPoint, anchorZ: CGFloat, perspective: CGFloat) -> some View

Renders a view’s content as if it’s rotated in three dimensions around the specified axis.

func projectionEffect(ProjectionTransform) -> some View

Applies a projection transformation to this view’s rendered output.

func transformEffect(CGAffineTransform) -> some View

Applies an affine transformation to this view’s rendered output.

func transform3DEffect(AffineTransform3D) -> some View

Applies a 3D transformation to the receiver.

### Graphical effects

func blur(radius: CGFloat, opaque: Bool) -> some View

Applies a Gaussian blur to this view.

func opacity(Double) -> some View

Sets the transparency of this view.

func brightness(Double) -> some View

Brightens this view by the specified amount.

func contrast(Double) -> some View

Sets the contrast and separation between similar colors in this view.

func colorInvert() -> some View

Inverts the colors in this view.

func colorMultiply(Color) -> some View

Adds a color multiplication effect to this view.

func saturation(Double) -> some View

Adjusts the color saturation of this view.

func grayscale(Double) -> some View

Adds a grayscale effect to this view.

func hueRotation(Angle) -> some View

Applies a hue rotation effect to this view.

func luminanceToAlpha() -> some View

Adds a luminance to alpha effect to this view.

func shadow(color: Color, radius: CGFloat, x: CGFloat, y: CGFloat) -> some View

Adds a shadow to this view.

func visualEffect((EmptyVisualEffect, GeometryProxy) -> some VisualEffect) -> some View

Applies effects to this view, while providing access to layout information through a geometry proxy.

func visualEffect3D((EmptyVisualEffect, GeometryProxy3D) -> some VisualEffect) -> some View

Applies effects to this view, while providing access to layout information through a 3D geometry proxy.

### Shaders

func colorEffect(Shader, isEnabled: Bool) -> some View

Returns a new view that applies `shader` to `self` as a filter effect on the color of each pixel.

func distortionEffect(Shader, maxSampleOffset: CGSize, isEnabled: Bool) -> some View

Returns a new view that applies `shader` to `self` as a geometric distortion effect on the location of each pixel.

func layerEffect(Shader, maxSampleOffset: CGSize, isEnabled: Bool) -> some View

Returns a new view that applies `shader` to `self` as a filter on the raster layer created from `self`.

### Composites

func blendMode(BlendMode) -> some View

Sets the blend mode for compositing this view with overlapping views.

func compositingGroup() -> some View

Wraps this view in a compositing group.

func drawingGroup(opaque: Bool, colorMode: ColorRenderingMode) -> some View

Composites this view’s contents into an offscreen image before final display.

### Animations

func animation(_:)

Applies the given animation to this view when this view changes.

func animation&lt;V>(Animation?, value: V) -> some View

Applies the given animation to this view when the specified value changes.

func animation&lt;V>(Animation?, body: (PlaceholderContentView&lt;Self>) -> V) -> some View

Applies the given animation to all animatable values within the `body` closure.

func keyframeAnimator&lt;Value>(initialValue: Value, repeating: Bool, content: (PlaceholderContentView&lt;Self>, Value) -> some View, keyframes: (Value) -> some Keyframes) -> some View

Loops the given keyframes continuously, updating the view using the modifiers you apply in `body`.

func keyframeAnimator&lt;Value>(initialValue: Value, trigger: some Equatable, content: (PlaceholderContentView&lt;Self>, Value) -> some View, keyframes: (Value) -> some Keyframes) -> some View

Plays the given keyframes when the given trigger value changes, updating the view using the modifiers you apply in `body`.

func phaseAnimator&lt;Phase>(some Sequence, content: (PlaceholderContentView&lt;Self>, Phase) -> some View, animation: (Phase) -> Animation?) -> some View

Animates effects that you apply to a view over a sequence of phases that change continuously.

func phaseAnimator&lt;Phase>(some Sequence, trigger: some Equatable, content: (PlaceholderContentView&lt;Self>, Phase) -> some View, animation: (Phase) -> Animation?) -> some View

Animates effects that you apply to a view over a sequence of phases that change based on a trigger.

func contentTransition(ContentTransition) -> some View

Modifies the view to use a given transition as its method of animating changes to the contents of its views.

func transition(_:)

Associates a transition with the view.

func transaction((inout Transaction) -> Void) -> some View

Applies the given transaction mutation function to all animations used within the view.

func transaction(value: some Equatable, (inout Transaction) -> Void) -> some View

Applies the given transaction mutation function to all animations used within the view.

func transaction&lt;V>((inout Transaction) -> Void, body: (PlaceholderContentView&lt;Self>) -> V) -> some View

Applies the given transaction mutation function to all animations used within the `body` closure.

func contentTransition(ContentTransition) -> some View

Modifies the view to use a given transition as its method of animating changes to the contents of its views.

func matchedGeometryEffect&lt;ID>(id: ID, in: Namespace.ID, properties: MatchedGeometryProperties, anchor: UnitPoint, isSource: Bool) -> some View

Defines a group of views with synchronized geometry using an identifier and namespace that you provide.

func geometryGroup() -> some View

Isolates the geometry (e.g. position and size) of the view from its parent view.

## See Also

### Drawing views

Style modifiers

Apply built-in styles to different types of views.

Layout modifiers

Tell a view how to arrange itself within a view hierarchy by adjusting its size, position, alignment, padding, and so on.

