

- SwiftUI
-  View 

Protocol

# View

A type that represents part of your app’s user interface and provides modifiers that you use to configure views.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
protocol View
```

## Mentioned in 

Declaring a custom view

Configuring views

Reducing view modifier maintenance

Performing a search operation

Migrating to the SwiftUI life cycle

## Overview

You create custom views by declaring types that conform to the `View` protocol. Implement the required body computed property to provide the content for your custom view.

```
struct MyView: View {
    var body: some View {
        Text("Hello, World!")
    }
}
```

Assemble the view’s body by combining one or more of the built-in views provided by SwiftUI, like the Text instance in the example above, plus other custom views that you define, into a hierarchy of views. For more information about creating custom views, see Declaring a custom view.

The `View` protocol provides a set of modifiers — protocol methods with default implementations — that you use to configure views in the layout of your app. Modifiers work by wrapping the view instance on which you call them in another view with the specified characteristics, as described in Configuring views. For example, adding the opacity(_:) modifier to a text view returns a new view with some amount of transparency:

```
Text("Hello, World!")
    .opacity(0.5) // Display partially transparent text.
```

The complete list of default modifiers provides a large set of controls for managing views. For example, you can fine tune Layout modifiers, add Accessibility modifiers information, and respond to Input and event modifiers. You can also collect groups of default modifiers into new, custom view modifiers for easy reuse.

A type conforming to this protocol inherits `@preconcurrency @MainActor` isolation from the protocol if the conformance is declared in its original declaration. Isolation to the main actor is the default, but it’s not required. Declare the conformance in an extension to opt-out the isolation.

## Topics

### Implementing a custom view

var body: Self.Body

The content and behavior of the view.

**Required** Default implementations provided.

associatedtype Body : View

The type of view representing the body of this view.

**Required**

func modifier&lt;T>(T) -> ModifiedContent&lt;Self, T>

Applies a modifier to a view and returns a new view.

Previews in Xcode

Generate dynamic, interactive previews of your custom views.

### Configuring view elements

Accessibility modifiers

Make your SwiftUI apps accessible to everyone, including people with disabilities.

Appearance modifiers

Configure a view’s foreground and background styles, controls, and visibility.

Text and symbol modifiers

Manage the rendering, selection, and entry of text in your view.

Auxiliary view modifiers

Add and configure supporting views, like toolbars and context menus.

Chart view modifiers

Configure charts that you declare with Swift Charts.

### Drawing views

Style modifiers

Apply built-in styles to different types of views.

Layout modifiers

Tell a view how to arrange itself within a view hierarchy by adjusting its size, position, alignment, padding, and so on.

Graphics and rendering modifiers

Affect the way the system draws a view, for example by scaling or masking a view, or by applying graphical effects.

### Providing interactivity

Input and event modifiers

Supply actions for a view to perform in response to user input and system events.

Search modifiers

Enable people to search for content in your app.

Presentation modifiers

Define additional views for the view to present under specified conditions.

State modifiers

Access storage and provide child views with configuration data.

### Deprecated modifiers

Deprecated modifiers

Review unsupported modifiers and their replacements.

### Instance Methods

func accessibilityActions&lt;Content>(category: AccessibilityActionCategory, () -> Content) -> some View

Adds multiple accessibility actions to the view with a specific category. Actions allow assistive technologies, such as VoiceOver, to interact with the view by invoking the action and are grouped by their category. When multiple action modifiers with an equal category are applied to the view, the actions are combined together.

func accessoryWidgetGroupStyle(AccessoryWidgetGroupStyle) -> some View

The view modifier that can be applied to `AccessoryWidgetGroup` to specify the shape the three content views will be masked with. The value of `style` is set to `.automatic`, which is `.circular` by default.

func addOrderToWalletButtonStyle(AddOrderToWalletButtonStyle) -> some View

Sets the button’s style.

func addPassToWalletButtonStyle(AddPassToWalletButtonStyle) -> some View

Sets the style to be used by the button. (see `PKAddPassButtonStyle`).

func automatedDeviceEnrollmentAddition(isPresented: Binding&lt;Bool>) -> some View

Presents a modal view that enables users to add devices to their organization.

func certificateSheet(trust: Binding&lt;SecTrust?>, title: String?, message: String?, help: URL?) -> some View

Displays a certificate sheet using the provided certificate trust.

func contactAccessButtonCaption(ContactAccessButton.Caption) -> some View

func contactAccessButtonStyle(ContactAccessButton.Style) -> some View

func contactAccessPicker(isPresented: Binding&lt;Bool>, completionHandler: ([String]) -> ()) -> some View

Modally present UI which allows the user to select which contacts your app has access to.

func containerValue&lt;V>(WritableKeyPath&lt;ContainerValues, V>, V) -> some View

Sets a particular container value of a view.

func contentToolbar(for:content:)

Populates the toolbar of the specified content view type with the views you provide.

func continuityDevicePicker(isPresented: Binding&lt;Bool>, onDidConnect: ((AVContinuityDevice?) -> Void)?) -> some View

A `continuityDevicePicker` should be used to discover and connect nearby continuity device through a button interface or other form of activation. On tvOS, this presents a fullscreen continuity device picker experience when selected. The modal view covers as much the screen of `self` as possible when a given condition is true.

func controlWidgetActionHint(_:)

The action hint of the control described by the modified label.

func controlWidgetStatus(_:)

The status of the control described by the modified label.

func currentEntitlementTask(for: String, priority: TaskPriority, action: (EntitlementTaskState&lt;VerificationResult&lt;Transaction>?>) async -> ()) -> some View

Declares the view as dependent on the entitlement of an In-App Purchase product, and returns a modified view.

func dialogPreventsAppTermination(Bool?) -> some View

Whether the alert or confirmation dialog prevents the app from being quit/terminated by the system or app termination menu item.

func documentBrowserContextMenu(([URL]?) -> some View) -> some View

Adds to a `DocumentLaunchView` actions that accept a list of selected files as their parameter.

func formStyle&lt;S>(S) -> some View

Sets the style for forms in a view hierarchy.

func glassBackgroundEffect&lt;S>(S, displayMode: GlassBackgroundDisplayMode) -> some View

Fills the view’s background with a custom glass background effect and container-relative rounded rectangle shape.

func glassBackgroundEffect&lt;T, S>(S, in: T, displayMode: GlassBackgroundDisplayMode) -> some View

Fills the view’s background with a custom glass background effect and a shape that you specify.

func handGestureShortcut(HandGestureShortcut, isEnabled: Bool) -> some View

Assigns a hand gesture shortcut to the modified control.

func handPointerBehavior(HandPointerBehavior?) -> some View

Sets the behavior of the hand pointer while the user is interacting with the view.

func handlesGameControllerEvents(matching: GCUIEventTypes) -> some View

Specifies the game controllers events which should be delivered through the GameController framework when the view, or one of its descendants has focus.

func healthDataAccessRequest(store: HKHealthStore, objectType: HKObjectType, predicate: NSPredicate?, trigger: some Equatable, completion: (Result&lt;Bool, any Error>) -> Void) -> some View

Asynchronously requests permission to read a data type that requires per-object authorization (such as vision prescriptions).

func healthDataAccessRequest(store: HKHealthStore, readTypes: Set&lt;HKObjectType>, trigger: some Equatable, completion: (Result&lt;Bool, any Error>) -> Void) -> some View

Requests permission to read the specified HealthKit data types.

func healthDataAccessRequest(store: HKHealthStore, shareTypes: Set&lt;HKSampleType>, readTypes: Set&lt;HKObjectType>?, trigger: some Equatable, completion: (Result&lt;Bool, any Error>) -> Void) -> some View

Requests permission to save and read the specified HealthKit data types.

func imagePlaygroundGenerationStyle(ImagePlaygroundStyle, in: [ImagePlaygroundStyle]) -> some View

Sets the generation style for an image playground.

func imagePlaygroundPersonalizationPolicy(ImagePlaygroundPersonalizationPolicy) -> some View

Policy determining whether to support the usage of people in the playground or not.

func imagePlaygroundSheet(isPresented: Binding&lt;Bool>, concept: String, sourceImage: Image?, onCompletion: (URL) -> Void, onCancellation: (() -> Void)?) -> some View

Presents the system sheet to create images from the specified input.

func imagePlaygroundSheet(isPresented: Binding&lt;Bool>, concept: String, sourceImageURL: URL, onCompletion: (URL) -> Void, onCancellation: (() -> Void)?) -> some View

Presents the system sheet to create images from the specified input.

func imagePlaygroundSheet(isPresented: Binding&lt;Bool>, concepts: [ImagePlaygroundConcept], sourceImage: Image?, onCompletion: (URL) -> Void, onCancellation: (() -> Void)?) -> some View

Presents the system sheet to create images from the specified input.

func imagePlaygroundSheet(isPresented: Binding&lt;Bool>, concepts: [ImagePlaygroundConcept], sourceImageURL: URL, onCompletion: (URL) -> Void, onCancellation: (() -> Void)?) -> some View

Presents the system sheet to create images from the specified input.

func immersiveEnvironmentPicker&lt;Content>(content: () -> Content) -> some View

Add menu items to open immersive spaces from a media player’s environment picker.

func inAppPurchaseOptions(((Product) async -> Set&lt;Product.PurchaseOption>)?) -> some View

Add a function to call before initiating a purchase from StoreKit view within this view, providing a set of options for the purchase.

func journalingSuggestionsPicker(isPresented: Binding&lt;Bool>, onCompletion: (JournalingSuggestion) async -> Void) -> some View

Presents a visual picker interface that contains events and images that a person can select to retrieve more information.

func labeledContentStyle&lt;S>(S) -> some View

Sets a style for labeled content.

func labelsVisibility(Visibility) -> some View

Controls the visibility of labels of any controls contained within this view.

func lookAroundViewer(isPresented: Binding&lt;Bool>, initialScene: MKLookAroundScene?, allowsNavigation: Bool, showsRoadLabels: Bool, pointsOfInterest: PointOfInterestCategories, onDismiss: (() -> Void)?) -> some View

func lookAroundViewer(isPresented: Binding&lt;Bool>, scene: Binding&lt;MKLookAroundScene?>, allowsNavigation: Bool, showsRoadLabels: Bool, pointsOfInterest: PointOfInterestCategories, onDismiss: (() -> Void)?) -> some View

func manageSubscriptionsSheet(isPresented: Binding&lt;Bool>, subscriptionGroupID: String) -> some View

func managedContentStyle(ManagedContentStyle) -> some View

Applies a managed content style to the view.

func mapCameraKeyframeAnimator(trigger: some Equatable, keyframes: (MapCamera) -> some Keyframes&lt;MapCamera>) -> some View

Uses the given keyframes to animate the camera of a `Map` when the given trigger value changes.

func mapControlVisibility(Visibility) -> some View

Configures all Map controls in the environment to have the specified visibility

func mapControls(() -> some View) -> some View

Configures all `Map` views in the associated environment to have standard size and position controls

func mapFeatureSelectionAccessory(MapItemDetailSelectionAccessoryStyle?) -> some View

Specifies the selection accessory to display for a `MapFeature`

func mapFeatureSelectionContent(content: (MapFeature) -> some MapContent) -> some View

Specifies a custom presentation for the currently selected feature.

func mapFeatureSelectionDisabled((MapFeature) -> Bool) -> some View

Specifies which map features should have selection disabled.

func mapItemDetailPopover(isPresented: Binding&lt;Bool>, item: MKMapItem?, displaysMap: Bool, attachmentAnchor: PopoverAttachmentAnchor) -> some View

Presents a map item detail popover.

func mapItemDetailPopover(isPresented: Binding&lt;Bool>, item: MKMapItem?, displaysMap: Bool, attachmentAnchor: PopoverAttachmentAnchor, arrowEdge: Edge) -> some View

Presents a map item detail popover.

func mapItemDetailPopover(item: Binding&lt;MKMapItem?>, displaysMap: Bool, attachmentAnchor: PopoverAttachmentAnchor) -> some View

Presents a map item detail popover.

func mapItemDetailPopover(item: Binding&lt;MKMapItem?>, displaysMap: Bool, attachmentAnchor: PopoverAttachmentAnchor, arrowEdge: Edge) -> some View

Presents a map item detail popover.

func mapItemDetailSheet(isPresented: Binding&lt;Bool>, item: MKMapItem?, displaysMap: Bool) -> some View

Presents a map item detail sheet.

func mapItemDetailSheet(item: Binding&lt;MKMapItem?>, displaysMap: Bool) -> some View

Presents a map item detail sheet.

func mapScope(Namespace.ID) -> some View

Creates a mapScope that SwiftUI uses to connect map controls to an associated map.

func mapStyle(MapStyle) -> some View

Specifies the map style to be used.

func matchedTransitionSource(id: some Hashable, in: Namespace.ID) -> some View

Identifies this view as the source of a navigation transition, such as a zoom transition.

func matchedTransitionSource(id: some Hashable, in: Namespace.ID, configuration: (EmptyMatchedTransitionSourceConfiguration) -> some MatchedTransitionSourceConfiguration) -> some View

Identifies this view as the source of a navigation transition, such as a zoom transition.

func materialActiveAppearance(MaterialActiveAppearance) -> some View

Sets an explicit active appearance for materials in this view.

func navigationTransition(some NavigationTransition) -> some View

Sets the navigation transition style for this view.

func onApplePayCouponCodeChange(perform: (String) async -> PKPaymentRequestCouponCodeUpdate) -> some View

Called when a user has entered or updated a coupon code. This is required if the user is being asked to provide a coupon code.

func onApplePayPaymentMethodChange(perform: (PKPaymentMethod) async -> PKPaymentRequestPaymentMethodUpdate) -> some View

Called when a payment method has changed and asks for an update payment request. If this modifier isn’t provided Wallet will assume the payment method is valid.

func onApplePayShippingContactChange(perform: (PKContact) async -> PKPaymentRequestShippingContactUpdate) -> some View

Called when a user selected a shipping address. This is required if the user is being asked to provide a shipping contact.

func onApplePayShippingMethodChange(perform: (PKShippingMethod) async -> PKPaymentRequestShippingMethodUpdate) -> some View

Called when a user selected a shipping method. This is required if the user is being asked to provide a shipping method.

func onGeometryChange3D(for:of:action:)

Returns a new view that arranges to call `action(value)` whenever the value computed by `transform(proxy)` changes, where `proxy` provides access to the view’s 3D geometry properties.

func onInAppPurchaseCompletion(perform: ((Product, Result&lt;Product.PurchaseResult, any Error>) async -> ())?) -> some View

Add an action to perform when a purchase initiated from a StoreKit view within this view completes.

func onInAppPurchaseStart(perform: ((Product) async -> ())?) -> some View

Add an action to perform when a user triggers the purchase button on a StoreKit view within this view.

func onMapCameraChange(frequency:_:)

Performs an action when Map camera framing changes

func payLaterViewAction(PayLaterViewAction) -> some View

Sets the action on the PayLaterView. See `PKPayLaterAction`.

func payLaterViewDisplayStyle(PayLaterViewDisplayStyle) -> some View

Sets the display style on the PayLaterView. See `PKPayLaterDisplayStyle`.

func payWithApplePayButtonStyle(PayWithApplePayButtonStyle) -> some View

Sets the style to be used by the button. (see `PayWithApplePayButtonStyle`).

func popoverTip((any Tip)?, arrowEdge: Edge?, action: (Tips.Action) -> Void) -> some View

Presents a popover tip on the modified view.

func preferredSubscriptionOffer((Product, Product.SubscriptionInfo, [Product.SubscriptionOffer]) -> Product.SubscriptionOffer?) -> some View

Selects a subscription offer to apply to a purchase that a customer makes from a subscription store view, a store view, or a product view.

func presentationPreventsAppTermination(Bool?) -> some View

Whether a presentation prevents the app from being terminated/quit by the system or app termination menu item.

func productDescription(Visibility) -> some View

Configure the visibility of labels displaying an in-app purchase product description within the view.

func productIconBorder() -> some View

Adds a standard border to an in-app purchase product’s icon .

func productViewStyle(some ProductViewStyle) -> some View

Sets the style for In-App Purchase product views within a view.

func realityViewCameraControls(CameraControls) -> some View

Adds gestures that control the position and direction of a virtual camera.

func scrollInputBehavior(ScrollInputBehavior, for: ScrollInputKind) -> some View

Enables or disables scrolling in scrollable views when using particular inputs.

func signInWithAppleButtonStyle(SignInWithAppleButton.Style) -> some View

Sets the style used for displaying the control (see `SignInWithAppleButton.Style`).

func storeButton(Visibility, for: StoreButtonKind...) -> some View

Specifies the visibility of auxiliary buttons that store view and subscription store view instances may use.

func storeProductTask(for: Product.ID, priority: TaskPriority, action: (Product.TaskState) async -> ()) -> some View

Declares the view as dependent on an In-App Purchase product and returns a modified view.

func storeProductsTask(for: some Collection&lt;String> &amp; Equatable &amp; Sendable, priority: TaskPriority, action: (Product.CollectionTaskState) async -> ()) -> some View

Declares the view as dependent on a collection of In-App Purchase products and returns a modified view.

func subscriptionPromotionalOffer(offer: (Product, Product.SubscriptionInfo) -> Product.SubscriptionOffer?, signature: (Product, Product.SubscriptionInfo, Product.SubscriptionOffer) async throws -> Product.SubscriptionOffer.Signature) -> some View

Selects a promotional offer to apply to a purchase a customer makes from a subscription store view.

func subscriptionStatusTask(for: String, priority: TaskPriority, action: (EntitlementTaskState&lt;[Product.SubscriptionInfo.Status]>) async -> ()) -> some View

Declares the view as dependent on the status of an auto-renewable subscription group, and returns a modified view.

func subscriptionStoreButtonLabel(SubscriptionStoreButtonLabel) -> some View

Configures subscription store view instances within a view to use the provided button label.

func subscriptionStoreControlBackground(_:)

Set a standard effect to use for the background of subscription store view controls within the view.

func subscriptionStoreControlIcon(icon: (Product, Product.SubscriptionInfo) -> some View) -> some View

Sets a view to use to decorate individual subscription options within a subscription store view.

func subscriptionStoreControlStyle(some SubscriptionStoreControlStyle) -> some View

Sets the control style for subscription store views within a view.

func subscriptionStoreControlStyle&lt;S>(S, placement: S.Placement) -> some View

Sets the control style and control placement for subscription store views within a view.

func subscriptionStoreOptionGroupStyle(some SubscriptionOptionGroupStyle) -> some View

Sets the style subscription store views within this view use to display groups of subscription options.

func subscriptionStorePickerItemBackground(some ShapeStyle) -> some View

Sets the background style for picker items of the subscription store view instances within a view.

func subscriptionStorePickerItemBackground(some ShapeStyle, in: some Shape) -> some View

Sets the background shape and style for subscription store view picker items within a view.

func subscriptionStorePolicyDestination(for: SubscriptionStorePolicyKind, destination: () -> some View) -> some View

Configures a view as the destination for a policy button action in subscription store views.

func subscriptionStorePolicyDestination(url: URL, for: SubscriptionStorePolicyKind) -> some View

Configures a URL as the destination for a policy button action in subscription store views.

func subscriptionStorePolicyForegroundStyle(some ShapeStyle) -> some View

Sets the style for the terms of service and privacy policy buttons within a subscription store view.

func subscriptionStorePolicyForegroundStyle(some ShapeStyle, some ShapeStyle) -> some View

Sets the primary and secondary style for the terms of service and privacy policy buttons within a subscription store view.

func subscriptionStoreSignInAction((() -> ())?) -> some View

Adds an action to perform when a person uses the sign-in button on a subscription store view within a view.

func tabletopGame(TabletopGame, parent: Entity, automaticUpdate: Bool) -> some View

Adds a tabletop game to a view.

func tabletopGame(TabletopGame, parent: Entity, automaticUpdate: Bool, interaction: (TabletopInteraction.Value) -> any TabletopInteraction.Delegate) -> some View

Supplies a closure which returns a new interaction whenever needed.

func textContentType(_:)

Sets the text content type for this view, which the system uses to offer suggestions while the user enters text on macOS.

func textRenderer&lt;T>(T) -> some View

Returns a new view such that any text views within it will use `renderer` to draw themselves.

func textSelectionAffinity(TextSelectionAffinity) -> some View

Sets the direction of a selection or cursor relative to a text character.

func tipBackground(some ShapeStyle) -> some View

Sets the tip’s view background to a style. Currently this only applies to inline tips, not popover tips.

func tipCornerRadius(CGFloat, antialiased: Bool) -> some View

Sets the corner radius for an inline tip view.

func tipImageSize(CGSize) -> some View

Sets the size for a tip’s image.

func tipImageStyle&lt;S>(S) -> some View

Sets the style for a tip’s image.

func tipImageStyle&lt;S1, S2>(S1, S2) -> some View

Sets the style for a tip’s image.

func tipImageStyle&lt;S1, S2, S3>(S1, S2, S3) -> some View

Sets the style for a tip’s image.

func tipViewStyle(some TipViewStyle) -> some View

Sets the given style for TipView within the view hierarchy.

func toolbarItemHidden(Bool) -> some View

Hides an individual view within a control group toolbar item.

func transactionPicker(isPresented: Binding&lt;Bool>, selection: Binding&lt;[Transaction]>) -> some View

Presents a picker that selects a collection of transactions.

func transactionTask(CredentialTransaction.Configuration?, action: (CredentialTransaction) async -> Void) -> some View

Provides a task to perform before this view appears

func translationPresentation(isPresented: Binding&lt;Bool>, text: String, attachmentAnchor: PopoverAttachmentAnchor, arrowEdge: Edge, replacementAction: ((String) -> Void)?) -> some View

Presents a translation popover when a given condition is true.

func translationTask(TranslationSession.Configuration?, action: (TranslationSession) async -> Void) -> some View

Adds a task to perform before this view appears or when the translation configuration changes.

func translationTask(source: Locale.Language?, target: Locale.Language?, action: (TranslationSession) async -> Void) -> some View

Adds a task to perform before this view appears or when the specified source or target languages change.

func verifyIdentityWithWalletButtonStyle(VerifyIdentityWithWalletButtonStyle) -> some View

Sets the style to be used by the button. (see `PKIdentityButtonStyle`).

func windowToolbarFullScreenVisibility(WindowToolbarFullScreenVisibility) -> some View

Configures the visibility of the window toolbar when the window enters full screen mode.

func workoutPreview(WorkoutPlan, isPresented: Binding&lt;Bool>) -> some View

Presents a preview of the workout contents as a modal sheet

func writingToolsAffordanceVisibility(Visibility) -> some View

Specifies whether the system should show the Writing Tools affordance for text input views affected by the environment.

func writingToolsBehavior(WritingToolsBehavior) -> some View

Specifies the Writing Tools behavior for text and text input in the environment.

## Relationships

### Inherited By

- DynamicViewContent
- InsettableShape
- NSViewControllerRepresentable
- NSViewRepresentable
- Shape
- ShapeView
- UIViewControllerRepresentable
- UIViewRepresentable
- WKInterfaceObjectRepresentable

### Conforming Types

- AngularGradient
- AnyShape
- AnyView
- AsyncImage
- Button
- ButtonBorderShape
- ButtonStyleConfiguration.Label
- Canvas

  Conforms when `Symbols` conforms to `View`.

- Capsule
- Circle
- Color
- ColorPicker
- ContainerRelativeShape
- ContentUnavailableView
- ControlGroup
- ControlGroupStyleConfiguration.Content
- ControlGroupStyleConfiguration.Label
- DatePicker
- DatePickerStyleConfiguration.Label
- DefaultDateProgressLabel
- DefaultDocumentGroupLaunchActions
- DefaultSettingsLinkLabel
- DefaultShareLinkLabel
- DefaultTabLabel
- DefaultWindowVisibilityToggleLabel
- DisclosureGroup
- DisclosureGroupStyleConfiguration.Content
- DisclosureGroupStyleConfiguration.Label
- Divider
- DocumentLaunchView
- EditButton
- EditableCollectionContent

  Conforms when `Content` conforms to `View`, `Data` conforms to `Copyable`, and `Data` conforms to `Escapable`.

- Ellipse
- EllipticalGradient
- EmptyView
- EquatableView
- FillShapeView
- ForEach

  Conforms when `Data` conforms to `RandomAccessCollection`, `ID` conforms to `Hashable`, and `Content` conforms to `View`.

- Form
- FormStyleConfiguration.Content
- Gauge
- GaugeStyleConfiguration.CurrentValueLabel
- GaugeStyleConfiguration.Label
- GaugeStyleConfiguration.MarkedValueLabel
- GaugeStyleConfiguration.MaximumValueLabel
- GaugeStyleConfiguration.MinimumValueLabel
- GeometryReader
- GeometryReader3D
- GlassBackgroundEffectConfiguration.Content
- Grid

  Conforms when `Content` conforms to `View`.

- GridRow

  Conforms when `Content` conforms to `View`.

- Group

  Conforms when `Content` conforms to `View`.

- GroupBox
- GroupBoxStyleConfiguration.Content
- GroupBoxStyleConfiguration.Label
- GroupElementsOfContent
- GroupSectionsOfContent
- HSplitView
- HStack
- HelpLink
- Image
- KeyframeAnimator
- Label
- LabelStyleConfiguration.Icon
- LabelStyleConfiguration.Title
- LabeledContent

  Conforms when `Label` conforms to `View` and `Content` conforms to `View`.

- LabeledContentStyleConfiguration.Content
- LabeledContentStyleConfiguration.Label
- LabeledControlGroupContent
- LabeledToolbarItemGroupContent
- LazyHGrid
- LazyHStack
- LazyVGrid
- LazyVStack
- LinearGradient
- Link
- List
- Menu
- MenuButton
- MenuStyleConfiguration.Content
- MenuStyleConfiguration.Label
- MeshGradient
- ModifiedContent

  Conforms when `Content` conforms to `View` and `Modifier` conforms to `ViewModifier`.

- MultiDatePicker
- NavigationLink
- NavigationSplitView
- NavigationStack
- NavigationView
- NewDocumentButton
- OffsetShape
- OutlineGroup

  Conforms when `Data` conforms to `RandomAccessCollection`, `ID` conforms to `Hashable`, `Parent` conforms to `View`, `Leaf` conforms to `View`, and `Subgroup` conforms to `View`.

- OutlineSubgroupChildren
- PasteButton
- Path
- PhaseAnimator
- Picker
- PlaceholderContentView
- PresentedWindowContent
- PreviewModifierContent
- PrimitiveButtonStyleConfiguration.Label
- ProgressView
- ProgressViewStyleConfiguration.CurrentValueLabel
- ProgressViewStyleConfiguration.Label
- RadialGradient
- Rectangle
- RenameButton
- RotatedShape

  Conforms when `Content` conforms to `InsettableShape`.

- RoundedRectangle
- ScaledShape
- ScrollView
- ScrollViewReader
- SearchUnavailableContent.Actions
- SearchUnavailableContent.Description
- SearchUnavailableContent.Label
- Section

  Conforms when `Parent` conforms to `View`, `Content` conforms to `View`, and `Footer` conforms to `View`.

- SecureField
- SettingsLink
- ShareLink
- Slider
- Spacer
- Stepper
- StrokeBorderShapeView
- StrokeShapeView
- SubscriptionView
- Subview
- SubviewsCollection
- SubviewsCollectionSlice
- TabContentBuilder.Content
- TabView
- Table
- Text
- TextEditor
- TextField
- TextFieldLink
- TimelineView

  Conforms when `Schedule` conforms to `TimelineSchedule` and `Content` conforms to `View`.

- Toggle
- ToggleStyleConfiguration.Label
- TransformedShape
- TupleView
- UnevenRoundedRectangle
- VSplitView
- VStack
- ViewThatFits
- WindowVisibilityToggle
- ZStack
- ZStackContent3D

  Conforms when `Content` conforms to `View`.

## See Also

### Creating a view

Declaring a custom view

Define views and assemble them into a view hierarchy.

struct ViewBuilder

A custom parameter attribute that constructs views from closures.

