

- SwiftUI
- View fundamentals
- View
-  Input and event modifiers 

API Collection

# Input and event modifiers

Supply actions for a view to perform in response to user input and system events.

## Overview

Use input and event modifiers to configure and provide handlers for a wide variety of user inputs or system events. For example, you can detect and control focus, respond to life cycle events like view appearance and disappearance, manage keyboard shortcuts, and much more.

## Topics

### Interactivity

func disabled(Bool) -> some View

Adds a condition that controls whether users can interact with this view.

func interactionActivityTrackingTag(String) -> some View

Sets a tag that you use for tracking interactivity.

### List controls

func swipeActions&lt;T>(edge: HorizontalEdge, allowsFullSwipe: Bool, content: () -> T) -> some View

Adds custom swipe actions to a row in a list.

func refreshable(action: () async -> Void) -> some View

Marks this view as refreshable.

func selectionDisabled(Bool) -> some View

Adds a condition that controls whether users can select this view.

### Scroll controls

func scrollPosition(Binding&lt;ScrollPosition>, anchor: UnitPoint?) -> some View

Associates a binding to a scroll position with a scroll view within this view.

func scrollPosition(id: Binding&lt;(some Hashable)?>, anchor: UnitPoint?) -> some View

Associates a binding to be updated when a scroll view within this view scrolls.

func defaultScrollAnchor(UnitPoint?) -> some View

Associates an anchor to control which part of the scroll view’s content should be rendered by default.

func defaultScrollAnchor(UnitPoint?, for: ScrollAnchorRole) -> some View

Associates an anchor to control the position of a scroll view in a particular circumstance.

func scrollTargetBehavior(some ScrollTargetBehavior) -> some View

Sets the scroll behavior of views scrollable in the provided axes.

func scrollTargetLayout(isEnabled: Bool) -> some View

Configures the outermost layout as a scroll target layout.

func scrollTransition(ScrollTransitionConfiguration, axis: Axis?, transition: (EmptyVisualEffect, ScrollTransitionPhase) -> some VisualEffect) -> some View

Applies the given transition, animating between the phases of the transition as this view appears and disappears within the visible region of the containing scroll view, or other container specified using the `coordinateSpace` parameter.

func scrollTransition(topLeading: ScrollTransitionConfiguration, bottomTrailing: ScrollTransitionConfiguration, axis: Axis?, transition: (EmptyVisualEffect, ScrollTransitionPhase) -> some VisualEffect) -> some View

Applies the given transition, animating between the phases of the transition as this view appears and disappears within the visible region of the containing scroll view, or other container specified using the `coordinateSpace` parameter.

func onScrollGeometryChange&lt;T>(for: T.Type, of: (ScrollGeometry) -> T, action: (T, T) -> Void) -> some View

Adds an action to be performed when a value, created from a scroll geometry, changes.

func onScrollTargetVisibilityChange&lt;ID>(idType: ID.Type, threshold: Double, ([ID]) -> Void) -> some View

Adds an action to be called with information about what views would be considered visible.

func onScrollVisibilityChange(threshold: Double, (Bool) -> Void) -> some View

Adds an action to be called when the view crosses the threshold to be considered on/off screen.

func onScrollPhaseChange(_:)

Adds an action to perform when the scroll phase of the first scroll view in the hierarchy changes.

### Geometry

func onGeometryChange(for:of:action:)

Adds an action to be performed when a value, created from a geometry proxy, changes.

### Taps and gestures

For more information, see Gestures.

func onTapGesture(count: Int, perform: () -> Void) -> some View

Adds an action to perform when this view recognizes a tap gesture.

func onTapGesture(count:coordinateSpace:perform:)

Adds an action to perform when this view recognizes a tap gesture, and provides the action with the location of the interaction.

func onLongPressGesture(minimumDuration: Double, maximumDistance: CGFloat, perform: () -> Void, onPressingChanged: ((Bool) -> Void)?) -> some View

Adds an action to perform when this view recognizes a long press gesture.

func onLongPressGesture(minimumDuration: Double, perform: () -> Void, onPressingChanged: ((Bool) -> Void)?) -> some View

Adds an action to perform when this view recognizes a long press gesture.

func onLongTouchGesture(minimumDuration: Double, perform: () -> Void, onTouchingChanged: ((Bool) -> Void)?) -> some View

Adds an action to perform when this view recognizes a remote long touch gesture. A long touch gesture is when the finger is on the remote touch surface without actually pressing.

func gesture(some UIGestureRecognizerRepresentable) -> some View

Attaches a UIGestureRecognizerRepresentable to the view.

func gesture&lt;T>(T, isEnabled: Bool) -> some View

Attaches a gesture to the view with a lower precedence than gestures defined by the view.

func gesture&lt;T>(T, name: String, isEnabled: Bool) -> some View

Attaches a gesture to the view with a lower precedence than gestures defined by the view.

func gesture&lt;T>(T, including: GestureMask) -> some View

Attaches a gesture to the view with a lower precedence than gestures defined by the view.

func highPriorityGesture&lt;T>(T, including: GestureMask) -> some View

Attaches a gesture to the view with a higher precedence than gestures defined by the view.

func highPriorityGesture&lt;T>(T, isEnabled: Bool) -> some View

Attaches a gesture to the view with a higher precedence than gestures defined by the view.

func highPriorityGesture&lt;T>(T, name: String, isEnabled: Bool) -> some View

Attaches a gesture to the view with a higher precedence than gestures defined by the view.

func simultaneousGesture&lt;T>(T, including: GestureMask) -> some View

Attaches a gesture to the view to process simultaneously with gestures defined by the view.

func simultaneousGesture&lt;T>(T, isEnabled: Bool) -> some View

Attaches a gesture to the view to process simultaneously with gestures defined by the view.

func simultaneousGesture&lt;T>(T, name: String, isEnabled: Bool) -> some View

Attaches a gesture to the view to process simultaneously with gestures defined by the view.

func defersSystemGestures(on: Edge.Set) -> some View

Sets the screen edge from which you want your gesture to take precedence over the system gesture.

func onPencilDoubleTap(perform: (PencilDoubleTapGestureValue) -> Void) -> some View

Adds an action to perform after the user double-taps their Apple Pencil.

func onPencilSqueeze(perform: (PencilSqueezeGesturePhase) -> Void) -> some View

Adds an action to perform when the user squeezes their Apple Pencil.

func allowsWindowActivationEvents(Bool?) -> some View

Configures whether gestures in this view hierarchy can handle events that activate the containing window.

### Keyboard input

func onKeyPress(KeyEquivalent, action: () -> KeyPress.Result) -> some View

Performs an action if the user presses a key on a hardware keyboard while the view has focus.

func onKeyPress(phases: KeyPress.Phases, action: (KeyPress) -> KeyPress.Result) -> some View

Performs an action if the user presses any key on a hardware keyboard while the view has focus.

func onKeyPress(KeyEquivalent, phases: KeyPress.Phases, action: (KeyPress) -> KeyPress.Result) -> some View

Performs an action if the user presses a key on a hardware keyboard while the view has focus.

func onKeyPress(characters: CharacterSet, phases: KeyPress.Phases, action: (KeyPress) -> KeyPress.Result) -> some View

Performs an action if the user presses one or more keys on a hardware keyboard while the view has focus.

func onKeyPress(keys: Set&lt;KeyEquivalent>, phases: KeyPress.Phases, action: (KeyPress) -> KeyPress.Result) -> some View

Performs an action if the user presses one or more keys on a hardware keyboard while the view has focus.

func onModifierKeysChanged(mask: EventModifiers, initial: Bool, (EventModifiers, EventModifiers) -> Void) -> some View

Performs an action whenever the user presses or releases a hardware modifier key.

### Keyboard shortcuts

func keyboardShortcut(_:)

Assigns a keyboard shortcut to the modified control.

func keyboardShortcut(KeyEquivalent, modifiers: EventModifiers) -> some View

Defines a keyboard shortcut and assigns it to the modified control.

func keyboardShortcut(KeyEquivalent, modifiers: EventModifiers, localization: KeyboardShortcut.Localization) -> some View

Defines a keyboard shortcut and assigns it to the modified control.

func modifierKeyAlternate&lt;V>(EventModifiers, () -> V) -> some View

Builds a view to use in place of the modified view when the user presses the modifier key(s) indicated by the given set.

### Hover

func onHover(perform: (Bool) -> Void) -> some View

Adds an action to perform when the user moves the pointer over or away from the view’s frame.

func onContinuousHover(coordinateSpace:perform:)

Adds an action to perform when the pointer enters, moves within, and exits the view’s bounds.

func hoverEffect(HoverEffect) -> some View

Applies a hover effect to this view.

func hoverEffect(_:isEnabled:)

Applies a hover effect to this view.

func hoverEffect(some CustomHoverEffect, in: HoverEffectGroup?, isEnabled: Bool) -> some View

Applies a hover effect to this view, optionally adding it to a HoverEffectGroup.

func hoverEffect(in: HoverEffectGroup?, isEnabled: Bool, body: (EmptyHoverEffectContent, Bool, GeometryProxy) -> some HoverEffectContent) -> some View

Applies a hover effect to this view described by the given closure.

func hoverEffectGroup() -> some View

Adds an implicit HoverEffectGroup to all effects defined on descendant views, so that all effects added to subviews activate as a group whenever this view or any descendant views are hovered.

func hoverEffectGroup(HoverEffectGroup?) -> some View

Adds a HoverEffectGroup to all effects defined on descendant views, and activates the group whenever this view or any descendant views are hovered.

func hoverEffectGroup(id: String?, in: Namespace.ID, behavior: HoverEffectGroup.Behavior) -> some View

Adds a HoverEffectGroup to all effects defined on descendant views, and activates the group whenever this view or any descendant views are hovered.

func hoverEffectDisabled(Bool) -> some View

Adds a condition that controls whether this view can display hover effects.

func defaultHoverEffect(_:)

Sets the default hover effect to use for views within this view.

func listRowHoverEffect(HoverEffect?) -> some View

Requests that the containing list row use the provided hover effect.

func listRowHoverEffectDisabled(Bool) -> some View

Requests that the containing list row have its hover effect disabled.

### Pointer

func pointerVisibility(Visibility) -> some View

Sets the visibility of the pointer when it’s over the view.

func pointerStyle(PointerStyle?) -> some View

Sets the pointer style to display when the pointer is over the view.

### Focus

For more information, see Focus.

func focused&lt;Value>(FocusState&lt;Value>.Binding, equals: Value) -> some View

Modifies this view by binding its focus state to the given state value.

func focused(FocusState&lt;Bool>.Binding) -> some View

Modifies this view by binding its focus state to the given Boolean state value.

func focusedValue&lt;T>(T?) -> some View

Sets the focused value for the given object type.

func focusedValue(_:_:)

Modifies this view by injecting a value that you provide for use by other views whose state depends on the focused view hierarchy.

func focusedSceneValue&lt;T>(T?) -> some View

Sets the focused value for the given object type at a scene-wide scope.

func focusedSceneValue(_:_:)

Modifies this view by injecting a value that you provide for use by other views whose state depends on the focused scene.

func focusedObject(_:)

Creates a new view that exposes the provided object to other views whose whose state depends on the focused view hierarchy.

func focusedSceneObject(_:)

Creates a new view that exposes the provided object to other views whose whose state depends on the active scene.

func prefersDefaultFocus(Bool, in: Namespace.ID) -> some View

Indicates that the view should receive focus by default for a given namespace.

func focusScope(Namespace.ID) -> some View

Creates a focus scope that SwiftUI uses to limit default focus preferences.

func focusSection() -> some View

Indicates that the view’s frame and cohort of focusable descendants should be used to guide focus movement.

func focusable(Bool) -> some View

Specifies if the view is focusable.

func focusable(Bool, interactions: FocusInteractions) -> some View

Specifies if the view is focusable, and if so, what focus-driven interactions it supports.

func focusEffectDisabled(Bool) -> some View

Adds a condition that controls whether this view can display focus effects, such as a default focus ring or hover effect.

func defaultFocus&lt;V>(FocusState&lt;V>.Binding, V, priority: DefaultFocusEvaluationPriority) -> some View

Defines a region of the window in which default focus is evaluated by assigning a value to a given focus state binding.

func searchFocused(FocusState&lt;Bool>.Binding) -> some View

Modifies this view by binding the focus state of the search field associated with the nearest searchable modifier to the given Boolean value.

func searchFocused&lt;V>(FocusState&lt;V>.Binding, equals: V) -> some View

Modifies this view by binding the focus state of the search field associated with the nearest searchable modifier to the given value.

### Copy and paste

For more information, see Clipboard.

func copyable&lt;T>(@autoclosure () -> [T]) -> some View

Specifies a list of items to copy in response to the system’s Copy command.

func cuttable&lt;T>(for: T.Type, action: () -> [T]) -> some View

Specifies an action that moves items to the Clipboard in response to the system’s Cut command.

func pasteDestination&lt;T>(for: T.Type, action: ([T]) -> Void, validator: ([T]) -> [T]) -> some View

Specifies an action that adds validated items to a view in response to the system’s Paste command.

func onCopyCommand(perform: (() -> [NSItemProvider])?) -> some View

Adds an action to perform in response to the system’s Copy command.

func onCutCommand(perform: (() -> [NSItemProvider])?) -> some View

Adds an action to perform in response to the system’s Cut command.

func onPasteCommand(of:perform:)

Adds an action to perform in response to the system’s Paste command.

func onPasteCommand(of:validator:perform:)

Adds an action to perform in response to the system’s Paste command with items that you validate.

### Drag and drop

For more information, see Drag and drop.

func onDrag&lt;V>(() -> NSItemProvider, preview: () -> V) -> some View

Activates this view as the source of a drag and drop operation.

func onDrag(() -> NSItemProvider) -> some View

Activates this view as the source of a drag and drop operation.

func itemProvider(Optional&lt;() -> NSItemProvider?>) -> some View

Provides a closure that vends the drag representation to be used for a particular data element.

func onDrop(of:isTargeted:perform:)

Defines the destination of a drag-and-drop operation that handles the dropped content with a closure that you specify.

func onDrop(of:delegate:)

Defines the destination of a drag and drop operation using behavior controlled by the delegate that you provide.

func dropDestination&lt;T>(for: T.Type, action: ([T], CGPoint) -> Bool, isTargeted: (Bool) -> Void) -> some View

Defines the destination of a drag and drop operation that handles the dropped content with a closure that you specify.

func draggable&lt;T>(@autoclosure () -> T) -> some View

Activates this view as the source of a drag and drop operation.

func draggable&lt;V, T>(@autoclosure () -> T, preview: () -> V) -> some View

Activates this view as the source of a drag and drop operation.

func springLoadingBehavior(SpringLoadingBehavior) -> some View

Sets the spring loading behavior this view.

### Submission

func onSubmit(of: SubmitTriggers, () -> Void) -> some View

Adds an action to perform when the user submits a value to this view.

func submitScope(Bool) -> some View

Prevents submission triggers originating from this view to invoke a submission action configured by a submission modifier higher up in the view hierarchy.

func submitLabel(SubmitLabel) -> some View

Sets the submit label for this view.

### Movement

func onMoveCommand(perform: ((MoveCommandDirection) -> Void)?) -> some View

Adds an action to perform in response to a move command, like when the user presses an arrow key on a Mac keyboard, or taps the edge of the Siri Remote when controlling an Apple TV.

func moveDisabled(Bool) -> some View

Adds a condition for whether the view’s view hierarchy is movable.

### Deletion

func onDeleteCommand(perform: (() -> Void)?) -> some View

Adds an action to perform in response to the system’s Delete command, or pressing either the ⌫ (backspace) or ⌦ (forward delete) keys while the view has focus.

func deleteDisabled(Bool) -> some View

Adds a condition for whether the view’s view hierarchy is deletable.

### Commands

func pageCommand&lt;V>(value: Binding&lt;V>, in: ClosedRange&lt;V>, step: V) -> some View

Steps a value through a range in response to page up or page down commands.

func onExitCommand(perform: (() -> Void)?) -> some View

Sets up an action that triggers in response to receiving the exit command while the view has focus.

func onPlayPauseCommand(perform: (() -> Void)?) -> some View

Adds an action to perform in response to the system’s Play/Pause command.

func onCommand(Selector, perform: (() -> Void)?) -> some View

Adds an action to perform in response to the given selector.

### Digital crown

func digitalCrownAccessory(Visibility) -> some View

Specifies the visibility of Digital Crown accessory Views on Apple Watch.

func digitalCrownAccessory&lt;Content>(content: () -> Content) -> some View

Places an accessory View next to the Digital Crown on Apple Watch.

func digitalCrownRotation&lt;V>(Binding&lt;V>, from: V, through: V, sensitivity: DigitalCrownRotationalSensitivity, isContinuous: Bool, isHapticFeedbackEnabled: Bool, onChange: (DigitalCrownEvent) -> Void, onIdle: () -> Void) -> some View

Tracks Digital Crown rotations by updating the specified binding.

func digitalCrownRotation&lt;V>(Binding&lt;V>, onChange: (DigitalCrownEvent) -> Void, onIdle: () -> Void) -> some View

Tracks Digital Crown rotations by updating the specified binding.

func digitalCrownRotation(detent:from:through:by:sensitivity:isContinuous:isHapticFeedbackEnabled:onChange:onIdle:)

Tracks Digital Crown rotations by updating the specified binding.

func digitalCrownRotation&lt;V>(Binding&lt;V>) -> some View

Tracks Digital Crown rotations by updating the specified binding.

func digitalCrownRotation&lt;V>(Binding&lt;V>, from: V, through: V, by: V.Stride?, sensitivity: DigitalCrownRotationalSensitivity, isContinuous: Bool, isHapticFeedbackEnabled: Bool) -> some View

Tracks Digital Crown rotations by updating the specified binding.

### Immersive Spaces

For more information, see Immersive spaces.

func onImmersionChange(initial: Bool, (ImmersionChangeContext, ImmersionChangeContext) -> Void) -> some View

Performs an action when the immersion state of your app changes.

### Volumes

func onVolumeViewpointChange(updateStrategy: VolumeViewpointUpdateStrategy, initial: Bool, (Viewpoint3D, Viewpoint3D) -> Void) -> some View

Adds an action to perform when the viewpoint of the volume changes.

func supportedVolumeViewpoints(SquareAzimuth.Set) -> some View

Specifies which viewpoints are supported for the window bar and ornaments in a volume.

### User activities

func userActivity&lt;P>(String, element: P?, (P, NSUserActivity) -> ()) -> some View

Advertises a user activity type.

func userActivity(String, isActive: Bool, (NSUserActivity) -> ()) -> some View

Advertises a user activity type.

func onContinueUserActivity(String, perform: (NSUserActivity) -> ()) -> some View

Registers a handler to invoke in response to a user activity that your app receives.

func handlesExternalEvents(preferring: Set&lt;String>, allowing: Set&lt;String>) -> some View

Specifies the external events that the view’s scene handles if the scene is already open.

### View life cycle

func onAppear(perform: (() -> Void)?) -> some View

Adds an action to perform before this view appears.

func onDisappear(perform: (() -> Void)?) -> some View

Adds an action to perform after this view disappears.

func onChange(of:initial:_:)

Adds a modifier for this view that fires an action when a specific value changes.

func task(priority: TaskPriority, () async -> Void) -> some View

Adds an asynchronous task to perform before this view appears.

func task&lt;T>(id: T, priority: TaskPriority, () async -> Void) -> some View

Adds a task to perform before this view appears or when a specified value changes.

### File renaming

func renameAction(_:)

Sets a closure to run for the rename action.

### URLs

func onOpenURL(perform: (URL) -> ()) -> some View

Registers a handler to invoke in response to a URL that your app receives.

func widgetURL(URL?) -> some View

Sets the URL to open in the containing app when the user clicks the widget.

### Publisher events

func onReceive&lt;P>(P, perform: (P.Output) -> Void) -> some View

Adds an action to perform when this view detects data emitted by the given publisher.

### Hit testing

func allowsHitTesting(Bool) -> some View

Configures whether this view participates in hit test operations.

### Content shape

func contentShape&lt;S>(S, eoFill: Bool) -> some View

Defines the content shape for hit testing.

func contentShape&lt;S>(ContentShapeKinds, S, eoFill: Bool) -> some View

Sets the content shape for this view.

### Import and export

func exportsItemProviders([UTType], onExport: () -> [NSItemProvider]) -> some View

Exports a read-only item provider for consumption by shortcuts, quick actions, and services.

func exportsItemProviders([UTType], onExport: () -> [NSItemProvider], onEdit: ([NSItemProvider]) -> Bool) -> some View

Exports a read-write item provider for consumption by shortcuts, quick actions, and services.

func importsItemProviders([UTType], onImport: ([NSItemProvider]) -> Bool) -> some View

Enables importing item providers from services, such as Continuity Camera on macOS.

func exportableToServices&lt;T>(@autoclosure () -> [T]) -> some View

Exports items for consumption by shortcuts, quick actions, and services.

func exportableToServices&lt;T>(@autoclosure () -> [T], onEdit: ([T]) -> Bool) -> some View

Exports read-write items for consumption by shortcuts, quick actions, and services.

func importableFromServices&lt;T>(for: T.Type, action: ([T]) -> Bool) -> some View

Enables importing items from services, such as Continuity Camera on macOS.

### App intents

func shortcutsLinkStyle(ShortcutsLinkStyle) -> some View

Sets the given style for ShortcutsLinks within the view hierarchy

func siriTipViewStyle(SiriTipViewStyle) -> some View

Sets the given style for SiriTipView within the view hierarchy

### Camera

func onCameraCaptureEvent(isEnabled: Bool, action: (AVCaptureEvent) -> Void) -> some View

Used to register an action triggered by system capture events.

func onCameraCaptureEvent(isEnabled: Bool, primaryAction: (AVCaptureEvent) -> Void, secondaryAction: (AVCaptureEvent) -> Void) -> some View

Used to register actions triggered by system capture events.

func cameraAnchor(isActive: Bool) -> some View

Specifies the view that should act as the virtual camera for Apple Vision Pro 2D Persona stream.

## See Also

### Providing interactivity

Search modifiers

Enable people to search for content in your app.

Presentation modifiers

Define additional views for the view to present under specified conditions.

State modifiers

Access storage and provide child views with configuration data.

