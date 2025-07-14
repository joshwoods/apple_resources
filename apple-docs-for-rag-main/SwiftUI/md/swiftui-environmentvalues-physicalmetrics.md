

- SwiftUI
- EnvironmentValues
-  physicalMetrics 

Instance Property

# physicalMetrics

The physical metrics associated with a scene.

visionOS 1.0+

``` source
var physicalMetrics: PhysicalMetricsConverter { get set }
```

## Discussion

Reading this value returns a `PhysicalMetricsConverter` corresponding to the window scene associated with the environment’s reader. The converter can convert point sizes into physical measurements of length, and vice versa.

Reading this value is only supported in the body of a View or of a type that inherits a View’s environment.

## See Also

### View attributes

var allowedDynamicRange: Image.DynamicRange?

The allowed dynamic range for the view, or nil.

var backgroundMaterial: Material?

The material underneath the current view.

var backgroundProminence: BackgroundProminence

The prominence of the background underneath views associated with this environment.

var backgroundStyle: AnyShapeStyle?

An optional style that overrides the default system background style when set.

var badgeProminence: BadgeProminence

The prominence to apply to badges associated with this environment.

var contentTransition: ContentTransition

The current method of animating the contents of views.

var contentTransitionAddsDrawingGroup: Bool

A Boolean value that controls whether views that render content transitions use GPU-accelerated rendering.

var defaultMinListHeaderHeight: CGFloat?

The default minimum height of a header in a list.

var defaultMinListRowHeight: CGFloat

The default minimum height of a row in a `List`. The default minimum height of a row in a list.

var headerProminence: Prominence

The prominence to apply to section headers within a view.

var realityKitScene: Scene?

var realityViewCameraControls: CameraControls

The camera controls for the reality view.

var redactionReasons: RedactionReasons

The current redaction reasons applied to the view hierarchy.

var springLoadingBehavior: SpringLoadingBehavior

The behavior of spring loaded interactions for the views associated with this environment.

var symbolRenderingMode: SymbolRenderingMode?

The current symbol rendering mode, or `nil` denoting that the mode is picked automatically using the current image and foreground style as parameters.

