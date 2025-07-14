

- SwiftUI
-  EnvironmentValues 

Structure

# EnvironmentValues

A collection of environment values propagated through a view hierarchy.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct EnvironmentValues
```

## Overview

SwiftUI exposes a collection of values to your app’s views in an `EnvironmentValues` structure. To read a value from the structure, declare a property using the Environment property wrapper and specify the value’s key path. For example, you can read the current locale:

```
@Environment(\.locale) var locale: Locale
```

Use the property you declare to dynamically control a view’s layout. SwiftUI automatically sets or updates many environment values, like pixelLength, scenePhase, or locale, based on device characteristics, system state, or user settings. For others, like lineLimit, SwiftUI provides a reasonable default value.

You can set or override some values using the environment(_:_:) view modifier:

```
MyView()
    .environment(\.lineLimit, 2)
```

The value that you set affects the environment for the view that you modify — including its descendants in the view hierarchy — but only up to the point where you apply a different environment modifier.

SwiftUI provides dedicated view modifiers for setting some values, which typically makes your code easier to read. For example, rather than setting the lineLimit value directly, as in the previous example, you should instead use the lineLimit(_:) modifier:

```
MyView()
    .lineLimit(2)
```

In some cases, using a dedicated view modifier provides additional functionality. For example, you must use the preferredColorScheme(_:) modifier rather than setting colorScheme directly to ensure that the new value propagates up to the presenting container when presenting a view like a popover:

```
MyView()
    .popover(isPresented: $isPopped) {
        PopoverContent()
            .preferredColorScheme(.dark)
    }
```

Create a custom environment value by declaring a new property in an extension to the environment values structure and applying the Entry() macro to the variable declaration:

```
extension EnvironmentValues {
    @Entry var myCustomValue: String = "Default value"
}

extension View {
    func myCustomValue(_ myCustomValue: String) -> some View {
        environment(\.myCustomValue, myCustomValue)
    }
}
```

Clients of your value then access the value in the usual way, reading it with the Environment property wrapper, and setting it with the `myCustomValue` view modifier.

## Topics

### Creating and accessing values

init()

Creates an environment values instance.

subscript(_:)

Accesses the environment value associated with a custom key.

var description: String

A string that represents the contents of the environment values instance.

### Accessibility

var accessibilityAssistiveAccessEnabled: Bool

A Boolean value that indicates whether Assistive Access is in use.

var accessibilityDimFlashingLights: Bool

Whether the setting to reduce flashing or strobing lights in video content is on. This setting can also be used to determine if UI in playback controls should be shown to indicate upcoming content that includes flashing or strobing lights.

var accessibilityDifferentiateWithoutColor: Bool

Whether the system preference for Differentiate without Color is enabled.

var accessibilityEnabled: Bool

A Boolean value that indicates whether the user has enabled an assistive technology.

var accessibilityInvertColors: Bool

Whether the system preference for Invert Colors is enabled.

var accessibilityLargeContentViewerEnabled: Bool

Whether the Large Content Viewer is enabled.

var accessibilityPlayAnimatedImages: Bool

Whether the setting for playing animations in an animated image is on. When this value is false, any presented image that contains animation should not play automatically.

var accessibilityPrefersHeadAnchorAlternative: Bool

Whether the system setting to prefer alternatives to head-anchored content is on.

var accessibilityQuickActionsEnabled: Bool

A Boolean that indicates whether the quick actions feature is enabled.

var accessibilityReduceMotion: Bool

Whether the system preference for Reduce Motion is enabled.

var accessibilityReduceTransparency: Bool

Whether the system preference for Reduce Transparency is enabled.

var accessibilityShowButtonShapes: Bool

Whether the system preference for Show Button Shapes is enabled.

var accessibilitySwitchControlEnabled: Bool

A Boolean value that indicates whether the Switch Control motor accessibility feature is in use.

var accessibilityVoiceOverEnabled: Bool

A Boolean value that indicates whether the VoiceOver screen reader is in use.

var legibilityWeight: LegibilityWeight?

The font weight to apply to text.

### Actions

var dismiss: DismissAction

An action that dismisses the current presentation.

var dismissSearch: DismissSearchAction

An action that ends the current search interaction.

var dismissWindow: DismissWindowAction

A window dismissal action stored in a view’s environment.

var openImmersiveSpace: OpenImmersiveSpaceAction

An action that presents an immersive space.

var dismissImmersiveSpace: DismissImmersiveSpaceAction

An immersive space dismissal action stored in a view’s environment.

var newDocument: NewDocumentAction

An action in the environment that presents a new document.

var openDocument: OpenDocumentAction

An action in the environment that presents an existing document.

var openURL: OpenURLAction

An action that opens a URL.

var openWindow: OpenWindowAction

A window presentation action stored in a view’s environment.

var pushWindow: PushWindowAction

A window presentation action stored in a view’s environment.

var purchase: PurchaseAction

An action that starts an in-app purchase.

var refresh: RefreshAction?

A refresh action stored in a view’s environment.

var rename: RenameAction?

An action that activates the standard rename interaction.

var resetFocus: ResetFocusAction

An action that requests the focus system to reevaluate default focus.

var openSettings: OpenSettingsAction

A Settings presentation action stored in a view’s environment.

### Authentication

var authorizationController: AuthorizationController

A value provided in the SwiftUI environment that views can use to perform authorization requests.

var webAuthenticationSession: WebAuthenticationSession

A value provided in the SwiftUI environment that views can use to authenticate a user through a web service.

### Controls and input

var buttonRepeatBehavior: ButtonRepeatBehavior

Whether buttons with this associated environment should repeatedly trigger their actions on prolonged interactions.

var controlSize: ControlSize

The size to apply to controls within a view.

var defaultWheelPickerItemHeight: CGFloat

The default height of an item in a wheel-style picker, such as a date picker.

var keyboardShortcut: KeyboardShortcut?

The keyboard shortcut that buttons in this environment will be triggered with.

var menuIndicatorVisibility: Visibility

The menu indicator visibility to apply to controls within a view.

var menuOrder: MenuOrder

The preferred order of items for menus presented from this view.

var searchSuggestionsPlacement: SearchSuggestionsPlacement

The current placement of search suggestions.

var preferredPencilDoubleTapAction: PencilPreferredAction

The action that the user prefers to perform after double-tapping their Apple Pencil, as selected in the Settings app.

var preferredPencilSqueezeAction: PencilPreferredAction

The action that the user prefers to perform when squeezing their Apple Pencil, as selected in the Settings app.

### Display characteristics

var appearsActive: Bool

Whether views and styles in this environment should prefer an active appearance over an inactive appearance.

var colorScheme: ColorScheme

The color scheme of this environment.

var colorSchemeContrast: ColorSchemeContrast

The contrast associated with the color scheme of this environment.

var displayScale: CGFloat

The display scale of this environment.

var horizontalSizeClass: UserInterfaceSizeClass?

The horizontal size class of this environment.

var imageScale: Image.Scale

The image scale for this environment.

var pixelLength: CGFloat

The size of a pixel on the screen.

var sidebarRowSize: SidebarRowSize

The current size of sidebar rows.

var verticalSizeClass: UserInterfaceSizeClass?

The vertical size class of this environment.

var immersiveSpaceDisplacement: Pose3D

The displacement that the system applies to the immersive space when moving the space away from its default position, in meters.

var labelsVisibility: Visibility

The labels visibility set by labelsVisibility(_:).

var materialActiveAppearance: MaterialActiveAppearance

The behavior materials should use for their active state, defaulting to `automatic`.

struct TabBarPlacement

A placement for tabs in a tab view.

var toolbarLabelStyle: ToolbarLabelStyle?

The label style to apply to controls within a toolbar.

### Global objects

var calendar: Calendar

The current calendar that views should use when handling dates.

var documentConfiguration: DocumentConfiguration?

The configuration of a document in a DocumentGroup.

var locale: Locale

The current locale that views should use.

var managedObjectContext: NSManagedObjectContext

var modelContext: ModelContext

The SwiftData model context that will be used for queries and other model operations within this environment.

var timeZone: TimeZone

The current time zone that views should use when handling dates.

var undoManager: UndoManager?

The undo manager used to register a view’s undo operations.

### Scrolling

var isScrollEnabled: Bool

A Boolean value that indicates whether any scroll views associated with this environment allow scrolling to occur.

var horizontalScrollIndicatorVisibility: ScrollIndicatorVisibility

The visibility to apply to scroll indicators of any horizontally scrollable content.

var verticalScrollIndicatorVisibility: ScrollIndicatorVisibility

The visiblity to apply to scroll indicators of any vertically scrollable content.

var scrollDismissesKeyboardMode: ScrollDismissesKeyboardMode

The way that scrollable content interacts with the software keyboard.

var horizontalScrollBounceBehavior: ScrollBounceBehavior

The scroll bounce mode for the horizontal axis of scrollable views.

var verticalScrollBounceBehavior: ScrollBounceBehavior

The scroll bounce mode for the vertical axis of scrollable views.

### State

var editMode: Binding&lt;EditMode>?

An indication of whether the user can edit the contents of a view associated with this environment.

var isActivityFullscreen: Bool

A Boolean value that indicates whether the Live Activity appears in a full-screen presentation.

var isEnabled: Bool

A Boolean value that indicates whether the view associated with this environment allows user interaction.

var isFocused: Bool

Returns whether the nearest focusable ancestor has focus.

var isFocusEffectEnabled: Bool

A Boolean value that indicates whether the view associated with this environment allows focus effects to be displayed.

var isHoverEffectEnabled: Bool

A Boolean value that indicates whether the view associated with this environment allows hover effects to be displayed.

var isLuminanceReduced: Bool

A Boolean value that indicates whether the display or environment currently requires reduced luminance.

var isPresented: Bool

A Boolean value that indicates whether the view associated with this environment is currently presented.

var isSceneCaptured: Bool

The current capture state.

var isSearching: Bool

A Boolean value that indicates when the user is searching.

var isTabBarShowingSections: Bool

A Boolean value that determines whether a tab view shows the expanded contents of a tab section.

var scenePhase: ScenePhase

The current phase of the scene.

var supportsMultipleWindows: Bool

A Boolean value that indicates whether the current platform supports opening multiple windows.

### StoreKit configuration

var displayStoreKitMessage: DisplayMessageAction

var requestReview: RequestReviewAction

### Text styles

var allowsTightening: Bool

A Boolean value that indicates whether inter-character spacing should tighten to fit the text into the available space.

var autocorrectionDisabled: Bool

A Boolean value that determines whether the view hierarchy has auto-correction enabled.

var dynamicTypeSize: DynamicTypeSize

The current Dynamic Type size.

var font: Font?

The default font of this environment.

var layoutDirection: LayoutDirection

The layout direction associated with the current environment.

var lineLimit: Int?

The maximum number of lines that text can occupy in a view.

var lineSpacing: CGFloat

The distance in points between the bottom of one line fragment and the top of the next.

var minimumScaleFactor: CGFloat

The minimum permissible proportion to shrink the font size to fit the text into the available space.

var multilineTextAlignment: TextAlignment

An environment value that indicates how a text view aligns its lines when the content wraps or contains newlines.

var textCase: Text.Case?

A stylistic override to transform the case of `Text` when displayed, using the environment’s locale.

var truncationMode: Text.TruncationMode

A value that indicates how the layout truncates the last line of text to fit into the available space.

var textSelectionAffinity: TextSelectionAffinity

A representation of the direction or association of a selection or cursor relative to a text character. This concept becomes much more prominent when dealing with bidirectional text (text that contains both LTR and RTL scripts, like English and Arabic combined).

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

var physicalMetrics: PhysicalMetricsConverter

The physical metrics associated with a scene.

var realityKitScene: Scene?

var realityViewCameraControls: CameraControls

The camera controls for the reality view.

var redactionReasons: RedactionReasons

The current redaction reasons applied to the view hierarchy.

var springLoadingBehavior: SpringLoadingBehavior

The behavior of spring loaded interactions for the views associated with this environment.

var symbolRenderingMode: SymbolRenderingMode?

The current symbol rendering mode, or `nil` denoting that the mode is picked automatically using the current image and foreground style as parameters.

var symbolVariants: SymbolVariants

The symbol variant to use in this environment.

var worldTrackingLimitations: Set&lt;WorldTrackingLimitation>

The current limitations of the device tracking the user’s surroundings.

### Widgets

var showsWidgetContainerBackground: Bool

An environment variable that indicates whether the background of a widget appears.

var showsWidgetLabel: Bool

A Boolean value that indicates whether an accessory family widget can display an accessory label.

var widgetFamily: WidgetFamily

The template of the widget — small, medium, or large.

var widgetRenderingMode: WidgetRenderingMode

The widget’s rendering mode, based on where the system is displaying it.

var widgetContentMargins: EdgeInsets

A property that identifies the content margins of a widget.

### Deprecated environment values

var disableAutocorrection: Bool?

A Boolean value that determines whether the view hierarchy has auto-correction enabled.

Deprecated

var sizeCategory: ContentSizeCategory

The size of content.

Deprecated

var presentationMode: Binding&lt;PresentationMode>

A binding to the current presentation mode of the view associated with this environment.

Deprecated

struct PresentationMode

An indication whether a view is currently presented by another view.

Deprecated

var complicationRenderingMode: ComplicationRenderingMode

The complication rendering mode for the current environment.

Deprecated

var controlActiveState: ControlActiveState

The active appearance expected of controls in a window.

Deprecated

### Instance Properties

var activityFamily: ActivityFamily

The size family of the current Live Activity.

var credentialExportManager: ASCredentialExportManager

This environment variable is for SwiftUI clients of the credential exchange API. An example usage might look like:

var credentialImportManager: ASCredentialImportManager

This environment variable is for SwiftUI clients of the credential exchange API. An example usage might look like:

var devicePickerSupports: DevicePickerSupportedAction

Checks for support to present a DevicePicker.

var imagePlaygroundAllowedGenerationStyles: [ImagePlaygroundStyle]

var imagePlaygroundPersonalizationPolicy: ImagePlaygroundPersonalizationPolicy

var imagePlaygroundSelectedGenerationStyle: ImagePlaygroundStyle

var isActivityUpdateReduced: Bool

A Boolean value that indicates whether the Live Activity update synchronization rate is reduced.

var isUserAuthenticationEnabled: Bool

The current system user authentication enablement status.

var supportedActivityFamilies: Set&lt;ActivityFamily>

An environment value that that indicates potential rendered family for a Live Activity.

var supportsImagePlayground: Bool

A Boolean value that indicates whether image generation is available on the current device.

var tabBarPlacement: TabBarPlacement?

The current placement of the tab bar.

## Relationships

### Conforms To

- CustomStringConvertible

## See Also

### Accessing environment values

struct Environment

A property wrapper that reads a value from a view’s environment.

