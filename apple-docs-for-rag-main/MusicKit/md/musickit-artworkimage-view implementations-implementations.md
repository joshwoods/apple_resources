

- MusicKit
- ArtworkImage
-  View Implementations 

API Collection

# View Implementations

## Topics

### Instance Methods

func accentColor(Color?) -> some View

Sets the accent color for this view and the views it contains.

Deprecated

func accessibility(activationPoint: CGPoint) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Specifies the point where activations occur in the view.

Deprecated

func accessibility(activationPoint: UnitPoint) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Specifies the unit point where activations occur in the view.

Deprecated

func accessibility(addTraits: AccessibilityTraits) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds the given traits to the view.

Deprecated

func accessibility(hidden: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Specifies whether to hide this view from system accessibility features.

Deprecated

func accessibility(hint: Text) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Communicates to the user what happens after performing the view’s action.

Deprecated

func accessibility(identifier: String) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Uses the specified string to identify the view.

Deprecated

func accessibility(inputLabels: [Text]) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets alternate input labels with which users identify a view.

Deprecated

func accessibility(label: Text) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds a label to the view that describes its contents.

Deprecated

func accessibility(removeTraits: AccessibilityTraits) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Removes the given traits from this view.

Deprecated

func accessibility(selectionIdentifier: AnyHashable) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets a selection identifier for this view’s accessibility element.

Deprecated

func accessibility(sortPriority: Double) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets the sort priority order for this view’s accessibility element, relative to other elements at the same level.

Deprecated

func accessibility(value: Text) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds a textual description of the value that the view contains.

Deprecated

func accessibilityAction(AccessibilityActionKind, () -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

func accessibilityAction&lt;Label>(action: () -> Void, label: () -> Label) -> some View

Adds an accessibility action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

func accessibilityAction(named: LocalizedStringKey, () -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

func accessibilityAction(named: Text, () -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

func accessibilityAction&lt;S>(named: S, () -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

func accessibilityActions&lt;Content>(() -> Content) -> some View

Adds multiple accessibility actions to the view.

func accessibilityActions&lt;Content>(category: AccessibilityActionCategory, () -> Content) -> some View

Adds multiple accessibility actions to the view with a specific category. Actions allow assistive technologies, such as VoiceOver, to interact with the view by invoking the action and are grouped by their category. When multiple action modifiers with an equal category are applied to the view, the actions are combined together.

func accessibilityActivationPoint(UnitPoint) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

The activation point for an element is the location assistive technologies use to initiate gestures.

func accessibilityActivationPoint(CGPoint) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

The activation point for an element is the location assistive technologies use to initiate gestures.

func accessibilityActivationPoint(UnitPoint, isEnabled: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

The activation point for an element is the location assistive technologies use to initiate gestures.

func accessibilityActivationPoint(CGPoint, isEnabled: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

The activation point for an element is the location assistive technologies use to initiate gestures.

func accessibilityAddTraits(AccessibilityTraits) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds the given traits to the view.

func accessibilityAdjustableAction((AccessibilityAdjustmentDirection) -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility adjustable action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

func accessibilityChartDescriptor&lt;R>(R) -> some View

Adds a descriptor to a View that represents a chart to make the chart’s contents accessible to all users.

func accessibilityChildren&lt;V>(children: () -> V) -> some View

Replaces the existing accessibility element’s children with one or more new synthetic accessibility elements.

func accessibilityCustomContent(Text, Text, importance: AXCustomContent.Importance) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Add additional accessibility information to the view.

func accessibilityCustomContent(AccessibilityCustomContentKey, LocalizedStringKey, importance: AXCustomContent.Importance) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Add additional accessibility information to the view.

func accessibilityCustomContent(AccessibilityCustomContentKey, Text?, importance: AXCustomContent.Importance) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Add additional accessibility information to the view.

func accessibilityCustomContent&lt;L, V>(L, V, importance: AXCustomContent.Importance) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Add additional accessibility information to the view.

Deprecated

func accessibilityCustomContent&lt;V>(AccessibilityCustomContentKey, V, importance: AXCustomContent.Importance) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Add additional accessibility information to the view.

func accessibilityCustomContent(LocalizedStringKey, Text, importance: AXCustomContent.Importance) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Add additional accessibility information to the view.

func accessibilityCustomContent&lt;V>(LocalizedStringKey, V, importance: AXCustomContent.Importance) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Add additional accessibility information to the view.

func accessibilityCustomContent(LocalizedStringKey, LocalizedStringKey, importance: AXCustomContent.Importance) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Add additional accessibility information to the view.

func accessibilityDirectTouch(Bool, options: AccessibilityDirectTouchOptions) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Explicitly set whether this accessibility element is a direct touch area. Direct touch areas passthrough touch events to the app rather than being handled through an assistive technology, such as VoiceOver. The modifier accepts an optional `AccessibilityDirectTouchOptions` option set to customize the functionality of the direct touch area.

func accessibilityDragPoint(UnitPoint, description: LocalizedStringKey) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

The point an assistive technology should use to begin a drag interaction.

func accessibilityDragPoint&lt;S>(UnitPoint, description: S) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

The point an assistive technology should use to begin a drag interaction.

func accessibilityDragPoint(UnitPoint, description: Text) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

The point an assistive technology should use to begin a drag interaction.

func accessibilityDragPoint&lt;S>(UnitPoint, description: S, isEnabled: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

The point an assistive technology should use to begin a drag interaction.

func accessibilityDragPoint(UnitPoint, description: Text, isEnabled: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

The point an assistive technology should use to begin a drag interaction.

func accessibilityDragPoint(UnitPoint, description: LocalizedStringKey, isEnabled: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

The point an assistive technology should use to begin a drag interaction.

func accessibilityDropPoint&lt;S>(UnitPoint, description: S) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

The point an assistive technology should use to end a drag interaction.

func accessibilityDropPoint(UnitPoint, description: Text) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

The point an assistive technology should use to end a drag interaction.

func accessibilityDropPoint(UnitPoint, description: LocalizedStringKey) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

The point an assistive technology should use to end a drag interaction.

func accessibilityDropPoint(UnitPoint, description: Text, isEnabled: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

The point an assistive technology should use to end a drag interaction.

func accessibilityDropPoint&lt;S>(UnitPoint, description: S, isEnabled: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

The point an assistive technology should use to end a drag interaction.

func accessibilityDropPoint(UnitPoint, description: LocalizedStringKey, isEnabled: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

The point an assistive technology should use to end a drag interaction.

func accessibilityElement(children: AccessibilityChildBehavior) -> some View

Creates a new accessibility element, or modifies the `AccessibilityChildBehavior` of the existing accessibility element.

func accessibilityFocused(AccessibilityFocusState&lt;Bool>.Binding) -> some View

Modifies this view by binding its accessibility element’s focus state to the given boolean state value.

func accessibilityFocused&lt;Value>(AccessibilityFocusState&lt;Value>.Binding, equals: Value) -> some View

Modifies this view by binding its accessibility element’s focus state to the given state value.

func accessibilityHeading(AccessibilityHeadingLevel) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets the accessibility level of this heading.

func accessibilityHidden(Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Specifies whether to hide this view from system accessibility features.

func accessibilityHidden(Bool, isEnabled: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Specifies whether to hide this view from system accessibility features.

func accessibilityHint(Text) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Communicates to the user what happens after performing the view’s action.

func accessibilityHint&lt;S>(S) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Communicates to the user what happens after performing the view’s action.

func accessibilityHint(LocalizedStringKey) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Communicates to the user what happens after performing the view’s action.

func accessibilityHint&lt;S>(S, isEnabled: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Communicates to the user what happens after performing the view’s action.

func accessibilityHint(LocalizedStringKey, isEnabled: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Communicates to the user what happens after performing the view’s action.

func accessibilityHint(Text, isEnabled: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Communicates to the user what happens after performing the view’s action.

func accessibilityIdentifier(String) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Uses the string you specify to identify the view.

func accessibilityIdentifier(String, isEnabled: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Uses the string you specify to identify the view.

func accessibilityIgnoresInvertColors(Bool) -> some View

Sets whether this view should ignore the system Smart Invert setting.

func accessibilityInputLabels&lt;S>([S]) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets alternate input labels with which users identify a view.

func accessibilityInputLabels([LocalizedStringKey]) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets alternate input labels with which users identify a view.

func accessibilityInputLabels([Text]) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets alternate input labels with which users identify a view.

func accessibilityInputLabels([LocalizedStringKey], isEnabled: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets alternate input labels with which users identify a view.

func accessibilityInputLabels&lt;S>([S], isEnabled: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets alternate input labels with which users identify a view.

func accessibilityInputLabels([Text], isEnabled: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets alternate input labels with which users identify a view.

func accessibilityLabel(Text) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds a label to the view that describes its contents.

func accessibilityLabel(LocalizedStringKey) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds a label to the view that describes its contents.

func accessibilityLabel&lt;S>(S) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds a label to the view that describes its contents.

func accessibilityLabel(Text, isEnabled: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds a label to the view that describes its contents.

func accessibilityLabel(LocalizedStringKey, isEnabled: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds a label to the view that describes its contents.

func accessibilityLabel&lt;S>(S, isEnabled: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds a label to the view that describes its contents.

func accessibilityLabel&lt;V>(content: (PlaceholderContentView&lt;Self>) -> V) -> some View

Adds a label to the view that describes its contents.

func accessibilityLabeledPair&lt;ID>(role: AccessibilityLabeledPairRole, id: ID, in: Namespace.ID) -> some View

Pairs an accessibility element representing a label with the element for the matching content.

func accessibilityLinkedGroup&lt;ID>(id: ID, in: Namespace.ID) -> some View

Links multiple accessibility elements so that the user can quickly navigate from one element to another, even when the elements are not near each other in the accessibility hierarchy.

func accessibilityQuickAction&lt;Style, Content>(style: Style, content: () -> Content) -> some View

Adds a quick action to be shown by the system when active.

func accessibilityQuickAction&lt;Style, Content>(style: Style, isActive: Binding&lt;Bool>, content: () -> Content) -> some View

Adds a quick action to be shown by the system when active.

func accessibilityRemoveTraits(AccessibilityTraits) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Removes the given traits from this view.

func accessibilityRepresentation&lt;V>(representation: () -> V) -> some View

Replaces one or more accessibility elements for this view with new accessibility elements.

func accessibilityRespondsToUserInteraction(Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Explicitly set whether this Accessibility element responds to user interaction and would thus be interacted with by technologies such as Switch Control, Voice Control or Full Keyboard Access.

func accessibilityRespondsToUserInteraction(Bool, isEnabled: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Explicitly set whether this Accessibility element responds to user interaction and would thus be interacted with by technologies such as Switch Control, Voice Control or Full Keyboard Access.

func accessibilityRotor&lt;Content>(AccessibilitySystemRotor, entries: () -> Content) -> some View

Create an Accessibility Rotor replacing the specified system-provided Rotor.

func accessibilityRotor&lt;L, Content>(L, entries: () -> Content) -> some View

Create an Accessibility Rotor with the specified user-visible label, and entries generated from the content closure.

func accessibilityRotor&lt;Content>(Text, entries: () -> Content) -> some View

Create an Accessibility Rotor with the specified user-visible label, and entries generated from the content closure.

func accessibilityRotor&lt;Content>(LocalizedStringKey, entries: () -> Content) -> some View

Create an Accessibility Rotor with the specified user-visible label, and entries generated from the content closure.

func accessibilityRotor&lt;EntryModel, ID>(Text, entries: [EntryModel], entryID: KeyPath&lt;EntryModel, ID>, entryLabel: KeyPath&lt;EntryModel, String>) -> some View

Create an Accessibility Rotor with the specified user-visible label and entries.

func accessibilityRotor&lt;EntryModel, ID>(LocalizedStringKey, entries: [EntryModel], entryID: KeyPath&lt;EntryModel, ID>, entryLabel: KeyPath&lt;EntryModel, String>) -> some View

Create an Accessibility Rotor with the specified user-visible label and entries.

func accessibilityRotor&lt;L, EntryModel, ID>(L, entries: [EntryModel], entryID: KeyPath&lt;EntryModel, ID>, entryLabel: KeyPath&lt;EntryModel, String>) -> some View

Create an Accessibility Rotor with the specified user-visible label and entries.

func accessibilityRotor&lt;EntryModel, ID>(AccessibilitySystemRotor, entries: [EntryModel], entryID: KeyPath&lt;EntryModel, ID>, entryLabel: KeyPath&lt;EntryModel, String>) -> some View

Create an Accessibility Rotor replacing the specified system-provided Rotor.

func accessibilityRotor&lt;EntryModel>(AccessibilitySystemRotor, entries: [EntryModel], entryLabel: KeyPath&lt;EntryModel, String>) -> some View

Create an Accessibility Rotor replacing the specified system-provided Rotor.

func accessibilityRotor&lt;EntryModel>(Text, entries: [EntryModel], entryLabel: KeyPath&lt;EntryModel, String>) -> some View

Create an Accessibility Rotor with the specified user-visible label and entries.

func accessibilityRotor&lt;EntryModel>(LocalizedStringKey, entries: [EntryModel], entryLabel: KeyPath&lt;EntryModel, String>) -> some View

Create an Accessibility Rotor with the specified user-visible label and entries.

func accessibilityRotor&lt;L, EntryModel>(L, entries: [EntryModel], entryLabel: KeyPath&lt;EntryModel, String>) -> some View

Create an Accessibility Rotor with the specified user-visible label and entries.

func accessibilityRotor(AccessibilitySystemRotor, textRanges: [Range&lt;String.Index>]) -> some View

Create an Accessibility Rotor replacing the specified system-provided Rotor. The Rotor will be attached to the current Accessibility element, and each entry will go the specified range of that element.

func accessibilityRotor(LocalizedStringKey, textRanges: [Range&lt;String.Index>]) -> some View

Create an Accessibility Rotor with the specified user-visible label and entries for each of the specified ranges. The Rotor will be attached to the current Accessibility element, and each entry will go the specified range of that element.

func accessibilityRotor&lt;L>(L, textRanges: [Range&lt;String.Index>]) -> some View

Create an Accessibility Rotor with the specified user-visible label and entries for each of the specified ranges. The Rotor will be attached to the current Accessibility element, and each entry will go the specified range of that element.

func accessibilityRotor(Text, textRanges: [Range&lt;String.Index>]) -> some View

Create an Accessibility Rotor with the specified user-visible label and entries for each of the specified ranges. The Rotor will be attached to the current Accessibility element, and each entry will go the specified range of that element.

func accessibilityRotorEntry&lt;ID>(id: ID, in: Namespace.ID) -> some View

Defines an explicit identifier tying an Accessibility element for this view to an entry in an Accessibility Rotor.

func accessibilityScrollAction((Edge) -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility scroll action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

func accessibilityShowsLargeContentViewer() -> some View

Adds a default large content view to be shown by the large content viewer.

func accessibilityShowsLargeContentViewer&lt;V>(() -> V) -> some View

Adds a custom large content view to be shown by the large content viewer.

func accessibilitySortPriority(Double) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets the sort priority order for this view’s accessibility element, relative to other elements at the same level.

func accessibilityTextContentType(AccessibilityTextContentType) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets an accessibility text content type.

func accessibilityValue(LocalizedStringKey) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds a textual description of the value that the view contains.

func accessibilityValue(Text) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds a textual description of the value that the view contains.

func accessibilityValue&lt;S>(S) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds a textual description of the value that the view contains.

func accessibilityValue(LocalizedStringKey, isEnabled: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds a textual description of the value that the view contains.

func accessibilityValue(Text, isEnabled: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds a textual description of the value that the view contains.

func accessibilityValue&lt;S>(S, isEnabled: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds a textual description of the value that the view contains.

func accessibilityZoomAction((AccessibilityZoomGestureAction) -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility zoom action to the view. Actions allow assistive technologies, such as VoiceOver, to interact with the view by invoking the action.

func actionSheet(isPresented: Binding&lt;Bool>, content: () -> ActionSheet) -> some View

Presents an action sheet when a given condition is true.

Deprecated

func actionSheet&lt;T>(item: Binding&lt;T?>, content: (T) -> ActionSheet) -> some View

Presents an action sheet using the given item as a data source for the sheet’s content.

Deprecated

func alert&lt;A>(Text, isPresented: Binding&lt;Bool>, actions: () -> A) -> some View

Presents an alert when a given condition is true, using a text view for the title.

func alert&lt;S, A>(S, isPresented: Binding&lt;Bool>, actions: () -> A) -> some View

Presents an alert when a given condition is true, using a string variable as a title.

func alert&lt;A>(LocalizedStringKey, isPresented: Binding&lt;Bool>, actions: () -> A) -> some View

Presents an alert when a given condition is true, using a localized string key for the title.

func alert&lt;A, M>(LocalizedStringKey, isPresented: Binding&lt;Bool>, actions: () -> A, message: () -> M) -> some View

Presents an alert with a message when a given condition is true, using a localized string key for a title.

func alert&lt;S, A, M>(S, isPresented: Binding&lt;Bool>, actions: () -> A, message: () -> M) -> some View

Presents an alert with a message when a given condition is true using a string variable as a title.

func alert&lt;A, M>(Text, isPresented: Binding&lt;Bool>, actions: () -> A, message: () -> M) -> some View

Presents an alert with a message when a given condition is true using a text view as a title.

func alert&lt;A, T>(Text, isPresented: Binding&lt;Bool>, presenting: T?, actions: (T) -> A) -> some View

Presents an alert using the given data to produce the alert’s content and a text view as a title.

func alert&lt;S, A, T>(S, isPresented: Binding&lt;Bool>, presenting: T?, actions: (T) -> A) -> some View

Presents an alert using the given data to produce the alert’s content and a string variable as a title.

func alert&lt;A, T>(LocalizedStringKey, isPresented: Binding&lt;Bool>, presenting: T?, actions: (T) -> A) -> some View

Presents an alert using the given data to produce the alert’s content and a localized string key for a title.

func alert&lt;S, A, M, T>(S, isPresented: Binding&lt;Bool>, presenting: T?, actions: (T) -> A, message: (T) -> M) -> some View

Presents an alert with a message using the given data to produce the alert’s content and a string variable as a title.

func alert&lt;A, M, T>(LocalizedStringKey, isPresented: Binding&lt;Bool>, presenting: T?, actions: (T) -> A, message: (T) -> M) -> some View

Presents an alert with a message using the given data to produce the alert’s content and a localized string key for a title.

func alert&lt;A, M, T>(Text, isPresented: Binding&lt;Bool>, presenting: T?, actions: (T) -> A, message: (T) -> M) -> some View

Presents an alert with a message using the given data to produce the alert’s content and a text view for a title.

func alert(isPresented: Binding&lt;Bool>, content: () -> Alert) -> some View

Presents an alert to the user.

Deprecated

func alert&lt;E, A>(isPresented: Binding&lt;Bool>, error: E?, actions: () -> A) -> some View

Presents an alert when an error is present.

func alert&lt;E, A, M>(isPresented: Binding&lt;Bool>, error: E?, actions: (E) -> A, message: (E) -> M) -> some View

Presents an alert with a message when an error is present.

func alert&lt;Item>(item: Binding&lt;Item?>, content: (Item) -> Alert) -> some View

Presents an alert to the user.

Deprecated

func alignmentGuide(VerticalAlignment, computeValue: (ViewDimensions) -> CGFloat) -> some View

Sets the view’s vertical alignment.

func alignmentGuide(HorizontalAlignment, computeValue: (ViewDimensions) -> CGFloat) -> some View

Sets the view’s horizontal alignment.

func allowedDynamicRange(Image.DynamicRange?) -> some View

Returns a new view configured with the specified allowed dynamic range.

func allowsHitTesting(Bool) -> some View

Configures whether this view participates in hit test operations.

func allowsTightening(Bool) -> some View

Sets whether text in this view can compress the space between characters when necessary to fit text in a line.

func allowsWindowActivationEvents(Bool?) -> some View

Configures whether gestures in this view hierarchy can handle events that activate the containing window.

func alternatingRowBackgrounds(AlternatingRowBackgroundBehavior) -> some View

Overrides whether lists and tables in this view have alternating row backgrounds.

func anchorPreference&lt;A, K>(key: K.Type, value: Anchor&lt;A>.Source, transform: (Anchor&lt;A>) -> K.Value) -> some View

Sets a value for the specified preference key, the value is a function of a geometry value tied to the current coordinate space, allowing readers of the value to convert the geometry to their local coordinates.

func animation(Animation?) -> some View

Applies the given animation to all animatable values within this view.

Deprecated

func animation&lt;V>(Animation?, body: (PlaceholderContentView&lt;Self>) -> V) -> some View

Applies the given animation to all animatable values within the `body` closure.

func animation&lt;V>(Animation?, value: V) -> some View

Applies the given animation to this view when the specified value changes.

func aspectRatio(CGSize, contentMode: ContentMode) -> some View

Constrains this view’s dimensions to the aspect ratio of the given size.

func aspectRatio(CGFloat?, contentMode: ContentMode) -> some View

Constrains this view’s dimensions to the specified aspect ratio.

func autocapitalization(UITextAutocapitalizationType) -> some View

Sets whether to apply auto-capitalization to this view.

Deprecated

func autocorrectionDisabled(Bool) -> some View

Sets whether to disable autocorrection for this view.

func background&lt;Background>(Background, alignment: Alignment) -> some View

Layers the given view behind this view.

Deprecated

func background&lt;S>(S, ignoresSafeAreaEdges: Edge.Set) -> some View

Sets the view’s background to a style.

func background&lt;S, T>(S, in: T, fillStyle: FillStyle) -> some View

Sets the view’s background to an insettable shape filled with a style.

func background&lt;S, T>(S, in: T, fillStyle: FillStyle) -> some View

Sets the view’s background to a shape filled with a style.

func background&lt;V>(alignment: Alignment, content: () -> V) -> some View

Layers the views that you specify behind this view.

func background(ignoresSafeAreaEdges: Edge.Set) -> some View

Sets the view’s background to the default background style.

func background&lt;S>(in: S, fillStyle: FillStyle) -> some View

Sets the view’s background to an insettable shape filled with the default background style.

func background&lt;S>(in: S, fillStyle: FillStyle) -> some View

Sets the view’s background to a shape filled with the default background style.

func backgroundPreferenceValue&lt;Key, T>(Key.Type, (Key.Value) -> T) -> some View

Reads the specified preference value from the view, using it to produce a second view that is applied as the background of the original view.

func backgroundPreferenceValue&lt;K, V>(K.Type, alignment: Alignment, (K.Value) -> V) -> some View

Reads the specified preference value from the view, using it to produce a second view that is applied as the background of the original view.

func backgroundStyle&lt;S>(S) -> some View

Sets the specified style to render backgrounds within the view.

func badge(Text?) -> some View

Generates a badge for the view from a text view.

func badge(Int) -> some View

Generates a badge for the view from an integer value.

func badge&lt;S>(S?) -> some View

Generates a badge for the view from a string.

func badge(LocalizedStringKey?) -> some View

Generates a badge for the view from a localized string key.

func badgeProminence(BadgeProminence) -> some View

Specifies the prominence of badges created by this view.

func baselineOffset(CGFloat) -> some View

Sets the vertical offset for the text relative to its baseline in this view.

func blendMode(BlendMode) -> some View

Sets the blend mode for compositing this view with overlapping views.

func blur(radius: CGFloat, opaque: Bool) -> some View

Applies a Gaussian blur to this view.

func bold(Bool) -> some View

Applies a bold font weight to the text in this view.

func border&lt;S>(S, width: CGFloat) -> some View

Adds a border to this view with the specified style and width.

func brightness(Double) -> some View

Brightens this view by the specified amount.

func buttonBorderShape(ButtonBorderShape) -> some View

Sets the border shape for buttons in this view.

func buttonRepeatBehavior(ButtonRepeatBehavior) -> some View

Sets whether buttons in this view should repeatedly trigger their actions on prolonged interactions.

func buttonStyle&lt;S>(S) -> some View

Sets the style for buttons within this view to a button style with a custom appearance and custom interaction behavior.

func buttonStyle&lt;S>(S) -> some View

Sets the style for buttons within this view to a button style with a custom appearance and standard interaction behavior.

func clipShape&lt;S>(S, style: FillStyle) -> some View

Sets a clipping shape for this view.

func clipped(antialiased: Bool) -> some View

Clips this view to its bounding rectangular frame.

func colorEffect(Shader, isEnabled: Bool) -> some View

Returns a new view that applies `shader` to `self` as a filter effect on the color of each pixel.

func colorInvert() -> some View

Inverts the colors in this view.

func colorMultiply(Color) -> some View

Adds a color multiplication effect to this view.

func colorScheme(ColorScheme) -> some View

Sets this view’s color scheme.

Deprecated

func compositingGroup() -> some View

Wraps this view in a compositing group.

func confirmationDialog&lt;S, A>(S, isPresented: Binding&lt;Bool>, titleVisibility: Visibility, actions: () -> A) -> some View

Presents a confirmation dialog when a given condition is true, using a string variable as a title.

func confirmationDialog&lt;A>(Text, isPresented: Binding&lt;Bool>, titleVisibility: Visibility, actions: () -> A) -> some View

Presents a confirmation dialog when a given condition is true, using a text view for the title.

func confirmationDialog&lt;A>(LocalizedStringKey, isPresented: Binding&lt;Bool>, titleVisibility: Visibility, actions: () -> A) -> some View

Presents a confirmation dialog when a given condition is true, using a localized string key for the title.

func confirmationDialog&lt;A, M>(LocalizedStringKey, isPresented: Binding&lt;Bool>, titleVisibility: Visibility, actions: () -> A, message: () -> M) -> some View

Presents a confirmation dialog with a message when a given condition is true, using a localized string key for the title.

func confirmationDialog&lt;S, A, M>(S, isPresented: Binding&lt;Bool>, titleVisibility: Visibility, actions: () -> A, message: () -> M) -> some View

Presents a confirmation dialog with a message when a given condition is true, using a string variable for the title.

func confirmationDialog&lt;A, M>(Text, isPresented: Binding&lt;Bool>, titleVisibility: Visibility, actions: () -> A, message: () -> M) -> some View

Presents a confirmation dialog with a message when a given condition is true, using a text view for the title.

func confirmationDialog&lt;A, T>(Text, isPresented: Binding&lt;Bool>, titleVisibility: Visibility, presenting: T?, actions: (T) -> A) -> some View

Presents a confirmation dialog using data to produce the dialog’s content and a text view for the title.

func confirmationDialog&lt;S, A, T>(S, isPresented: Binding&lt;Bool>, titleVisibility: Visibility, presenting: T?, actions: (T) -> A) -> some View

Presents a confirmation dialog using data to produce the dialog’s content and a string variable for the title.

func confirmationDialog&lt;A, T>(LocalizedStringKey, isPresented: Binding&lt;Bool>, titleVisibility: Visibility, presenting: T?, actions: (T) -> A) -> some View

Presents a confirmation dialog using data to produce the dialog’s content and a localized string key for the title.

func confirmationDialog&lt;A, M, T>(LocalizedStringKey, isPresented: Binding&lt;Bool>, titleVisibility: Visibility, presenting: T?, actions: (T) -> A, message: (T) -> M) -> some View

Presents a confirmation dialog with a message using data to produce the dialog’s content and a localized string key for the title.

func confirmationDialog&lt;S, A, M, T>(S, isPresented: Binding&lt;Bool>, titleVisibility: Visibility, presenting: T?, actions: (T) -> A, message: (T) -> M) -> some View

Presents a confirmation dialog with a message using data to produce the dialog’s content and a string variable for the title.

func confirmationDialog&lt;A, M, T>(Text, isPresented: Binding&lt;Bool>, titleVisibility: Visibility, presenting: T?, actions: (T) -> A, message: (T) -> M) -> some View

Presents a confirmation dialog with a message using data to produce the dialog’s content and a text view for the message.

func containerBackground&lt;S>(S, for: ContainerBackgroundPlacement) -> some View

Sets the container background of the enclosing container using a view.

func containerBackground&lt;V>(for: ContainerBackgroundPlacement, alignment: Alignment, content: () -> V) -> some View

Sets the container background of the enclosing container using a view.

func containerRelativeFrame(Axis.Set, alignment: Alignment) -> some View

Positions this view within an invisible frame with a size relative to the nearest container.

func containerRelativeFrame(Axis.Set, alignment: Alignment, (CGFloat, Axis) -> CGFloat) -> some View

Positions this view within an invisible frame with a size relative to the nearest container.

func containerRelativeFrame(Axis.Set, count: Int, span: Int, spacing: CGFloat, alignment: Alignment) -> some View

Positions this view within an invisible frame with a size relative to the nearest container.

func containerShape&lt;T>(T) -> some View

Sets the container shape to use for any container relative shape within this view.

func containerValue&lt;V>(WritableKeyPath&lt;ContainerValues, V>, V) -> some View

Sets a particular container value of a view.

func contentMargins(Edge.Set, EdgeInsets, for: ContentMarginPlacement) -> some View

Configures the content margin for a provided placement.

func contentMargins(Edge.Set, CGFloat?, for: ContentMarginPlacement) -> some View

Configures the content margin for a provided placement.

func contentMargins(CGFloat, for: ContentMarginPlacement) -> some View

Configures the content margin for a provided placement.

func contentShape&lt;S>(ContentShapeKinds, S, eoFill: Bool) -> some View

Sets the content shape for this view.

func contentShape&lt;S>(S, eoFill: Bool) -> some View

Defines the content shape for hit testing.

func contentToolbar&lt;Content>(for: ContentToolbarPlacement, content: () -> Content) -> some View

Populates the toolbar of the specified content view type with the views you provide.

func contentToolbar&lt;Content>(for: ContentToolbarPlacement, content: () -> Content) -> some View

Populates the toolbar of the specified content view type with the views you provide.

func contentTransition(ContentTransition) -> some View

Modifies the view to use a given transition as its method of animating changes to the contents of its views.

func contextMenu&lt;MenuItems>(ContextMenu&lt;MenuItems>?) -> some View

Adds a context menu to the view.

Deprecated

func contextMenu&lt;I, M>(forSelectionType: I.Type, menu: (Set&lt;I>) -> M, primaryAction: ((Set&lt;I>) -> Void)?) -> some View

Adds an item-based context menu to a view.

func contextMenu&lt;MenuItems>(menuItems: () -> MenuItems) -> some View

Adds a context menu to a view.

func contextMenu&lt;M, P>(menuItems: () -> M, preview: () -> P) -> some View

Adds a context menu with a custom preview to a view.

func contrast(Double) -> some View

Sets the contrast and separation between similar colors in this view.

func controlGroupStyle&lt;S>(S) -> some View

Sets the style for control groups within this view.

func controlSize(ControlSize) -> some View

Sets the size for controls within this view.

func coordinateSpace(NamedCoordinateSpace) -> some View

Assigns a name to the view’s coordinate space, so other code can operate on dimensions like points and sizes relative to the named space.

func coordinateSpace&lt;T>(name: T) -> some View

Assigns a name to the view’s coordinate space, so other code can operate on dimensions like points and sizes relative to the named space.

Deprecated

func copyable&lt;T>(@autoclosure () -> [T]) -> some View

Specifies a list of items to copy in response to the system’s Copy command.

func cornerRadius(CGFloat, antialiased: Bool) -> some View

Clips this view to its bounding frame, with the specified corner radius.

Deprecated

func cuttable&lt;T>(for: T.Type, action: () -> [T]) -> some View

Specifies an action that moves items to the Clipboard in response to the system’s Cut command.

func datePickerStyle&lt;S>(S) -> some View

Sets the style for date pickers within this view.

func defaultAdaptableTabBarPlacement(AdaptableTabBarPlacement) -> some View

Specifies the default placement for the tabs in a tab view using the adaptable sidebar style.

func defaultAppStorage(UserDefaults) -> some View

The default store used by `AppStorage` contained within the view.

func defaultFocus&lt;V>(FocusState&lt;V>.Binding, V, priority: DefaultFocusEvaluationPriority) -> some View

Defines a region of the window in which default focus is evaluated by assigning a value to a given focus state binding.

func defaultHoverEffect(HoverEffect?) -> some View

Sets the default hover effect to use for views within this view.

func defaultHoverEffect(some CustomHoverEffect) -> some View

Sets the default hover effect to use within this view hierarchy.

func defaultScrollAnchor(UnitPoint?) -> some View

Associates an anchor to control which part of the scroll view’s content should be rendered by default.

func defaultScrollAnchor(UnitPoint?, for: ScrollAnchorRole) -> some View

Associates an anchor to control the position of a scroll view in a particular circumstance.

func defaultWheelPickerItemHeight(CGFloat) -> some View

Sets the default wheel-style picker item height.

func defersSystemGestures(on: Edge.Set) -> some View

Sets the screen edge from which you want your gesture to take precedence over the system gesture.

func deleteDisabled(Bool) -> some View

Adds a condition for whether the view’s view hierarchy is deletable.

func dialogIcon(Image?) -> some View

Configures the icon used by dialogs within this view.

func dialogPreventsAppTermination(Bool?) -> some View

Whether the alert or confirmation dialog prevents the app from being quit/terminated by the system or app termination menu item.

func dialogSeverity(DialogSeverity) -> some View

func dialogSuppressionToggle(LocalizedStringKey, isSuppressed: Binding&lt;Bool>) -> some View

Enables user suppression of dialogs and alerts presented within `self`, with a custom suppression message on macOS. Unused on other platforms.

func dialogSuppressionToggle(Text, isSuppressed: Binding&lt;Bool>) -> some View

Enables user suppression of dialogs and alerts presented within `self`, with a custom suppression message on macOS. Unused on other platforms.

func dialogSuppressionToggle&lt;S>(S, isSuppressed: Binding&lt;Bool>) -> some View

Enables user suppression of dialogs and alerts presented within `self`, with a custom suppression message on macOS. Unused on other platforms.

func dialogSuppressionToggle(isSuppressed: Binding&lt;Bool>) -> some View

Enables user suppression of dialogs and alerts presented within `self`, with a default suppression message on macOS. Unused on other platforms.

func digitalCrownAccessory(Visibility) -> some View

Specifies the visibility of Digital Crown accessory Views on Apple Watch.

func digitalCrownAccessory&lt;Content>(content: () -> Content) -> some View

Places an accessory View next to the Digital Crown on Apple Watch.

func digitalCrownRotation&lt;V>(Binding&lt;V>) -> some View

Tracks Digital Crown rotations by updating the specified binding.

func digitalCrownRotation&lt;V>(Binding&lt;V>, from: V, through: V, by: V.Stride?, sensitivity: DigitalCrownRotationalSensitivity, isContinuous: Bool, isHapticFeedbackEnabled: Bool) -> some View

Tracks Digital Crown rotations by updating the specified binding.

func digitalCrownRotation&lt;V>(Binding&lt;V>, from: V, through: V, sensitivity: DigitalCrownRotationalSensitivity, isContinuous: Bool, isHapticFeedbackEnabled: Bool, onChange: (DigitalCrownEvent) -> Void, onIdle: () -> Void) -> some View

Tracks Digital Crown rotations by updating the specified binding.

func digitalCrownRotation&lt;V>(Binding&lt;V>, onChange: (DigitalCrownEvent) -> Void, onIdle: () -> Void) -> some View

Tracks Digital Crown rotations by updating the specified binding.

func digitalCrownRotation&lt;V>(detent: Binding&lt;V>, from: V, through: V, by: V.Stride, sensitivity: DigitalCrownRotationalSensitivity, isContinuous: Bool, isHapticFeedbackEnabled: Bool, onChange: (DigitalCrownEvent) -> Void, onIdle: () -> Void) -> some View

Tracks Digital Crown rotations by updating the specified binding.

func digitalCrownRotation&lt;V>(detent: Binding&lt;V>, from: V, through: V, by: V.Stride, sensitivity: DigitalCrownRotationalSensitivity, isContinuous: Bool, isHapticFeedbackEnabled: Bool, onChange: (DigitalCrownEvent) -> Void, onIdle: () -> Void) -> some View

Tracks Digital Crown rotations by updating the specified binding.

func disableAutocorrection(Bool?) -> some View

Sets whether to disable autocorrection for this view.

Deprecated

func disabled(Bool) -> some View

Adds a condition that controls whether users can interact with this view.

func disclosureGroupStyle&lt;S>(S) -> some View

Sets the style for disclosure groups within this view.

func dismissalConfirmationDialog&lt;S, A>(S, shouldPresent: Bool, actions: () -> A) -> some View

Presents a confirmation dialog when a dismiss action has been triggered.

func dismissalConfirmationDialog&lt;A>(LocalizedStringKey, shouldPresent: Bool, actions: () -> A) -> some View

Presents a confirmation dialog when a dismiss action has been triggered.

func dismissalConfirmationDialog&lt;A>(Text, shouldPresent: Bool, actions: () -> A) -> some View

Presents a confirmation dialog when a dismiss action has been triggered.

func dismissalConfirmationDialog&lt;S, A, M>(S, shouldPresent: Bool, actions: () -> A, message: () -> M) -> some View

Presents a confirmation dialog when a dismiss action has been triggered.

func dismissalConfirmationDialog&lt;A, M>(LocalizedStringKey, shouldPresent: Bool, actions: () -> A, message: () -> M) -> some View

Presents a confirmation dialog when a dismiss action has been triggered.

func dismissalConfirmationDialog&lt;A, M>(Text, shouldPresent: Bool, actions: () -> A, message: () -> M) -> some View

Presents a confirmation dialog when a dismiss action has been triggered.

func distortionEffect(Shader, maxSampleOffset: CGSize, isEnabled: Bool) -> some View

Returns a new view that applies `shader` to `self` as a geometric distortion effect on the location of each pixel.

func documentBrowserContextMenu(([URL]?) -> some View) -> some View

Adds to a `DocumentLaunchView` actions that accept a list of selected files as their parameter.

func draggable&lt;T>(@autoclosure () -> T) -> some View

Activates this view as the source of a drag and drop operation.

func draggable&lt;V, T>(@autoclosure () -> T, preview: () -> V) -> some View

Activates this view as the source of a drag and drop operation.

func drawingGroup(opaque: Bool, colorMode: ColorRenderingMode) -> some View

Composites this view’s contents into an offscreen image before final display.

func dropDestination&lt;T>(for: T.Type, action: ([T], CGPoint) -> Bool, isTargeted: (Bool) -> Void) -> some View

Defines the destination of a drag and drop operation that handles the dropped content with a closure that you specify.

func dynamicTypeSize(DynamicTypeSize) -> some View

Sets the Dynamic Type size within the view to the given value.

func dynamicTypeSize&lt;T>(T) -> some View

Limits the Dynamic Type size within the view to the given range.

func edgesIgnoringSafeArea(Edge.Set) -> some View

Changes the view’s proposed area to extend outside the screen’s safe areas.

Deprecated

func environment&lt;T>(T?) -> some View

Places an observable object in the view’s environment.

func environment&lt;V>(WritableKeyPath&lt;EnvironmentValues, V>, V) -> some View

Sets the environment value of the specified key path to the given value.

func environmentObject&lt;T>(T) -> some View

Supplies an observable object to a view’s hierarchy.

func exportableToServices&lt;T>(@autoclosure () -> [T]) -> some View

Exports items for consumption by shortcuts, quick actions, and services.

func exportableToServices&lt;T>(@autoclosure () -> [T], onEdit: ([T]) -> Bool) -> some View

Exports read-write items for consumption by shortcuts, quick actions, and services.

func exportsItemProviders([UTType], onExport: () -> [NSItemProvider]) -> some View

Exports a read-only item provider for consumption by shortcuts, quick actions, and services.

func exportsItemProviders([UTType], onExport: () -> [NSItemProvider], onEdit: ([NSItemProvider]) -> Bool) -> some View

Exports a read-write item provider for consumption by shortcuts, quick actions, and services.

func fileDialogBrowserOptions(FileDialogBrowserOptions) -> some View

On macOS, configures the `fileExporter`, `fileImporter`, or `fileMover` to provide a refined URL search experience: include or exclude hidden files, allow searching by tag, etc.

func fileDialogConfirmationLabel&lt;S>(S) -> some View

On macOS, configures the the `fileExporter`, `fileImporter`, or `fileMover` with a custom confirmation button label.

func fileDialogConfirmationLabel(Text?) -> some View

On macOS, configures the the `fileExporter`, `fileImporter`, or `fileMover` with custom text as a confirmation button label.

func fileDialogConfirmationLabel(LocalizedStringKey) -> some View

On macOS, configures the the `fileExporter`, `fileImporter`, or `fileMover` with a custom confirmation button label.

func fileDialogCustomizationID(String) -> some View

On macOS, configures the `fileExporter`, `fileImporter`, or `fileMover` to persist and restore the file dialog configuration.

func fileDialogDefaultDirectory(URL?) -> some View

Configures the `fileExporter`, `fileImporter`, or `fileMover` to open with the specified default directory.

func fileDialogImportsUnresolvedAliases(Bool) -> some View

On macOS, configures the `fileExporter`, `fileImporter`, or `fileMover` behavior when a user chooses an alias.

func fileDialogMessage&lt;S>(S) -> some View

On macOS, configures the the `fileExporter`, `fileImporter`, or `fileMover` with a custom message that is presented to the user, similar to a title.

func fileDialogMessage(LocalizedStringKey) -> some View

On macOS, configures the the `fileExporter`, `fileImporter`, or `fileMover` with a custom message that is presented to the user, similar to a title.

func fileDialogMessage(Text?) -> some View

On macOS, configures the the `fileExporter`, `fileImporter`, or `fileMover` with a custom text that is presented to the user, similar to a title.

func fileDialogURLEnabled(Predicate&lt;URL>) -> some View

On macOS, configures the the `fileImporter` or `fileMover` to conditionally disable presented URLs.

func fileExporter&lt;D>(isPresented: Binding&lt;Bool>, document: D?, contentType: UTType, defaultFilename: String?, onCompletion: (Result&lt;URL, any Error>) -> Void) -> some View

Presents a system interface for exporting a document that’s stored in a value type, like a structure, to a file on disk.

func fileExporter&lt;D>(isPresented: Binding&lt;Bool>, document: D?, contentType: UTType, defaultFilename: String?, onCompletion: (Result&lt;URL, any Error>) -> Void) -> some View

Presents a system interface for exporting a document that’s stored in a reference type, like a class, to a file on disk.

func fileExporter&lt;D>(isPresented: Binding&lt;Bool>, document: D?, contentTypes: [UTType], defaultFilename: String?, onCompletion: (Result&lt;URL, any Error>) -> Void, onCancellation: () -> Void) -> some View

Presents a system dialog for allowing the user to export a `ReferenceFileDocument` to a file on disk.

func fileExporter&lt;D>(isPresented: Binding&lt;Bool>, document: D?, contentTypes: [UTType], defaultFilename: String?, onCompletion: (Result&lt;URL, any Error>) -> Void, onCancellation: () -> Void) -> some View

Presents a system interface for allowing the user to export a `FileDocument` to a file on disk.

func fileExporter&lt;C>(isPresented: Binding&lt;Bool>, documents: C, contentType: UTType, onCompletion: (Result&lt;[URL], any Error>) -> Void) -> some View

Presents a system interface for exporting a collection of value type documents to files on disk.

func fileExporter&lt;C>(isPresented: Binding&lt;Bool>, documents: C, contentType: UTType, onCompletion: (Result&lt;[URL], any Error>) -> Void) -> some View

Presents a system interface for exporting a collection of reference type documents to files on disk.

func fileExporter&lt;C>(isPresented: Binding&lt;Bool>, documents: C, contentTypes: [UTType], onCompletion: (Result&lt;[URL], any Error>) -> Void, onCancellation: () -> Void) -> some View

Presents a system dialog for allowing the user to export a collection of documents that conform to `FileDocument` to files on disk.

func fileExporter&lt;C>(isPresented: Binding&lt;Bool>, documents: C, contentTypes: [UTType], onCompletion: (Result&lt;[URL], any Error>) -> Void, onCancellation: () -> Void) -> some View

Presents a system dialog for allowing the user to export a collection of documents that conform to `ReferenceFileDocument` to files on disk.

func fileExporter&lt;T>(isPresented: Binding&lt;Bool>, item: T?, contentTypes: [UTType], defaultFilename: String?, onCompletion: (Result&lt;URL, any Error>) -> Void, onCancellation: () -> Void) -> some View

Presents a system interface allowing the user to export a `Transferable` item to file on disk.

func fileExporter&lt;C, T>(isPresented: Binding&lt;Bool>, items: C, contentTypes: [UTType], onCompletion: (Result&lt;[URL], any Error>) -> Void, onCancellation: () -> Void) -> some View

Presents a system interface allowing the user to export a collection of items to files on disk.

func fileExporterFilenameLabel(LocalizedStringKey) -> some View

On macOS, configures the `fileExporter` with a label for the file name field.

func fileExporterFilenameLabel&lt;S>(S) -> some View

On macOS, configures the `fileExporter` with a label for the file name field.

func fileExporterFilenameLabel(Text?) -> some View

On macOS, configures the `fileExporter` with a text to use as a label for the file name field.

func fileImporter(isPresented: Binding&lt;Bool>, allowedContentTypes: [UTType], allowsMultipleSelection: Bool, onCompletion: (Result&lt;[URL], any Error>) -> Void) -> some View

Presents a system interface for allowing the user to import multiple files.

func fileImporter(isPresented: Binding&lt;Bool>, allowedContentTypes: [UTType], allowsMultipleSelection: Bool, onCompletion: (Result&lt;[URL], any Error>) -> Void, onCancellation: () -> Void) -> some View

Presents a system dialog for allowing the user to import multiple files.

func fileImporter(isPresented: Binding&lt;Bool>, allowedContentTypes: [UTType], onCompletion: (Result&lt;URL, any Error>) -> Void) -> some View

Presents a system interface for allowing the user to import an existing file.

func fileMover(isPresented: Binding&lt;Bool>, file: URL?, onCompletion: (Result&lt;URL, any Error>) -> Void) -> some View

Presents a system interface for allowing the user to move an existing file to a new location.

func fileMover(isPresented: Binding&lt;Bool>, file: URL?, onCompletion: (Result&lt;URL, any Error>) -> Void, onCancellation: () -> Void) -> some View

Presents a system dialog for allowing the user to move an existing file to a new location.

func fileMover&lt;C>(isPresented: Binding&lt;Bool>, files: C, onCompletion: (Result&lt;[URL], any Error>) -> Void) -> some View

Presents a system interface for allowing the user to move a collection of existing files to a new location.

func fileMover&lt;C>(isPresented: Binding&lt;Bool>, files: C, onCompletion: (Result&lt;[URL], any Error>) -> Void, onCancellation: () -> Void) -> some View

Presents a system dialog for allowing the user to move a collection of existing files to a new location.

func findDisabled(Bool) -> some View

Prevents find and replace operations in a text editor.

func findNavigator(isPresented: Binding&lt;Bool>) -> some View

Programmatically presents the find and replace interface for text editor views.

func fixedSize() -> some View

Fixes this view at its ideal size.

func fixedSize(horizontal: Bool, vertical: Bool) -> some View

Fixes this view at its ideal size in the specified dimensions.

func flipsForRightToLeftLayoutDirection(Bool) -> some View

Sets whether this view mirrors its contents horizontally when the layout direction is right-to-left.

func focusEffectDisabled(Bool) -> some View

Adds a condition that controls whether this view can display focus effects, such as a default focus ring or hover effect.

func focusScope(Namespace.ID) -> some View

Creates a focus scope that SwiftUI uses to limit default focus preferences.

func focusSection() -> some View

Indicates that the view’s frame and cohort of focusable descendants should be used to guide focus movement.

func focusable(Bool) -> some View

Specifies if the view is focusable.

func focusable(Bool, interactions: FocusInteractions) -> some View

Specifies if the view is focusable, and if so, what focus-driven interactions it supports.

func focusable(Bool, onFocusChange: (Bool) -> Void) -> some View

Specifies if the view is focusable and, if so, adds an action to perform when the view comes into focus.

Deprecated

func focused(FocusState&lt;Bool>.Binding) -> some View

Modifies this view by binding its focus state to the given Boolean state value.

func focused&lt;Value>(FocusState&lt;Value>.Binding, equals: Value) -> some View

Modifies this view by binding its focus state to the given state value.

func focusedObject&lt;T>(T) -> some View

Creates a new view that exposes the provided object to other views whose whose state depends on the focused view hierarchy.

func focusedObject&lt;T>(T?) -> some View

Creates a new view that exposes the provided object to other views whose state depends on the focused view hierarchy.

func focusedSceneObject&lt;T>(T?) -> some View

Creates a new view that exposes the provided object to other views whose whose state depends on the active scene.

func focusedSceneObject&lt;T>(T) -> some View

Creates a new view that exposes the provided object to other views whose whose state depends on the active scene.

func focusedSceneValue&lt;T>(T?) -> some View

Sets the focused value for the given object type at a scene-wide scope.

func focusedSceneValue&lt;T>(WritableKeyPath&lt;FocusedValues, T?>, T) -> some View

Modifies this view by injecting a value that you provide for use by other views whose state depends on the focused scene.

func focusedSceneValue&lt;T>(WritableKeyPath&lt;FocusedValues, T?>, T?) -> some View

Creates a new view that exposes the provided value to other views whose state depends on the active scene.

func focusedValue&lt;T>(T?) -> some View

Sets the focused value for the given object type.

func focusedValue&lt;Value>(WritableKeyPath&lt;FocusedValues, Value?>, Value) -> some View

Modifies this view by injecting a value that you provide for use by other views whose state depends on the focused view hierarchy.

func focusedValue&lt;Value>(WritableKeyPath&lt;FocusedValues, Value?>, Value?) -> some View

Creates a new view that exposes the provided value to other views whose state depends on the focused view hierarchy.

func font(Font?) -> some View

Sets the default font for text in this view.

func fontDesign(Font.Design?) -> some View

Sets the font design of the text in this view.

func fontWeight(Font.Weight?) -> some View

Sets the font weight of the text in this view.

func fontWidth(Font.Width?) -> some View

Sets the font width of the text in this view.

func foregroundColor(Color?) -> some View

Sets the color of the foreground elements displayed by this view.

Deprecated

func foregroundStyle&lt;S>(S) -> some View

Sets a view’s foreground elements to use a given style.

func foregroundStyle&lt;S1, S2>(S1, S2) -> some View

Sets the primary and secondary levels of the foreground style in the child view.

func foregroundStyle&lt;S1, S2, S3>(S1, S2, S3) -> some View

Sets the primary, secondary, and tertiary levels of the foreground style.

func formStyle&lt;S>(S) -> some View

Sets the style for forms in a view hierarchy.

func frame() -> some View

Positions this view within an invisible frame.

Deprecated

func frame(depth: CGFloat?, alignment: DepthAlignment) -> some View

Positions this view within an invisible frame with the specified depth.

func frame(minDepth: CGFloat?, idealDepth: CGFloat?, maxDepth: CGFloat?, alignment: DepthAlignment) -> some View

Positions this view within an invisible frame having the specified depth constraints.

func frame(minWidth: CGFloat?, idealWidth: CGFloat?, maxWidth: CGFloat?, minHeight: CGFloat?, idealHeight: CGFloat?, maxHeight: CGFloat?, alignment: Alignment) -> some View

Positions this view within an invisible frame having the specified size constraints.

func frame(width: CGFloat?, height: CGFloat?, alignment: Alignment) -> some View

Positions this view within an invisible frame with the specified size.

func fullScreenCover&lt;Content>(isPresented: Binding&lt;Bool>, onDismiss: (() -> Void)?, content: () -> Content) -> some View

Presents a modal view that covers as much of the screen as possible when binding to a Boolean value you provide is true.

func fullScreenCover&lt;Item, Content>(item: Binding&lt;Item?>, onDismiss: (() -> Void)?, content: (Item) -> Content) -> some View

Presents a modal view that covers as much of the screen as possible using the binding you provide as a data source for the sheet’s content.

func gaugeStyle&lt;S>(S) -> some View

Sets the style for gauges within this view.

func geometryGroup() -> some View

Isolates the geometry (e.g. position and size) of the view from its parent view.

func gesture(some UIGestureRecognizerRepresentable) -> some View

Attaches a `UIGestureRecognizerRepresentable` to the view.

func gesture&lt;T>(T, including: GestureMask) -> some View

Attaches a gesture to the view with a lower precedence than gestures defined by the view.

func gesture&lt;T>(T, isEnabled: Bool) -> some View

Attaches a gesture to the view with a lower precedence than gestures defined by the view.

func gesture&lt;T>(T, name: String, isEnabled: Bool) -> some View

Attaches a gesture to the view with a lower precedence than gestures defined by the view.

func glassBackgroundEffect&lt;S>(S, displayMode: GlassBackgroundDisplayMode) -> some View

Fills the view’s background with a custom glass background effect and container-relative rounded rectangle shape.

func glassBackgroundEffect&lt;T, S>(S, in: T, displayMode: GlassBackgroundDisplayMode) -> some View

Fills the view’s background with a custom glass background effect and a shape that you specify.

func glassBackgroundEffect(displayMode: GlassBackgroundDisplayMode) -> some View

Fills the view’s background with an automatic glass background effect and container-relative rounded rectangle shape.

func glassBackgroundEffect&lt;S>(in: S, displayMode: GlassBackgroundDisplayMode) -> some View

Fills the view’s background with an automatic glass background effect and a shape that you specify.

func grayscale(Double) -> some View

Adds a grayscale effect to this view.

func gridCellAnchor(UnitPoint) -> some View

Specifies a custom alignment anchor for a view that acts as a grid cell.

func gridCellColumns(Int) -> some View

Tells a view that acts as a cell in a grid to span the specified number of columns.

func gridCellUnsizedAxes(Axis.Set) -> some View

Asks grid layouts not to offer the view extra size in the specified axes.

func gridColumnAlignment(HorizontalAlignment) -> some View

Overrides the default horizontal alignment of the grid column that the view appears in.

func groupBoxStyle&lt;S>(S) -> some View

Sets the style for group boxes within this view.

func handGestureShortcut(HandGestureShortcut, isEnabled: Bool) -> some View

Assigns a hand gesture shortcut to the modified control.

func handPointerBehavior(HandPointerBehavior?) -> some View

Sets the behavior of the hand pointer while the user is interacting with the view.

func handlesExternalEvents(preferring: Set&lt;String>, allowing: Set&lt;String>) -> some View

Specifies the external events that the view’s scene handles if the scene is already open.

func headerProminence(Prominence) -> some View

Sets the header prominence for this view.

func help&lt;S>(S) -> some View

Adds help text to a view using a string that you provide.

func help(LocalizedStringKey) -> some View

Adds help text to a view using a localized string that you provide.

func help(Text) -> some View

Adds help text to a view using a text view that you provide.

func hidden() -> some View

Hides this view unconditionally.

func highPriorityGesture&lt;T>(T, including: GestureMask) -> some View

Attaches a gesture to the view with a higher precedence than gestures defined by the view.

func highPriorityGesture&lt;T>(T, isEnabled: Bool) -> some View

Attaches a gesture to the view with a higher precedence than gestures defined by the view.

func highPriorityGesture&lt;T>(T, name: String, isEnabled: Bool) -> some View

Attaches a gesture to the view with a higher precedence than gestures defined by the view.

func horizontalRadioGroupLayout() -> some View

Sets the style for radio group style pickers within this view to be horizontally positioned with the radio buttons inside the layout.

func hoverEffect(HoverEffect) -> some View

Applies a hover effect to this view.

func hoverEffect(some CustomHoverEffect, in: HoverEffectGroup?, isEnabled: Bool) -> some View

Applies a hover effect to this view, optionally adding it to a `HoverEffectGroup`.

func hoverEffect(HoverEffect, isEnabled: Bool) -> some View

Applies a hover effect to this view.

func hoverEffect(some CustomHoverEffect, isEnabled: Bool) -> some View

Applies a hover effect to this view, while providing a way to conditionally enable or disable it.

func hoverEffect(in: HoverEffectGroup?, isEnabled: Bool, body: (EmptyHoverEffectContent, Bool, GeometryProxy) -> some HoverEffectContent) -> some View

Applies a hover effect to this view described by the given closure.

func hoverEffectDisabled(Bool) -> some View

Adds a condition that controls whether this view can display hover effects.

func hoverEffectGroup() -> some View

Adds an implicit `HoverEffectGroup` to all effects defined on descendant views, so that all effects added to subviews activate as a group whenever this view or any descendant views are hovered.

func hoverEffectGroup(HoverEffectGroup?) -> some View

Adds a `HoverEffectGroup` to all effects defined on descendant views, and activates the group whenever this view or any descendant views are hovered.

func hoverEffectGroup(id: String?, in: Namespace.ID, behavior: HoverEffectGroup.Behavior) -> some View

Adds a `HoverEffectGroup` to all effects defined on descendant views, and activates the group whenever this view or any descendant views are hovered.

func hueRotation(Angle) -> some View

Applies a hue rotation effect to this view.

func id&lt;ID>(ID) -> some View

Binds a view’s identity to the given proxy value.

func ignoresSafeArea(SafeAreaRegions, edges: Edge.Set) -> some View

Expands the safe area of a view.

func imageScale(Image.Scale) -> some View

Scales images within the view according to one of the relative sizes available including small, medium, and large images sizes.

func immersiveEnvironmentPicker&lt;Content>(content: () -> Content) -> some View

Add menu items to open immersive spaces from a media player’s environment picker.

func importableFromServices&lt;T>(for: T.Type, action: ([T]) -> Bool) -> some View

Enables importing items from services, such as Continuity Camera on macOS.

func importsItemProviders([UTType], onImport: ([NSItemProvider]) -> Bool) -> some View

Enables importing item providers from services, such as Continuity Camera on macOS.

func indexViewStyle&lt;S>(S) -> some View

Sets the style for the index view within the current environment.

func inspector&lt;V>(isPresented: Binding&lt;Bool>, content: () -> V) -> some View

Inserts an inspector at the applied position in the view hierarchy.

func inspectorColumnWidth(CGFloat) -> some View

Sets a fixed, preferred width for the inspector containing this view when presented as a trailing column.

func inspectorColumnWidth(min: CGFloat?, ideal: CGFloat, max: CGFloat?) -> some View

Sets a flexible, preferred width for the inspector in a trailing-column presentation.

func interactionActivityTrackingTag(String) -> some View

Sets a tag that you use for tracking interactivity.

func interactiveDismissDisabled(Bool) -> some View

Conditionally prevents interactive dismissal of presentations like popovers, sheets, and inspectors.

func invalidatableContent(Bool) -> some View

Mark the receiver as their content might be invalidated.

func italic(Bool) -> some View

Applies italics to the text in this view.

func itemProvider(Optional&lt;() -> NSItemProvider?>) -> some View

Provides a closure that vends the drag representation to be used for a particular data element.

func kerning(CGFloat) -> some View

Sets the spacing, or kerning, between characters for the text in this view.

func keyboardShortcut(KeyboardShortcut?) -> some View

Assigns an optional keyboard shortcut to the modified control.

func keyboardShortcut(KeyboardShortcut) -> some View

Assigns a keyboard shortcut to the modified control.

func keyboardShortcut(KeyEquivalent, modifiers: EventModifiers) -> some View

Defines a keyboard shortcut and assigns it to the modified control.

func keyboardShortcut(KeyEquivalent, modifiers: EventModifiers, localization: KeyboardShortcut.Localization) -> some View

Defines a keyboard shortcut and assigns it to the modified control.

func keyboardType(UIKeyboardType) -> some View

Sets the keyboard type for this view.

func keyframeAnimator&lt;Value>(initialValue: Value, repeating: Bool, content: (PlaceholderContentView&lt;Self>, Value) -> some View, keyframes: (Value) -> some Keyframes) -> some View

Loops the given keyframes continuously, updating the view using the modifiers you apply in `body`.

func keyframeAnimator&lt;Value>(initialValue: Value, trigger: some Equatable, content: (PlaceholderContentView&lt;Self>, Value) -> some View, keyframes: (Value) -> some Keyframes) -> some View

Plays the given keyframes when the given trigger value changes, updating the view using the modifiers you apply in `body`.

func labelStyle&lt;S>(S) -> some View

Sets the style for labels within this view.

func labeledContentStyle&lt;S>(S) -> some View

Sets a style for labeled content.

func labelsHidden() -> some View

Hides the labels of any controls contained within this view.

func labelsVisibility(Visibility) -> some View

Controls the visibility of labels of any controls contained within this view.

func layerEffect(Shader, maxSampleOffset: CGSize, isEnabled: Bool) -> some View

Returns a new view that applies `shader` to `self` as a filter on the raster layer created from `self`.

func layoutDirectionBehavior(LayoutDirectionBehavior) -> some View

Sets the behavior of this view for different layout directions.

func layoutPriority(Double) -> some View

Sets the priority by which a parent layout should apportion space to this child.

func layoutValue&lt;K>(key: K.Type, value: K.Value) -> some View

Associates a value with a custom layout property.

func lineLimit(PartialRangeThrough&lt;Int>) -> some View

Sets to a partial range the number of lines that text can occupy in this view.

func lineLimit(ClosedRange&lt;Int>) -> some View

Sets to a closed range the number of lines that text can occupy in this view.

func lineLimit(PartialRangeFrom&lt;Int>) -> some View

Sets to a partial range the number of lines that text can occupy in this view.

func lineLimit(Int?) -> some View

Sets the maximum number of lines that text can occupy in this view.

func lineLimit(Int, reservesSpace: Bool) -> some View

Sets a limit for the number of lines text can occupy in this view.

func lineSpacing(CGFloat) -> some View

Sets the amount of space between lines of text in this view.

func listItemTint(ListItemTint?) -> some View

Sets the tint effect for content in a list.

func listItemTint(Color?) -> some View

Sets a fixed tint color for content in a list.

func listRowBackground&lt;V>(V?) -> some View

Places a custom background view behind a list row item.

func listRowHoverEffect(HoverEffect?) -> some View

Requests that the containing list row use the provided hover effect.

func listRowHoverEffectDisabled(Bool) -> some View

Requests that the containing list row have its hover effect disabled.

func listRowInsets(EdgeInsets?) -> some View

Applies an inset to the rows in a list.

func listRowPlatterColor(Color?) -> some View

Sets the color that the system applies to the row background when this view is placed in a list.

Deprecated

func listRowSeparator(Visibility, edges: VerticalEdge.Set) -> some View

Sets the display mode for the separator associated with this specific row.

func listRowSeparatorTint(Color?, edges: VerticalEdge.Set) -> some View

Sets the tint color associated with a row.

func listRowSpacing(CGFloat?) -> some View

Sets the vertical spacing between two adjacent rows in a List.

func listSectionSeparator(Visibility, edges: VerticalEdge.Set) -> some View

Sets whether to hide the separator associated with a list section.

func listSectionSeparatorTint(Color?, edges: VerticalEdge.Set) -> some View

Sets the tint color associated with a section.

func listSectionSpacing(ListSectionSpacing) -> some View

Sets the spacing between adjacent sections in a `List`.

func listSectionSpacing(CGFloat) -> some View

Sets the spacing between adjacent sections in a `List` to a custom value.

func listStyle&lt;S>(S) -> some View

Sets the style for lists within this view.

func luminanceToAlpha() -> some View

Adds a luminance to alpha effect to this view.

func mask&lt;Mask>(Mask) -> some View

Masks this view using the alpha channel of the given view.

Deprecated

func mask&lt;Mask>(alignment: Alignment, () -> Mask) -> some View

Masks this view using the alpha channel of the given view.

func matchedGeometryEffect&lt;ID>(id: ID, in: Namespace.ID, properties: MatchedGeometryProperties, anchor: UnitPoint, isSource: Bool) -> some View

Defines a group of views with synchronized geometry using an identifier and namespace that you provide.

func matchedTransitionSource(id: some Hashable, in: Namespace.ID) -> some View

Identifies this view as the source of a navigation transition, such as a zoom transition.

func matchedTransitionSource(id: some Hashable, in: Namespace.ID, configuration: (EmptyMatchedTransitionSourceConfiguration) -> some MatchedTransitionSourceConfiguration) -> some View

Identifies this view as the source of a navigation transition, such as a zoom transition.

func materialActiveAppearance(MaterialActiveAppearance) -> some View

Sets an explicit active appearance for materials in this view.

func menuActionDismissBehavior(MenuActionDismissBehavior) -> some View

Tells a menu whether to dismiss after performing an action.

func menuButtonStyle&lt;S>(S) -> some View

Sets the style for menu buttons within this view.

Deprecated

func menuIndicator(Visibility) -> some View

Sets the menu indicator visibility for controls within this view.

func menuOrder(MenuOrder) -> some View

Sets the preferred order of items for menus presented from this view.

func menuStyle&lt;S>(S) -> some View

Sets the style for menus within this view.

func minimumScaleFactor(CGFloat) -> some View

Sets the minimum amount that text in this view scales down to fit in the available space.

func modifier&lt;T>(T) -> ModifiedContent&lt;Self, T>

Applies a modifier to a view and returns a new view.

func modifierKeyAlternate&lt;V>(EventModifiers, () -> V) -> some View

Builds a view to use in place of the modified view when the user presses the modifier key(s) indicated by the given set.

func monospaced(Bool) -> some View

Modifies the fonts of all child views to use the fixed-width variant of the current font, if possible.

func monospacedDigit() -> some View

Modifies the fonts of all child views to use fixed-width digits, if possible, while leaving other characters proportionally spaced.

func moveDisabled(Bool) -> some View

Adds a condition for whether the view’s view hierarchy is movable.

func multilineTextAlignment(TextAlignment) -> some View

Sets the alignment of a text view that contains multiple lines of text.

func musicSubscriptionOffer(isPresented: Binding&lt;Bool>, options: MusicSubscriptionOffer.Options, onLoadCompletion: ((any Error)?) -> Void) -> some View

Initiates the process of presenting a sheet with subscription offers for Apple Music when the `isPresented` binding is `true`.

func navigationBarBackButtonHidden(Bool) -> some View

Hides the navigation bar back button for the view.

func navigationBarHidden(Bool) -> some View

Hides the navigation bar for this view.

Deprecated

func navigationBarItems&lt;L>(leading: L) -> some ViewDeprecated

func navigationBarItems&lt;L, T>(leading: L, trailing: T) -> some ViewDeprecated

func navigationBarItems&lt;T>(trailing: T) -> some ViewDeprecated

func navigationBarTitle&lt;S>(S) -> some View

Sets the title of this view’s navigation bar with a string.

Deprecated

func navigationBarTitle(Text) -> some View

Sets the title in the navigation bar for this view.

Deprecated

func navigationBarTitle(LocalizedStringKey) -> some View

Sets the title of this view’s navigation bar with a localized string.

Deprecated

func navigationBarTitle(LocalizedStringKey, displayMode: NavigationBarItem.TitleDisplayMode) -> some View

Sets the title and display mode in the navigation bar for this view.

Deprecated

func navigationBarTitle(Text, displayMode: NavigationBarItem.TitleDisplayMode) -> some View

Sets the title and display mode in the navigation bar for this view.

Deprecated

func navigationBarTitle&lt;S>(S, displayMode: NavigationBarItem.TitleDisplayMode) -> some View

Sets the title and display mode in the navigation bar for this view.

Deprecated

func navigationBarTitleDisplayMode(NavigationBarItem.TitleDisplayMode) -> some View

Configures the title display mode for this view.

func navigationDestination&lt;D, C>(for: D.Type, destination: (D) -> C) -> some View

Associates a destination view with a presented data type for use within a navigation stack.

func navigationDestination&lt;V>(isPresented: Binding&lt;Bool>, destination: () -> V) -> some View

Associates a destination view with a binding that can be used to push the view onto a `NavigationStack`.

func navigationDestination&lt;D, C>(item: Binding&lt;Optional&lt;D>>, destination: (D) -> C) -> some View

Associates a destination view with a bound value for use within a navigation stack or navigation split view

func navigationDocument&lt;D>(D) -> some View

Configures the view’s document for purposes of navigation.

func navigationDocument(URL) -> some View

Configures the view’s document for purposes of navigation.

func navigationDocument&lt;D>(D, preview: SharePreview&lt;Never, Never>) -> some View

Configures the view’s document for purposes of navigation.

func navigationDocument&lt;D, I>(D, preview: SharePreview&lt;Never, I>) -> some View

Configures the view’s document for purposes of navigation.

func navigationDocument&lt;D, I1, I2>(D, preview: SharePreview&lt;I1, I2>) -> some View

Configures the view’s document for purposes of navigation.

func navigationDocument&lt;D, I>(D, preview: SharePreview&lt;I, Never>) -> some View

Configures the view’s document for purposes of navigation.

func navigationSplitViewColumnWidth(CGFloat) -> some View

Sets a fixed, preferred width for the column containing this view.

func navigationSplitViewColumnWidth(min: CGFloat?, ideal: CGFloat, max: CGFloat?) -> some View

Sets a flexible, preferred width for the column containing this view.

func navigationSplitViewStyle&lt;S>(S) -> some View

Sets the style for navigation split views within this view.

func navigationSubtitle&lt;S>(S) -> some View

Configures the view’s subtitle for purposes of navigation, using a string.

func navigationSubtitle(Text) -> some View

Configures the view’s subtitle for purposes of navigation.

func navigationSubtitle(LocalizedStringKey) -> some View

Configures the view’s subtitle for purposes of navigation, using a localized string.

func navigationTitle&lt;V>(() -> V) -> some View

Configures the view’s title for purposes of navigation, using a custom view.

func navigationTitle(LocalizedStringKey) -> some View

Configures the view’s title for purposes of navigation, using a localized string.

func navigationTitle(Text) -> some View

Configures the view’s title for purposes of navigation.

func navigationTitle(Binding&lt;String>) -> some View

Configures the view’s title for purposes of navigation, using a string binding.

func navigationTitle&lt;S>(S) -> some View

Configures the view’s title for purposes of navigation, using a string.

func navigationTransition(some NavigationTransition) -> some View

Sets the navigation transition style for this view.

func navigationViewStyle&lt;S>(S) -> some View

Sets the style for navigation views within this view.

Deprecated

func offset(CGSize) -> some View

Offset this view by the horizontal and vertical amount specified in the offset parameter.

func offset(x: CGFloat, y: CGFloat) -> some View

Offset this view by the specified horizontal and vertical distances.

func offset(z: CGFloat) -> some View

Brings a view forward in Z by the provided distance in points.

func onAppear(perform: (() -> Void)?) -> some View

Adds an action to perform before this view appears.

func onChange&lt;V>(of: V, initial: Bool, (V, V) -> Void) -> some View

Adds a modifier for this view that fires an action when a specific value changes.

func onChange&lt;V>(of: V, initial: Bool, () -> Void) -> some View

Adds a modifier for this view that fires an action when a specific value changes.

func onChange&lt;V>(of: V, perform: (V) -> Void) -> some View

Performs an action when a specified value changes.

Deprecated

func onCommand(Selector, perform: (() -> Void)?) -> some View

Adds an action to perform in response to the given selector.

func onContinueUserActivity(String, perform: (NSUserActivity) -> ()) -> some View

Registers a handler to invoke in response to a user activity that your app receives.

func onContinuousHover(coordinateSpace: some CoordinateSpaceProtocol, perform: (HoverPhase) -> Void) -> some View

Adds an action to perform when the pointer enters, moves within, and exits the view’s bounds.

func onContinuousHover(coordinateSpace: CoordinateSpace, perform: (HoverPhase) -> Void) -> some View

Adds an action to perform when the pointer enters, moves within, and exits the view’s bounds.

Deprecated

func onCopyCommand(perform: (() -> [NSItemProvider])?) -> some View

Adds an action to perform in response to the system’s Copy command.

func onCutCommand(perform: (() -> [NSItemProvider])?) -> some View

Adds an action to perform in response to the system’s Cut command.

func onDeleteCommand(perform: (() -> Void)?) -> some View

Adds an action to perform in response to the system’s Delete command, or pressing either the ⌫ (backspace) or ⌦ (forward delete) keys while the view has focus.

func onDisappear(perform: (() -> Void)?) -> some View

Adds an action to perform after this view disappears.

func onDrag(() -> NSItemProvider) -> some View

Activates this view as the source of a drag and drop operation.

func onDrag&lt;V>(() -> NSItemProvider, preview: () -> V) -> some View

Activates this view as the source of a drag and drop operation.

func onDrop(of: [String], delegate: any DropDelegate) -> some View

Defines the destination for a drag and drop operation with the same size and position as this view, with behavior controlled by the given delegate.

Deprecated

func onDrop(of: [UTType], delegate: any DropDelegate) -> some View

Defines the destination of a drag and drop operation using behavior controlled by the delegate that you provide.

func onDrop(of: [String], isTargeted: Binding&lt;Bool>?, perform: ([NSItemProvider], CGPoint) -> Bool) -> some View

Defines the destination for a drag and drop operation with the same size and position as this view, handling dropped content and the drop location with the given closure.

Deprecated

func onDrop(of: [String], isTargeted: Binding&lt;Bool>?, perform: ([NSItemProvider]) -> Bool) -> some View

Defines the destination for a drag and drop operation, using the same size and position as this view, handling dropped content with the given closure.

Deprecated

func onDrop(of: [UTType], isTargeted: Binding&lt;Bool>?, perform: ([NSItemProvider]) -> Bool) -> some View

Defines the destination of a drag-and-drop operation that handles the dropped content with a closure that you specify.

func onDrop(of: [UTType], isTargeted: Binding&lt;Bool>?, perform: ([NSItemProvider], CGPoint) -> Bool) -> some View

Defines the destination of a drag and drop operation that handles the dropped content with a closure that you specify.

func onExitCommand(perform: (() -> Void)?) -> some View

Sets up an action that triggers in response to receiving the exit command while the view has focus.

func onGeometryChange&lt;T>(for: T.Type, of: (GeometryProxy) -> T, action: (T) -> Void) -> some View

Adds an action to be performed when a value, created from a geometry proxy, changes.

func onGeometryChange&lt;T>(for: T.Type, of: (GeometryProxy) -> T, action: (T, T) -> Void) -> some View

Adds an action to be performed when a value, created from a geometry proxy, changes.

func onGeometryChange3D&lt;T>(for: T.Type, of: (GeometryProxy3D) -> T, action: (T) -> Void) -> some View

Returns a new view that arranges to call `action(value)` whenever the value computed by `transform(proxy)` changes, where `proxy` provides access to the view’s 3D geometry properties.

func onGeometryChange3D&lt;T>(for: T.Type, of: (GeometryProxy3D) -> T, action: (T, T) -> Void) -> some View

Returns a new view that arranges to call `action(oldValue, newValue)` whenever the value computed by `value(proxy)` changes, where `proxy` provides access to the view’s 3D geometry properties.

func onHover(perform: (Bool) -> Void) -> some View

Adds an action to perform when the user moves the pointer over or away from the view’s frame.

func onImmersionChange(initial: Bool, (ImmersionChangeContext, ImmersionChangeContext) -> Void) -> some View

Performs an action when the immersion state of your app changes.

func onKeyPress(KeyEquivalent, action: () -> KeyPress.Result) -> some View

Performs an action if the user presses a key on a hardware keyboard while the view has focus.

func onKeyPress(KeyEquivalent, phases: KeyPress.Phases, action: (KeyPress) -> KeyPress.Result) -> some View

Performs an action if the user presses a key on a hardware keyboard while the view has focus.

func onKeyPress(characters: CharacterSet, phases: KeyPress.Phases, action: (KeyPress) -> KeyPress.Result) -> some View

Performs an action if the user presses one or more keys on a hardware keyboard while the view has focus.

func onKeyPress(keys: Set&lt;KeyEquivalent>, phases: KeyPress.Phases, action: (KeyPress) -> KeyPress.Result) -> some View

Performs an action if the user presses one or more keys on a hardware keyboard while the view has focus.

func onKeyPress(phases: KeyPress.Phases, action: (KeyPress) -> KeyPress.Result) -> some View

Performs an action if the user presses any key on a hardware keyboard while the view has focus.

func onLongPressGesture(minimumDuration: Double, maximumDistance: CGFloat, perform: () -> Void, onPressingChanged: ((Bool) -> Void)?) -> some View

Adds an action to perform when this view recognizes a long press gesture.

func onLongPressGesture(minimumDuration: Double, maximumDistance: CGFloat, pressing: ((Bool) -> Void)?, perform: () -> Void) -> some View

Adds an action to perform when this view recognizes a long press gesture.

Deprecated

func onLongPressGesture(minimumDuration: Double, perform: () -> Void, onPressingChanged: ((Bool) -> Void)?) -> some View

Adds an action to perform when this view recognizes a long press gesture.

func onLongPressGesture(minimumDuration: Double, pressing: ((Bool) -> Void)?, perform: () -> Void) -> some View

Adds an action to perform when this view recognizes a long press gesture.

Deprecated

func onLongTouchGesture(minimumDuration: Double, perform: () -> Void, onTouchingChanged: ((Bool) -> Void)?) -> some View

Adds an action to perform when this view recognizes a remote long touch gesture. A long touch gesture is when the finger is on the remote touch surface without actually pressing.

func onModifierKeysChanged(mask: EventModifiers, initial: Bool, (EventModifiers, EventModifiers) -> Void) -> some View

Performs an action whenever the user presses or releases a hardware modifier key.

func onMoveCommand(perform: ((MoveCommandDirection) -> Void)?) -> some View

Adds an action to perform in response to a move command, like when the user presses an arrow key on a Mac keyboard, or taps the edge of the Siri Remote when controlling an Apple TV.

func onOpenURL(perform: (URL) -> ()) -> some View

Registers a handler to invoke in response to a URL that your app receives.

func onPasteCommand(of: [String], perform: ([NSItemProvider]) -> Void) -> some View

Adds an action to perform in response to the system’s Paste command.

Deprecated

func onPasteCommand(of: [UTType], perform: ([NSItemProvider]) -> Void) -> some View

Adds an action to perform in response to the system’s Paste command.

func onPasteCommand&lt;Payload>(of: [String], validator: ([NSItemProvider]) -> Payload?, perform: (Payload) -> Void) -> some View

Adds an action to perform in response to the system’s Paste command with items that you validate.

Deprecated

func onPasteCommand&lt;Payload>(of: [UTType], validator: ([NSItemProvider]) -> Payload?, perform: (Payload) -> Void) -> some View

Adds an action to perform in response to the system’s Paste command with items that you validate.

func onPencilDoubleTap(perform: (PencilDoubleTapGestureValue) -> Void) -> some View

Adds an action to perform after the user double-taps their Apple Pencil.

func onPencilSqueeze(perform: (PencilSqueezeGesturePhase) -> Void) -> some View

Adds an action to perform when the user squeezes their Apple Pencil.

func onPlayPauseCommand(perform: (() -> Void)?) -> some View

Adds an action to perform in response to the system’s Play/Pause command.

func onPreferenceChange&lt;K>(K.Type, perform: (K.Value) -> Void) -> some View

Adds an action to perform when the specified preference key’s value changes.

func onReceive&lt;P>(P, perform: (P.Output) -> Void) -> some View

Adds an action to perform when this view detects data emitted by the given publisher.

func onScrollGeometryChange&lt;T>(for: T.Type, of: (ScrollGeometry) -> T, action: (T, T) -> Void) -> some View

Adds an action to be performed when a value, created from a scroll geometry, changes.

func onScrollPhaseChange((ScrollPhase, ScrollPhase) -> Void) -> some View

Adds an action to perform when the scroll phase of the first scroll view in the hierarchy changes.

func onScrollPhaseChange((ScrollPhase, ScrollPhase, ScrollPhaseChangeContext) -> Void) -> some View

Adds an action to perform when the scroll phase of the first scroll view in the hierarchy changes.

func onScrollTargetVisibilityChange&lt;ID>(idType: ID.Type, threshold: Double, ([ID]) -> Void) -> some View

Adds an action to be called with information about what views would be considered visible.

func onScrollVisibilityChange(threshold: Double, (Bool) -> Void) -> some View

Adds an action to be called when the view crosses the threshold to be considered on/off screen.

func onSubmit(of: SubmitTriggers, () -> Void) -> some View

Adds an action to perform when the user submits a value to this view.

func onTapGesture(count: Int, coordinateSpace: some CoordinateSpaceProtocol, perform: (CGPoint) -> Void) -> some View

Adds an action to perform when this view recognizes a tap gesture, and provides the action with the location of the interaction.

func onTapGesture(count: Int, coordinateSpace: CoordinateSpace, perform: (CGPoint) -> Void) -> some View

Adds an action to perform when this view recognizes a tap gesture, and provides the action with the location of the interaction.

Deprecated

func onTapGesture(count: Int, perform: () -> Void) -> some View

Adds an action to perform when this view recognizes a tap gesture.

func onVolumeViewpointChange(updateStrategy: VolumeViewpointUpdateStrategy, initial: Bool, (Viewpoint3D, Viewpoint3D) -> Void) -> some View

Adds an action to perform when the viewpoint of the volume changes.

func opacity(Double) -> some View

Sets the transparency of this view.

func ornament&lt;Content>(visibility: Visibility, attachmentAnchor: OrnamentAttachmentAnchor, contentAlignment: Alignment, ornament: () -> Content) -> some View

Presents an ornament.

func overlay&lt;Overlay>(Overlay, alignment: Alignment) -> some View

Layers a secondary view in front of this view.

Deprecated

func overlay&lt;S>(S, ignoresSafeAreaEdges: Edge.Set) -> some View

Layers the specified style in front of this view.

func overlay&lt;S, T>(S, in: T, fillStyle: FillStyle) -> some View

Layers a shape that you specify in front of this view.

func overlay&lt;V>(alignment: Alignment, content: () -> V) -> some View

Layers the views that you specify in front of this view.

func overlayPreferenceValue&lt;Key, T>(Key.Type, (Key.Value) -> T) -> some View

Reads the specified preference value from the view, using it to produce a second view that is applied as an overlay to the original view.

func overlayPreferenceValue&lt;K, V>(K.Type, alignment: Alignment, (K.Value) -> V) -> some View

Reads the specified preference value from the view, using it to produce a second view that is applied as an overlay to the original view.

func padding(EdgeInsets) -> some View

Adds a different padding amount to each edge of this view.

func padding(CGFloat) -> some View

Adds a specific padding amount to each edge of this view.

func padding(Edge.Set, CGFloat?) -> some View

Adds an equal padding amount to specific edges of this view.

func padding3D(EdgeInsets3D) -> some View

Pads this view using the edge insets you specify.

func padding3D(CGFloat) -> some View

Pads this view along all edge insets by the amount you specify.

func padding3D(Edge3D.Set, CGFloat?) -> some View

Pads this view using the edge insets you specify.

func pageCommand&lt;V>(value: Binding&lt;V>, in: ClosedRange&lt;V>, step: V) -> some View

Steps a value through a range in response to page up or page down commands.

func paletteSelectionEffect(PaletteSelectionEffect) -> some View

Specifies the selection effect to apply to a palette item.

func pasteDestination&lt;T>(for: T.Type, action: ([T]) -> Void, validator: ([T]) -> [T]) -> some View

Specifies an action that adds validated items to a view in response to the system’s Paste command.

func persistentSystemOverlays(Visibility) -> some View

Sets the preferred visibility of the non-transient system views overlaying the app.

func perspectiveRotationEffect(Angle, axis: (x: CGFloat, y: CGFloat, z: CGFloat), anchor: UnitPoint, anchorZ: CGFloat, perspective: CGFloat) -> some View

Renders a view’s content as if it’s rotated in three dimensions around the specified axis.

func phaseAnimator&lt;Phase>(some Sequence, content: (PlaceholderContentView&lt;Self>, Phase) -> some View, animation: (Phase) -> Animation?) -> some View

Animates effects that you apply to a view over a sequence of phases that change continuously.

func phaseAnimator&lt;Phase>(some Sequence, trigger: some Equatable, content: (PlaceholderContentView&lt;Self>, Phase) -> some View, animation: (Phase) -> Animation?) -> some View

Animates effects that you apply to a view over a sequence of phases that change based on a trigger.

func pickerStyle&lt;S>(S) -> some View

Sets the style for pickers within this view.

func pointerStyle(PointerStyle?) -> some View

Sets the pointer style to display when the pointer is over the view.

func pointerVisibility(Visibility) -> some View

Sets the visibility of the pointer when it’s over the view.

func popover&lt;Content>(isPresented: Binding&lt;Bool>, attachmentAnchor: PopoverAttachmentAnchor, arrowEdge: Edge?, content: () -> Content) -> some View

Presents a popover when a given condition is true.

func popover&lt;Item, Content>(item: Binding&lt;Item?>, attachmentAnchor: PopoverAttachmentAnchor, arrowEdge: Edge?, content: (Item) -> Content) -> some View

Presents a popover using the given item as a data source for the popover’s content.

func position(CGPoint) -> some View

Positions the center of this view at the specified point in its parent’s coordinate space.

func position(x: CGFloat, y: CGFloat) -> some View

Positions the center of this view at the specified coordinates in its parent’s coordinate space.

func preference&lt;K>(key: K.Type, value: K.Value) -> some View

Sets a value for the given preference.

func preferredColorScheme(ColorScheme?) -> some View

Sets the preferred color scheme for this presentation.

func preferredSurroundingsEffect(SurroundingsEffect?) -> some View

Applies an effect to passthrough video.

func prefersDefaultFocus(Bool, in: Namespace.ID) -> some View

Indicates that the view should receive focus by default for a given namespace.

func presentationBackground&lt;S>(S) -> some View

Sets the presentation background of the enclosing sheet using a shape style.

func presentationBackground&lt;V>(alignment: Alignment, content: () -> V) -> some View

Sets the presentation background of the enclosing sheet to a custom view.

func presentationBackgroundInteraction(PresentationBackgroundInteraction) -> some View

Controls whether people can interact with the view behind a presentation.

func presentationCompactAdaptation(PresentationAdaptation) -> some View

Specifies how to adapt a presentation to compact size classes.

func presentationCompactAdaptation(horizontal: PresentationAdaptation, vertical: PresentationAdaptation) -> some View

Specifies how to adapt a presentation to horizontally and vertically compact size classes.

func presentationContentInteraction(PresentationContentInteraction) -> some View

Configures the behavior of swipe gestures on a presentation.

func presentationCornerRadius(CGFloat?) -> some View

Requests that the presentation have a specific corner radius.

func presentationDetents(Set&lt;PresentationDetent>) -> some View

Sets the available detents for the enclosing sheet.

func presentationDetents(Set&lt;PresentationDetent>, selection: Binding&lt;PresentationDetent>) -> some View

Sets the available detents for the enclosing sheet, giving you programmatic control of the currently selected detent.

func presentationDragIndicator(Visibility) -> some View

Sets the visibility of the drag indicator on top of a sheet.

func presentationPreventsAppTermination(Bool?) -> some View

Whether a presentation prevents the app from being terminated/quit by the system or app termination menu item.

func presentationSizing(some PresentationSizing) -> some View

Sets the sizing of the containing presentation.

func presentedWindowStyle&lt;S>(S) -> some View

Sets the style for windows created by interacting with this view.

func presentedWindowToolbarStyle&lt;S>(S) -> some View

Sets the style for the toolbar in windows created by interacting with this view.

func previewContext&lt;C>(C) -> some View

Declares a context for the preview.

func previewDevice(PreviewDevice?) -> some View

Overrides the device for a preview.

func previewDisplayName(String?) -> some View

Sets a user visible name to show in the canvas for a preview.

func previewInterfaceOrientation(InterfaceOrientation) -> some View

Overrides the orientation of the preview.

func previewLayout(PreviewLayout) -> some View

Overrides the size of the container for the preview.

func privacySensitive(Bool) -> some View

Marks the view as containing sensitive, private user data.

func progressViewStyle&lt;S>(S) -> some View

Sets the style for progress views in this view.

func projectionEffect(ProjectionTransform) -> some View

Applies a projection transformation to this view’s rendered output.

func redacted(reason: RedactionReasons) -> some View

Adds a reason to apply a redaction to this view hierarchy.

func refreshable(action: () async -> Void) -> some View

Marks this view as refreshable.

func renameAction(() -> Void) -> some View

Sets a closure to run for the rename action.

func renameAction(FocusState&lt;Bool>.Binding) -> some View

Sets the rename action in the environment to update focus state.

func replaceDisabled(Bool) -> some View

Prevents replace operations in a text editor.

func rotation3DEffect(Rotation3D, anchor: UnitPoint3D) -> some View

Rotates the view’s content by the specified 3D rotation value.

func rotation3DEffect(Angle, axis: (x: CGFloat, y: CGFloat, z: CGFloat), anchor: UnitPoint3D) -> some View

Rotates the view’s content by an angle about an axis that you specify as a tuple of elements.

func rotation3DEffect(Angle, axis: RotationAxis3D, anchor: UnitPoint3D) -> some View

Rotates the view’s content by an angle about an axis that you specify as a rotation axis value.

Deprecated

func rotation3DEffect(Angle, axis: RotationAxis3D, anchor: UnitPoint3D) -> ModifiedContent&lt;Self, _Rotation3DEffectAngleAxis>

Rotates the view’s content by an angle about an axis that you specify as a rotation axis value.

func rotation3DEffect(Angle, axis: (x: CGFloat, y: CGFloat, z: CGFloat), anchor: UnitPoint, anchorZ: CGFloat, perspective: CGFloat) -> some View

Renders a view’s content as if it’s rotated in three dimensions around the specified axis.

func rotationEffect(Angle, anchor: UnitPoint) -> some View

Rotates a view’s rendered output in two dimensions around the specified point.

func safeAreaInset&lt;V>(edge: VerticalEdge, alignment: HorizontalAlignment, spacing: CGFloat?, content: () -> V) -> some View

Shows the specified content above or below the modified view.

func safeAreaInset&lt;V>(edge: HorizontalEdge, alignment: VerticalAlignment, spacing: CGFloat?, content: () -> V) -> some View

Shows the specified content beside the modified view.

func safeAreaPadding(EdgeInsets) -> some View

Adds the provided insets into the safe area of this view.

func safeAreaPadding(CGFloat) -> some View

Adds the provided insets into the safe area of this view.

func safeAreaPadding(Edge.Set, CGFloat?) -> some View

Adds the provided insets into the safe area of this view.

func saturation(Double) -> some View

Adjusts the color saturation of this view.

func scaleEffect(CGFloat, anchor: UnitPoint3D) -> some View

Scales this view uniformly by the specified factor.

func scaleEffect(CGFloat, anchor: UnitPoint) -> ModifiedContent&lt;Self, _UniformScaleEffect>

Scales this view’s rendered output by the given amount in both the horizontal and vertical directions, relative to an anchor point.

func scaleEffect(CGSize, anchor: UnitPoint) -> some View

Scales this view’s rendered output by the given vertical and horizontal size amounts, relative to an anchor point.

func scaleEffect(CGFloat, anchor: UnitPoint) -> some View

Scales this view’s rendered output by the given amount in both the horizontal and vertical directions, relative to an anchor point.

func scaleEffect(Size3D, anchor: UnitPoint3D) -> some View

Scales this view uniformly by the specified size in each dimension.

func scaleEffect(x: CGFloat, y: CGFloat, anchor: UnitPoint) -> some View

Scales this view’s rendered output by the given horizontal and vertical amounts, relative to an anchor point.

func scaleEffect(x: CGFloat, y: CGFloat, z: CGFloat, anchor: UnitPoint3D) -> some View

Scales this view by the specified horizontal, vertical, and depth factors.

func scaledToFill() -> some View

Scales this view to fill its parent.

func scaledToFit() -> some View

Scales this view to fit its parent.

func scenePadding(Edge.Set) -> some View

Adds padding to the specified edges of this view using an amount that’s appropriate for the current scene.

func scenePadding(ScenePadding, edges: Edge.Set) -> some View

Adds a specified kind of padding to the specified edges of this view using an amount that’s appropriate for the current scene.

func scrollBounceBehavior(ScrollBounceBehavior, axes: Axis.Set) -> some View

Configures the bounce behavior of scrollable views along the specified axis.

func scrollClipDisabled(Bool) -> some View

Sets whether a scroll view clips its content to its bounds.

func scrollContentBackground(Visibility) -> some View

Specifies the visibility of the background for scrollable views within this view.

func scrollDisabled(Bool) -> some View

Disables or enables scrolling in scrollable views.

func scrollDismissesKeyboard(ScrollDismissesKeyboardMode) -> some View

Configures the behavior in which scrollable content interacts with the software keyboard.

func scrollIndicators(ScrollIndicatorVisibility, axes: Axis.Set) -> some View

Sets the visibility of scroll indicators within this view.

func scrollIndicatorsFlash(onAppear: Bool) -> some View

Flashes the scroll indicators of a scrollable view when it appears.

func scrollIndicatorsFlash(trigger: some Equatable) -> some View

Flashes the scroll indicators of scrollable views when a value changes.

func scrollInputBehavior(ScrollInputBehavior, for: ScrollInputKind) -> some View

Enables or disables scrolling in scrollable views when using particular inputs.

func scrollPosition(Binding&lt;ScrollPosition>, anchor: UnitPoint?) -> some View

Associates a binding to a scroll position with a scroll view within this view.

func scrollPosition(id: Binding&lt;(some Hashable)?>, anchor: UnitPoint?) -> some View

Associates a binding to be updated when a scroll view within this view scrolls.

func scrollTargetBehavior(some ScrollTargetBehavior) -> some View

Sets the scroll behavior of views scrollable in the provided axes.

func scrollTargetLayout(isEnabled: Bool) -> some View

Configures the outermost layout as a scroll target layout.

func scrollTransition(ScrollTransitionConfiguration, axis: Axis?, transition: (EmptyVisualEffect, ScrollTransitionPhase) -> some VisualEffect) -> some View

Applies the given transition, animating between the phases of the transition as this view appears and disappears within the visible region of the containing scroll view, or other container specified using the `coordinateSpace` parameter.

func scrollTransition(topLeading: ScrollTransitionConfiguration, bottomTrailing: ScrollTransitionConfiguration, axis: Axis?, transition: (EmptyVisualEffect, ScrollTransitionPhase) -> some VisualEffect) -> some View

Applies the given transition, animating between the phases of the transition as this view appears and disappears within the visible region of the containing scroll view, or other container specified using the `coordinateSpace` parameter.

func searchCompletion(String) -> some View

Associates a fully formed string with the value of this view when used as a search suggestion.

func searchCompletion&lt;T>(T) -> some View

Associates a search token with the value of this view when used as a search suggestion.

func searchDictationBehavior(TextInputDictationBehavior) -> some View

Configures the dictation behavior for any search fields configured by the searchable modifier.

func searchFocused(FocusState&lt;Bool>.Binding) -> some View

Modifies this view by binding the focus state of the search field associated with the nearest searchable modifier to the given Boolean value.

func searchFocused&lt;V>(FocusState&lt;V>.Binding, equals: V) -> some View

Modifies this view by binding the focus state of the search field associated with the nearest searchable modifier to the given value.

func searchPresentationToolbarBehavior(SearchPresentationToolbarBehavior) -> some View

Configures the search toolbar presentation behavior for any searchable modifiers within this view.

func searchScopes&lt;V, S>(Binding&lt;V>, activation: SearchScopeActivation, () -> S) -> some View

Configures the search scopes for this view with the specified activation strategy.

func searchScopes&lt;V, S>(Binding&lt;V>, scopes: () -> S) -> some View

Configures the search scopes for this view.

func searchSuggestions&lt;S>(() -> S) -> some View

Configures the search suggestions for this view.

func searchSuggestions(Visibility, for: SearchSuggestionsPlacement.Set) -> some View

Configures how to display search suggestions within this view.

func searchable&lt;C>(text: Binding&lt;String>, editableTokens: Binding&lt;C>, isPresented: Binding&lt;Bool>, placement: SearchFieldPlacement, prompt: LocalizedStringKey, token: (Binding&lt;C.Element>) -> some View) -> some View

Marks this view as searchable, which configures the display of a search field.

func searchable&lt;C>(text: Binding&lt;String>, editableTokens: Binding&lt;C>, isPresented: Binding&lt;Bool>, placement: SearchFieldPlacement, prompt: some StringProtocol, token: (Binding&lt;C.Element>) -> some View) -> some View

Marks this view as searchable, which configures the display of a search field.

func searchable&lt;C>(text: Binding&lt;String>, editableTokens: Binding&lt;C>, isPresented: Binding&lt;Bool>, placement: SearchFieldPlacement, prompt: Text?, token: (Binding&lt;C.Element>) -> some View) -> some View

Marks this view as searchable, which configures the display of a search field.

func searchable&lt;C>(text: Binding&lt;String>, editableTokens: Binding&lt;C>, placement: SearchFieldPlacement, prompt: LocalizedStringKey, token: (Binding&lt;C.Element>) -> some View) -> some View

Marks this view as searchable, which configures the display of a search field.

func searchable&lt;C>(text: Binding&lt;String>, editableTokens: Binding&lt;C>, placement: SearchFieldPlacement, prompt: Text?, token: (Binding&lt;C.Element>) -> some View) -> some View

Marks this view as searchable, which configures the display of a search field.

func searchable&lt;C>(text: Binding&lt;String>, editableTokens: Binding&lt;C>, placement: SearchFieldPlacement, prompt: some StringProtocol, token: (Binding&lt;C.Element>) -> some View) -> some View

Marks this view as searchable, which configures the display of a search field.

func searchable&lt;S>(text: Binding&lt;String>, isPresented: Binding&lt;Bool>, placement: SearchFieldPlacement, prompt: S) -> some View

Marks this view as searchable with programmatic presentation of the search field.

func searchable(text: Binding&lt;String>, isPresented: Binding&lt;Bool>, placement: SearchFieldPlacement, prompt: LocalizedStringKey) -> some View

Marks this view as searchable with programmatic presentation of the search field.

func searchable(text: Binding&lt;String>, isPresented: Binding&lt;Bool>, placement: SearchFieldPlacement, prompt: Text?) -> some View

Marks this view as searchable with programmatic presentation of the search field.

func searchable&lt;S>(text: Binding&lt;String>, placement: SearchFieldPlacement, prompt: S) -> some View

Marks this view as searchable, which configures the display of a search field.

func searchable(text: Binding&lt;String>, placement: SearchFieldPlacement, prompt: LocalizedStringKey) -> some View

Marks this view as searchable, which configures the display of a search field.

func searchable(text: Binding&lt;String>, placement: SearchFieldPlacement, prompt: Text?) -> some View

Marks this view as searchable, which configures the display of a search field.

func searchable&lt;S>(text: Binding&lt;String>, placement: SearchFieldPlacement, prompt: LocalizedStringKey, suggestions: () -> S) -> some View

Marks this view as searchable, which configures the display of a search field.

Deprecated

func searchable&lt;S>(text: Binding&lt;String>, placement: SearchFieldPlacement, prompt: Text?, suggestions: () -> S) -> some View

Marks this view as searchable, which configures the display of a search field.

Deprecated

func searchable&lt;V, S>(text: Binding&lt;String>, placement: SearchFieldPlacement, prompt: S, suggestions: () -> V) -> some View

Marks this view as searchable, which configures the display of a search field.

Deprecated

func searchable&lt;C, T>(text: Binding&lt;String>, tokens: Binding&lt;C>, isPresented: Binding&lt;Bool>, placement: SearchFieldPlacement, prompt: Text?, token: (C.Element) -> T) -> some View

Marks this view as searchable with text and tokens, as well as programmatic presentation.

func searchable&lt;C, T, S>(text: Binding&lt;String>, tokens: Binding&lt;C>, isPresented: Binding&lt;Bool>, placement: SearchFieldPlacement, prompt: S, token: (C.Element) -> T) -> some View

Marks this view as searchable with text and tokens, as well as programmatic presentation.

func searchable&lt;C, T>(text: Binding&lt;String>, tokens: Binding&lt;C>, isPresented: Binding&lt;Bool>, placement: SearchFieldPlacement, prompt: LocalizedStringKey, token: (C.Element) -> T) -> some View

Marks this view as searchable with text and tokens, as well as programmatic presentation.

func searchable&lt;C, T>(text: Binding&lt;String>, tokens: Binding&lt;C>, placement: SearchFieldPlacement, prompt: Text?, token: (C.Element) -> T) -> some View

Marks this view as searchable with text and tokens.

func searchable&lt;C, T, S>(text: Binding&lt;String>, tokens: Binding&lt;C>, placement: SearchFieldPlacement, prompt: S, token: (C.Element) -> T) -> some View

Marks this view as searchable with text and tokens.

func searchable&lt;C, T>(text: Binding&lt;String>, tokens: Binding&lt;C>, placement: SearchFieldPlacement, prompt: LocalizedStringKey, token: (C.Element) -> T) -> some View

Marks this view as searchable with text and tokens.

func searchable&lt;C, T>(text: Binding&lt;String>, tokens: Binding&lt;C>, suggestedTokens: Binding&lt;C>, isPresented: Binding&lt;Bool>, placement: SearchFieldPlacement, prompt: LocalizedStringKey, token: (C.Element) -> T) -> some View

Marks this view as searchable with text, tokens, and suggestions, as well as programmatic presentation.

func searchable&lt;C, T>(text: Binding&lt;String>, tokens: Binding&lt;C>, suggestedTokens: Binding&lt;C>, isPresented: Binding&lt;Bool>, placement: SearchFieldPlacement, prompt: Text?, token: (C.Element) -> T) -> some View

Marks this view as searchable with text, tokens, and suggestions, as well as programmatic presentation.

func searchable&lt;C, T, S>(text: Binding&lt;String>, tokens: Binding&lt;C>, suggestedTokens: Binding&lt;C>, isPresented: Binding&lt;Bool>, placement: SearchFieldPlacement, prompt: S, token: (C.Element) -> T) -> some View

Marks this view as searchable with text, tokens, and suggestions, as well as programmatic presentation.

func searchable&lt;C, T>(text: Binding&lt;String>, tokens: Binding&lt;C>, suggestedTokens: Binding&lt;C>, placement: SearchFieldPlacement, prompt: LocalizedStringKey, token: (C.Element) -> T) -> some View

Marks this view as searchable with text, tokens, and suggestions.

func searchable&lt;C, T>(text: Binding&lt;String>, tokens: Binding&lt;C>, suggestedTokens: Binding&lt;C>, placement: SearchFieldPlacement, prompt: Text?, token: (C.Element) -> T) -> some View

Marks this view as searchable with text, tokens, and suggestions.

func searchable&lt;C, T, S>(text: Binding&lt;String>, tokens: Binding&lt;C>, suggestedTokens: Binding&lt;C>, placement: SearchFieldPlacement, prompt: S, token: (C.Element) -> T) -> some View

Marks this view as searchable with text, tokens, and suggestions.

func sectionActions&lt;Content>(content: () -> Content) -> some View

Adds custom actions to a section.

func selectionDisabled(Bool) -> some View

Adds a condition that controls whether users can select this view.

func sensoryFeedback&lt;T>(SensoryFeedback, trigger: T) -> some View

Plays the specified `feedback` when the provided `trigger` value changes.

func sensoryFeedback&lt;T>(SensoryFeedback, trigger: T, condition: (T, T) -> Bool) -> some View

Plays the specified `feedback` when the provided `trigger` value changes and the `condition` closure returns `true`.

func sensoryFeedback&lt;T>(trigger: T, (T, T) -> SensoryFeedback?) -> some View

Plays feedback when returned from the `feedback` closure after the provided `trigger` value changes.

func shadow(color: Color, radius: CGFloat, x: CGFloat, y: CGFloat) -> some View

Adds a shadow to this view.

func sheet&lt;Content>(isPresented: Binding&lt;Bool>, onDismiss: (() -> Void)?, content: () -> Content) -> some View

Presents a sheet when a binding to a Boolean value that you provide is true.

func sheet&lt;Item, Content>(item: Binding&lt;Item?>, onDismiss: (() -> Void)?, content: (Item) -> Content) -> some View

Presents a sheet using the given item as a data source for the sheet’s content.

func simultaneousGesture&lt;T>(T, including: GestureMask) -> some View

Attaches a gesture to the view to process simultaneously with gestures defined by the view.

func simultaneousGesture&lt;T>(T, isEnabled: Bool) -> some View

Attaches a gesture to the view to process simultaneously with gestures defined by the view.

func simultaneousGesture&lt;T>(T, name: String, isEnabled: Bool) -> some View

Attaches a gesture to the view to process simultaneously with gestures defined by the view.

func speechAdjustedPitch(Double) -> some View

Raises or lowers the pitch of spoken text.

func speechAlwaysIncludesPunctuation(Bool) -> some View

Sets whether VoiceOver should always speak all punctuation in the text view.

func speechAnnouncementsQueued(Bool) -> some View

Controls whether to queue pending announcements behind existing speech rather than interrupting speech in progress.

func speechSpellsOutCharacters(Bool) -> some View

Sets whether VoiceOver should speak the contents of the text view character by character.

func springLoadingBehavior(SpringLoadingBehavior) -> some View

Sets the spring loading behavior this view.

func statusBar(hidden: Bool) -> some View

Sets the visibility of the status bar.

Deprecated

func statusBarHidden(Bool) -> some View

Sets the visibility of the status bar.

func strikethrough(Bool, pattern: Text.LineStyle.Pattern, color: Color?) -> some View

Applies a strikethrough to the text in this view.

func submitLabel(SubmitLabel) -> some View

Sets the submit label for this view.

func submitScope(Bool) -> some View

Prevents submission triggers originating from this view to invoke a submission action configured by a submission modifier higher up in the view hierarchy.

func supportedVolumeViewpoints(SquareAzimuth.Set) -> some View

Specifies which viewpoints are supported for the window bar and ornaments in a volume.

func swipeActions&lt;T>(edge: HorizontalEdge, allowsFullSwipe: Bool, content: () -> T) -> some View

Adds custom swipe actions to a row in a list.

func symbolEffect&lt;T>(T, options: SymbolEffectOptions, isActive: Bool) -> some View

Returns a new view with a symbol effect added to it.

func symbolEffect&lt;T, U>(T, options: SymbolEffectOptions, value: U) -> some View

Returns a new view with a symbol effect added to it.

func symbolEffectsRemoved(Bool) -> some View

Returns a new view with its inherited symbol image effects either removed or left unchanged.

func symbolRenderingMode(SymbolRenderingMode?) -> some View

Sets the rendering mode for symbol images within this view.

func symbolVariant(SymbolVariants) -> some View

Makes symbols within the view show a particular variant.

func tabItem&lt;V>(() -> V) -> some View

Sets the tab bar item associated with this view.

Deprecated

func tabViewCustomization(Binding&lt;TabViewCustomization>?) -> some View

Specifies the customizations to apply to the sidebar representation of the tab view.

func tabViewSidebarBottomBar&lt;Content>(content: () -> Content) -> some View

Adds a custom bottom bar to the sidebar of a tab view.

func tabViewSidebarFooter&lt;Content>(content: () -> Content) -> some View

Adds a custom footer to the sidebar of a tab view.

func tabViewSidebarHeader&lt;Content>(content: () -> Content) -> some View

Adds a custom header to the sidebar of a tab view.

func tabViewStyle&lt;S>(S) -> some View

Sets the style for the tab view within the current environment.

func tableColumnHeaders(Visibility) -> some View

Controls the visibility of a `Table`’s column header views.

func tableStyle&lt;S>(S) -> some View

Sets the style for tables within this view.

func tag&lt;V>(V, includeOptional: Bool) -> some View

Sets the unique tag value of this view.

func task&lt;T>(id: T, priority: TaskPriority, () async -> Void) -> some View

Adds a task to perform before this view appears or when a specified value changes.

func task(priority: TaskPriority, () async -> Void) -> some View

Adds an asynchronous task to perform before this view appears.

func textCase(Text.Case?) -> some View

Sets a transform for the case of the text contained in this view when displayed.

func textContentType(UITextContentType?) -> some View

Sets the text content type for this view, which the system uses to offer suggestions while the user enters text on an iOS or tvOS device.

func textContentType(NSTextContentType?) -> some View

Sets the text content type for this view, which the system uses to offer suggestions while the user enters text on macOS.

func textContentType(WKTextContentType?) -> some View

Sets the text content type for this view, which the system uses to offer suggestions while the user enters text on a watchOS device.

func textEditorStyle(some TextEditorStyle) -> some View

Sets the style for text editors within this view.

func textFieldStyle&lt;S>(S) -> some View

Sets the style for text fields within this view.

func textInputAutocapitalization(TextInputAutocapitalization?) -> some View

Sets how often the shift key in the keyboard is automatically enabled.

func textInputCompletion(String) -> some View

Associates a fully formed string with the value of this view when used as a text input suggestion

func textInputSuggestions&lt;S>(() -> S) -> some View

Configures the text input suggestions for this view.

func textInputSuggestions&lt;Data, Content>(Data, content: (Data.Element) -> Content) -> some View

Configures the text input suggestions for this view.

func textInputSuggestions&lt;Data, ID, Content>(Data, id: KeyPath&lt;Data.Element, ID>, content: (Data.Element) -> Content) -> some View

Configures the text input suggestions for this view.

func textRenderer&lt;T>(T) -> some View

Returns a new view such that any text views within it will use `renderer` to draw themselves.

func textScale(Text.Scale, isEnabled: Bool) -> some View

Applies a text scale to text in the view.

func textSelection&lt;S>(S) -> some View

Controls whether people can select text within this view.

func textSelectionAffinity(TextSelectionAffinity) -> some View

Sets the direction of a selection or cursor relative to a text character.

func tint(Color?) -> some View

Sets the tint color within this view.

func toggleStyle&lt;S>(S) -> some View

Sets the style for toggles in a view hierarchy.

func toolbar(Visibility, for: ToolbarPlacement...) -> some View

Specifies the visibility of a bar managed by SwiftUI.

func toolbar&lt;Content>(content: () -> Content) -> some View

Populates the toolbar or navigation bar with the specified items.

func toolbar&lt;Content>(content: () -> Content) -> some View

Populates the toolbar or navigation bar with the views you provide.

func toolbar&lt;Content>(id: String, content: () -> Content) -> some View

Populates the toolbar or navigation bar with the specified items, allowing for user customization.

func toolbar(removing: ToolbarDefaultItemKind?) -> some View

Remove a toolbar item present by default

func toolbarBackground&lt;S>(S, for: ToolbarPlacement...) -> some View

Specifies the preferred shape style of the background of a bar managed by SwiftUI.

func toolbarBackground(Visibility, for: ToolbarPlacement...) -> some View

Specifies the preferred visibility of backgrounds on a bar managed by SwiftUI.

func toolbarBackgroundVisibility(Visibility, for: ToolbarPlacement...) -> some View

Specifies the preferred visibility of backgrounds on a bar managed by SwiftUI.

func toolbarColorScheme(ColorScheme?, for: ToolbarPlacement...) -> some View

Specifies the preferred color scheme of a bar managed by SwiftUI.

func toolbarForegroundStyle&lt;S>(S, for: ToolbarPlacement...) -> some View

Specifies the preferred foreground style of bars managed by SwiftUI.

func toolbarItemHidden(Bool) -> some View

Hides an individual view within a control group toolbar item.

func toolbarRole(ToolbarRole) -> some View

Configures the semantic role for the content populating the toolbar.

func toolbarTitleDisplayMode(ToolbarTitleDisplayMode) -> some View

Configures the toolbar title display mode for this view.

func toolbarTitleMenu&lt;C>(content: () -> C) -> some View

Configure the title menu of a toolbar.

func toolbarVisibility(Visibility, for: ToolbarPlacement...) -> some View

Specifies the visibility of a bar managed by SwiftUI.

func touchBar&lt;Content>(TouchBar&lt;Content>) -> some View

Sets the Touch Bar content to be shown in the Touch Bar when applicable.

func touchBar&lt;Content>(content: () -> Content) -> some View

Sets the content that the Touch Bar displays.

func touchBarCustomizationLabel(Text) -> some View

Sets a user-visible string that identifies the view’s functionality.

func touchBarItemPresence(TouchBarItemPresence) -> some View

Sets the behavior of the user-customized view.

func touchBarItemPrincipal(Bool) -> some View

Sets principal views that have special significance to this Touch Bar.

func tracking(CGFloat) -> some View

Sets the tracking for the text in this view.

func transaction((inout Transaction) -> Void) -> some View

Applies the given transaction mutation function to all animations used within the view.

func transaction&lt;V>((inout Transaction) -> Void, body: (PlaceholderContentView&lt;Self>) -> V) -> some View

Applies the given transaction mutation function to all animations used within the `body` closure.

func transaction(value: some Equatable, (inout Transaction) -> Void) -> some View

Applies the given transaction mutation function to all animations used within the view.

func transform3DEffect(AffineTransform3D) -> some View

Applies a 3D transformation to the receiver.

func transformAnchorPreference&lt;A, K>(key: K.Type, value: Anchor&lt;A>.Source, transform: (inout K.Value, Anchor&lt;A>) -> Void) -> some View

Sets a value for the specified preference key, the value is a function of the key’s current value and a geometry value tied to the current coordinate space, allowing readers of the value to convert the geometry to their local coordinates.

func transformEffect(CGAffineTransform) -> some View

Applies an affine transformation to this view’s rendered output.

func transformEnvironment&lt;V>(WritableKeyPath&lt;EnvironmentValues, V>, transform: (inout V) -> Void) -> some View

Transforms the environment value of the specified key path with the given function.

func transformPreference&lt;K>(K.Type, (inout K.Value) -> Void) -> some View

Applies a transformation to a preference value.

func transition(AnyTransition) -> some View

Associates a transition with the view.

func transition&lt;T>(T) -> some View

Associates a transition with the view.

func truncationMode(Text.TruncationMode) -> some View

Sets the truncation mode for lines of text that are too long to fit in the available space.

func typeSelectEquivalent&lt;S>(S) -> some View

Sets an explicit type select equivalent text in a collection, such as a list or table.

func typeSelectEquivalent(Text?) -> some View

Sets an explicit type select equivalent text in a collection, such as a list or table.

func typeSelectEquivalent(LocalizedStringKey) -> some View

Sets an explicit type select equivalent text in a collection, such as a list or table.

func typesettingLanguage(Locale.Language, isEnabled: Bool) -> some View

Specifies the language for typesetting.

func typesettingLanguage(TypesettingLanguage, isEnabled: Bool) -> some View

Specifies the language for typesetting.

func underline(Bool, pattern: Text.LineStyle.Pattern, color: Color?) -> some View

Applies an underline to the text in this view.

func unredacted() -> some View

Removes any reason to apply a redaction to this view hierarchy.

func upperLimbVisibility(Visibility) -> some View

Sets the preferred visibility of the user’s upper limbs, while an `ImmersiveSpace` scene is presented.

func userActivity&lt;P>(String, element: P?, (P, NSUserActivity) -> ()) -> some View

Advertises a user activity type.

func userActivity(String, isActive: Bool, (NSUserActivity) -> ()) -> some View

Advertises a user activity type.

func visualEffect((EmptyVisualEffect, GeometryProxy) -> some VisualEffect) -> some View

Applies effects to this view, while providing access to layout information through a geometry proxy.

func visualEffect3D((EmptyVisualEffect, GeometryProxy3D) -> some VisualEffect) -> some View

Applies effects to this view, while providing access to layout information through a 3D geometry proxy.

func volumeBaseplateVisibility(Visibility) -> some View

Sets the visibility of the baseplate of a volume, which appears when a user looks towards the ‘floor’ of a volume and during resize. Both `automatic` and `visible` will show the baseplate. `hidden` will never show it.

func windowDismissBehavior(WindowInteractionBehavior) -> some View

Configures the dismiss functionality for the window enclosing `self`.

func windowFullScreenBehavior(WindowInteractionBehavior) -> some View

Configures the full screen functionality for the window enclosing `self`.

func windowMinimizeBehavior(WindowInteractionBehavior) -> some View

Configures the minimize functionality for the window enclosing `self`.

func windowResizeBehavior(WindowInteractionBehavior) -> some View

Configures the resize functionality for the window enclosing `self`.

func windowToolbarFullScreenVisibility(WindowToolbarFullScreenVisibility) -> some View

Configures the visibility of the window toolbar when the window enters full screen mode.

func writingToolsAffordanceVisibility(Visibility) -> some View

Specifies whether the system should show the Writing Tools affordance for text input views affected by the environment.

func writingToolsBehavior(WritingToolsBehavior) -> some View

Specifies the Writing Tools behavior for text and text input in the environment.

func zIndex(Double) -> some View

Controls the display order of overlapping views.

