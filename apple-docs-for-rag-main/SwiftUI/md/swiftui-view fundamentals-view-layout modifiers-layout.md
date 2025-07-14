

- SwiftUI
- View fundamentals
- View
-  Layout modifiers 

API Collection

# Layout modifiers

Tell a view how to arrange itself within a view hierarchy by adjusting its size, position, alignment, padding, and so on.

## Overview

Use layout modifiers to fine tune the placement of views in a view hierarchy. You can adjust or constrain the size, position, and alignment of a view. You can also add padding around a view, and indicate how the view interacts with system-defined safe areas.

To get started arranging views, see Layout fundamentals. To make adjustments to a basic layout, see Layout adjustments.

## Topics

### Size

func frame(width: CGFloat?, height: CGFloat?, alignment: Alignment) -> some View

Positions this view within an invisible frame with the specified size.

func frame(depth: CGFloat?, alignment: DepthAlignment) -> some View

Positions this view within an invisible frame with the specified depth.

func frame(minWidth: CGFloat?, idealWidth: CGFloat?, maxWidth: CGFloat?, minHeight: CGFloat?, idealHeight: CGFloat?, maxHeight: CGFloat?, alignment: Alignment) -> some View

Positions this view within an invisible frame having the specified size constraints.

func frame(minDepth: CGFloat?, idealDepth: CGFloat?, maxDepth: CGFloat?, alignment: DepthAlignment) -> some View

Positions this view within an invisible frame having the specified depth constraints.

func containerRelativeFrame(Axis.Set, alignment: Alignment) -> some View

Positions this view within an invisible frame with a size relative to the nearest container.

func containerRelativeFrame(Axis.Set, alignment: Alignment, (CGFloat, Axis) -> CGFloat) -> some View

Positions this view within an invisible frame with a size relative to the nearest container.

func containerRelativeFrame(Axis.Set, count: Int, span: Int, spacing: CGFloat, alignment: Alignment) -> some View

Positions this view within an invisible frame with a size relative to the nearest container.

func fixedSize() -> some View

Fixes this view at its ideal size.

func fixedSize(horizontal: Bool, vertical: Bool) -> some View

Fixes this view at its ideal size in the specified dimensions.

func layoutPriority(Double) -> some View

Sets the priority by which a parent layout should apportion space to this child.

### Position

func position(CGPoint) -> some View

Positions the center of this view at the specified point in its parent’s coordinate space.

func position(x: CGFloat, y: CGFloat) -> some View

Positions the center of this view at the specified coordinates in its parent’s coordinate space.

func offset(CGSize) -> some View

Offset this view by the horizontal and vertical amount specified in the offset parameter.

func offset(x: CGFloat, y: CGFloat) -> some View

Offset this view by the specified horizontal and vertical distances.

func offset(z: CGFloat) -> some View

Brings a view forward in Z by the provided distance in points.

func coordinateSpace(NamedCoordinateSpace) -> some View

Assigns a name to the view’s coordinate space, so other code can operate on dimensions like points and sizes relative to the named space.

### Alignment

func alignmentGuide(_:computeValue:)

Sets the view’s horizontal alignment.

### Padding and spacing

func padding(_:)

Adds a different padding amount to each edge of this view.

func padding(Edge.Set, CGFloat?) -> some View

Adds an equal padding amount to specific edges of this view.

func padding3D(_:)

Pads this view using the edge insets you specify.

func padding3D(Edge3D.Set, CGFloat?) -> some View

Pads this view using the edge insets you specify.

func listRowInsets(EdgeInsets?) -> some View

Applies an inset to the rows in a list.

func scenePadding(Edge.Set) -> some View

Adds padding to the specified edges of this view using an amount that’s appropriate for the current scene.

func scenePadding(ScenePadding, edges: Edge.Set) -> some View

Adds a specified kind of padding to the specified edges of this view using an amount that’s appropriate for the current scene.

func listRowSpacing(CGFloat?) -> some View

Sets the vertical spacing between two adjacent rows in a List.

func listSectionSpacing(_:)

Sets the spacing between adjacent sections in a List to a custom value.

### Grid configuration

func gridCellColumns(Int) -> some View

Tells a view that acts as a cell in a grid to span the specified number of columns.

func gridCellAnchor(UnitPoint) -> some View

Specifies a custom alignment anchor for a view that acts as a grid cell.

func gridCellUnsizedAxes(Axis.Set) -> some View

Asks grid layouts not to offer the view extra size in the specified axes.

func gridColumnAlignment(HorizontalAlignment) -> some View

Overrides the default horizontal alignment of the grid column that the view appears in.

### Safe area and margins

func ignoresSafeArea(SafeAreaRegions, edges: Edge.Set) -> some View

Expands the safe area of a view.

func safeAreaInset(edge:alignment:spacing:content:)

Shows the specified content beside the modified view.

func safeAreaPadding(_:)

Adds the provided insets into the safe area of this view.

func safeAreaPadding(Edge.Set, CGFloat?) -> some View

Adds the provided insets into the safe area of this view.

func contentMargins(CGFloat, for: ContentMarginPlacement) -> some View

Configures the content margin for a provided placement.

func contentMargins(_:_:for:)

Configures the content margin for a provided placement.

### Layer order

func zIndex(Double) -> some View

Controls the display order of overlapping views.

### Layout direction

func layoutDirectionBehavior(LayoutDirectionBehavior) -> some View

Sets the behavior of this view for different layout directions.

### Custom layout characteristics

func layoutValue&lt;K>(key: K.Type, value: K.Value) -> some View

Associates a value with a custom layout property.

## See Also

### Drawing views

Style modifiers

Apply built-in styles to different types of views.

Graphics and rendering modifiers

Affect the way the system draws a view, for example by scaling or masking a view, or by applying graphical effects.

