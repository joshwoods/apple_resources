

- SwiftUI
- View fundamentals
- View
-  Deprecated modifiers 

API Collection

# Deprecated modifiers

Review unsupported modifiers and their replacements.

## Overview

Avoid using deprecated modifiers in your app. Select a modifier to see the replacement that you should use instead.

## Topics

### Accessibility modifiers

func accessibility(label: Text) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds a label to the view that describes its contents.

Deprecated

func accessibility(value: Text) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds a textual description of the value that the view contains.

Deprecated

func accessibility(hidden: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Specifies whether to hide this view from system accessibility features.

Deprecated

func accessibility(identifier: String) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Uses the specified string to identify the view.

Deprecated

func accessibility(selectionIdentifier: AnyHashable) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets a selection identifier for this view’s accessibility element.

Deprecated

func accessibility(hint: Text) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Communicates to the user what happens after performing the view’s action.

Deprecated

func accessibility(activationPoint:)

Specifies the point where activations occur in the view.

Deprecated

func accessibility(inputLabels: [Text]) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets alternate input labels with which users identify a view.

Deprecated

func accessibility(addTraits: AccessibilityTraits) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds the given traits to the view.

Deprecated

func accessibility(removeTraits: AccessibilityTraits) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Removes the given traits from this view.

Deprecated

func accessibility(sortPriority: Double) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets the sort priority order for this view’s accessibility element, relative to other elements at the same level.

Deprecated

### Appearance modifiers

func colorScheme(ColorScheme) -> some View

Sets this view’s color scheme.

Deprecated

func listRowPlatterColor(Color?) -> some View

Sets the color that the system applies to the row background when this view is placed in a list.

Deprecated

func background&lt;Background>(Background, alignment: Alignment) -> some View

Layers the given view behind this view.

Deprecated

func overlay&lt;Overlay>(Overlay, alignment: Alignment) -> some View

Layers a secondary view in front of this view.

Deprecated

func foregroundColor(Color?) -> some View

Sets the color of the foreground elements displayed by this view.

Deprecated

func complicationForeground() -> some View

Promotes this view to the foreground in a complication.

Deprecated

### Text modifiers

func autocapitalization(UITextAutocapitalizationType) -> some View

Sets whether to apply auto-capitalization to this view.

Deprecated

func disableAutocorrection(Bool?) -> some View

Sets whether to disable autocorrection for this view.

Deprecated

### Auxiliary view modifiers

func navigationBarTitle(_:)

Sets the title in the navigation bar for this view.

Deprecated

func navigationBarTitle(_:displayMode:)

Sets the title and display mode in the navigation bar for this view.

Deprecated

func navigationBarItems&lt;L>(leading: L) -> some View

Sets the navigation bar items for this view.

Deprecated

func navigationBarItems&lt;L, T>(leading: L, trailing: T) -> some View

Sets the navigation bar items for this view.

Deprecated

func navigationBarItems&lt;T>(trailing: T) -> some View

Configures the navigation bar items for this view.

Deprecated

func navigationBarHidden(Bool) -> some View

Hides the navigation bar for this view.

Deprecated

func statusBar(hidden: Bool) -> some View

Sets the visibility of the status bar.

Deprecated

func contextMenu&lt;MenuItems>(ContextMenu&lt;MenuItems>?) -> some View

Adds a context menu to the view.

Deprecated

### Style modifiers

func menuButtonStyle&lt;S>(S) -> some View

Sets the style for menu buttons within this view.

Deprecated

func navigationViewStyle&lt;S>(S) -> some View

Sets the style for navigation views within this view.

Deprecated

### Layout modifiers

func frame() -> some View

Positions this view within an invisible frame.

Deprecated

func edgesIgnoringSafeArea(Edge.Set) -> some View

Changes the view’s proposed area to extend outside the screen’s safe areas.

Deprecated

func coordinateSpace&lt;T>(name: T) -> some View

Assigns a name to the view’s coordinate space, so other code can operate on dimensions like points and sizes relative to the named space.

Deprecated

### Graphics and rendering modifiers

func accentColor(Color?) -> some View

Sets the accent color for this view and the views it contains.

Deprecated

func mask&lt;Mask>(Mask) -> some View

Masks this view using the alpha channel of the given view.

Deprecated

func animation(Animation?) -> some View

Applies the given animation to all animatable values within this view.

Deprecated

func cornerRadius(CGFloat, antialiased: Bool) -> some View

Clips this view to its bounding frame, with the specified corner radius.

Deprecated

### Input and events modifiers

func onChange&lt;V>(of: V, perform: (V) -> Void) -> some View

Adds an action to perform when the given value changes.

Deprecated

func onTapGesture(count: Int, coordinateSpace: CoordinateSpace, perform: (CGPoint) -> Void) -> some View

Adds an action to perform when this view recognizes a tap gesture, and provides the action with the location of the interaction.

Deprecated

func onLongPressGesture(minimumDuration: Double, maximumDistance: CGFloat, pressing: ((Bool) -> Void)?, perform: () -> Void) -> some View

Adds an action to perform when this view recognizes a long press gesture.

Deprecated

func onLongPressGesture(minimumDuration: Double, pressing: ((Bool) -> Void)?, perform: () -> Void) -> some View

Adds an action to perform when this view recognizes a long press gesture.

Deprecated

func onPasteCommand(of: [String], perform: ([NSItemProvider]) -> Void) -> some View

Adds an action to perform in response to the system’s Paste command.

Deprecated

func onPasteCommand&lt;Payload>(of: [String], validator: ([NSItemProvider]) -> Payload?, perform: (Payload) -> Void) -> some View

Adds an action to perform in response to the system’s Paste command with items that you validate.

Deprecated

func onDrop(of: [String], delegate: any DropDelegate) -> some View

Defines the destination for a drag and drop operation with the same size and position as this view, with behavior controlled by the given delegate.

Deprecated

func onDrop(of:isTargeted:perform:)

Defines the destination of a drag-and-drop operation that handles the dropped content with a closure that you specify.

func focusable(Bool, onFocusChange: (Bool) -> Void) -> some View

Specifies if the view is focusable and, if so, adds an action to perform when the view comes into focus.

Deprecated

func onContinuousHover(coordinateSpace: CoordinateSpace, perform: (HoverPhase) -> Void) -> some View

Adds an action to perform when the pointer enters, moves within, and exits the view’s bounds.

Deprecated

### View presentation modifiers

func actionSheet(isPresented: Binding&lt;Bool>, content: () -> ActionSheet) -> some View

Presents an action sheet when a given condition is true.

Deprecated

func actionSheet&lt;T>(item: Binding&lt;T?>, content: (T) -> ActionSheet) -> some View

Presents an action sheet using the given item as a data source for the sheet’s content.

Deprecated

func alert(isPresented: Binding&lt;Bool>, content: () -> Alert) -> some View

Presents an alert to the user.

Deprecated

func alert&lt;Item>(item: Binding&lt;Item?>, content: (Item) -> Alert) -> some View

Presents an alert to the user.

Deprecated

### Search modifiers

func searchable(text:placement:prompt:suggestions:)

Marks this view as searchable, which configures the display of a search field.

Deprecated

### Tab modifiers

func tabItem&lt;V>(() -> V) -> some View

Sets the tab bar item associated with this view.

Deprecated

