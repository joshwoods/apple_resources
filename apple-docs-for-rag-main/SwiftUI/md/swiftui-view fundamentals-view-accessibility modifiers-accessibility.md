

- SwiftUI
- View fundamentals
- View
-  Accessibility modifiers 

API Collection

# Accessibility modifiers

Make your SwiftUI apps accessible to everyone, including people with disabilities.

## Overview

Like all Apple UI frameworks, SwiftUI comes with built-in accessibility support. The framework introspects common elements like navigation views, lists, text fields, sliders, buttons, and so on, and provides basic accessibility labels and values by default. You don’t have to do any extra work to enable these standard accessibility features.

SwiftUI also provides tools to help you enhance the accessibility of your app. For example, you can explicitly add accessibility labels to elements in your UI using the accessibilityLabel(_:) or the accessibilityValue(_:) view modifier.

To learn more about adding accessibility features to your app, see Accessibility fundamentals.

## Topics

### Labels

func accessibilityLabel(_:)

Adds a label to the view that describes its contents.

func accessibilityLabel(_:isEnabled:)

Adds a label to the view that describes its contents.

func accessibilityLabel&lt;V>(content: (PlaceholderContentView&lt;Self>) -> V) -> some View

Adds a label to the view that describes its contents.

func accessibilityInputLabels(_:)

Sets alternate input labels with which users identify a view.

func accessibilityInputLabels(_:isEnabled:)

Sets alternate input labels with which users identify a view.

func accessibilityLabeledPair&lt;ID>(role: AccessibilityLabeledPairRole, id: ID, in: Namespace.ID) -> some View

Pairs an accessibility element representing a label with the element for the matching content.

### Values

func accessibilityValue(_:)

Adds a textual description of the value that the view contains.

func accessibilityValue(_:isEnabled:)

Adds a textual description of the value that the view contains.

### Hints

func accessibilityHint(_:)

Communicates to the user what happens after performing the view’s action.

func accessibilityHint(_:isEnabled:)

Communicates to the user what happens after performing the view’s action.

### Actions

func accessibilityAction(AccessibilityActionKind, () -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

func accessibilityActions&lt;Content>(() -> Content) -> some View

Adds multiple accessibility actions to the view.

func accessibilityAction(named:_:)

Adds an accessibility action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

func accessibilityAction&lt;Label>(action: () -> Void, label: () -> Label) -> some View

Adds an accessibility action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

func accessibilityAction&lt;I, Label>(intent: I, label: () -> Label) -> some View

Adds an accessibility action labeled by the contents of `label` to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action. When the action is performed, the `intent` will be invoked.

func accessibilityAction&lt;I>(AccessibilityActionKind, intent: I) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility action representing `actionKind` to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action. When the action is performed, the `intent` will be invoked.

func accessibilityAction(named:intent:)

Adds an accessibility action labeled `name` to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action. When the action is performed, the `intent` will be invoked.

func accessibilityAdjustableAction((AccessibilityAdjustmentDirection) -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility adjustable action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

func accessibilityScrollAction((Edge) -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility scroll action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

### Gestures

func accessibilityActivationPoint(_:)

The activation point for an element is the location assistive technologies use to initiate gestures.

func accessibilityActivationPoint(_:isEnabled:)

The activation point for an element is the location assistive technologies use to initiate gestures.

func accessibilityDragPoint(_:description:)

The point an assistive technology should use to begin a drag interaction.

func accessibilityDragPoint(_:description:isEnabled:)

The point an assistive technology should use to begin a drag interaction.

func accessibilityDropPoint(_:description:)

The point an assistive technology should use to end a drag interaction.

func accessibilityDropPoint(_:description:isEnabled:)

The point an assistive technology should use to end a drag interaction.

func accessibilityDirectTouch(Bool, options: AccessibilityDirectTouchOptions) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Explicitly set whether this accessibility element is a direct touch area. Direct touch areas passthrough touch events to the app rather than being handled through an assistive technology, such as VoiceOver. The modifier accepts an optional `AccessibilityDirectTouchOptions` option set to customize the functionality of the direct touch area.

func accessibilityZoomAction((AccessibilityZoomGestureAction) -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility zoom action to the view. Actions allow assistive technologies, such as VoiceOver, to interact with the view by invoking the action.

### Elements

func accessibilityElement(children: AccessibilityChildBehavior) -> some View

Creates a new accessibility element, or modifies the AccessibilityChildBehavior of the existing accessibility element.

func accessibilityChildren&lt;V>(children: () -> V) -> some View

Replaces the existing accessibility element’s children with one or more new synthetic accessibility elements.

func accessibilityHidden(Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Specifies whether to hide this view from system accessibility features.

func accessibilityHidden(Bool, isEnabled: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Specifies whether to hide this view from system accessibility features.

### Custom controls

func accessibilityRepresentation&lt;V>(representation: () -> V) -> some View

Replaces one or more accessibility elements for this view with new accessibility elements.

func accessibilityRespondsToUserInteraction(Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Explicitly set whether this Accessibility element responds to user interaction and would thus be interacted with by technologies such as Switch Control, Voice Control or Full Keyboard Access.

func accessibilityRespondsToUserInteraction(Bool, isEnabled: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Explicitly set whether this Accessibility element responds to user interaction and would thus be interacted with by technologies such as Switch Control, Voice Control or Full Keyboard Access.

### Custom content

func accessibilityCustomContent(_:_:importance:)

Add additional accessibility information to the view.

### Working with rotors

func accessibilityRotor(_:entries:)

Create an Accessibility Rotor with the specified user-visible label, and entries generated from the content closure.

func accessibilityRotor(_:entries:entryID:entryLabel:)

Create an Accessibility Rotor with the specified user-visible label and entries.

func accessibilityRotor(_:entries:entryLabel:)

Create an Accessibility Rotor with the specified user-visible label and entries.

func accessibilityRotor(_:textRanges:)

Create an Accessibility Rotor with the specified user-visible label and entries for each of the specified ranges. The Rotor will be attached to the current Accessibility element, and each entry will go the specified range of that element.

### Configuring rotors

func accessibilityRotorEntry&lt;ID>(id: ID, in: Namespace.ID) -> some View

Defines an explicit identifier tying an Accessibility element for this view to an entry in an Accessibility Rotor.

func accessibilityLinkedGroup&lt;ID>(id: ID, in: Namespace.ID) -> some View

Links multiple accessibility elements so that the user can quickly navigate from one element to another, even when the elements are not near each other in the accessibility hierarchy.

func accessibilitySortPriority(Double) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets the sort priority order for this view’s accessibility element, relative to other elements at the same level.

### Focus

func accessibilityFocused(AccessibilityFocusState&lt;Bool>.Binding) -> some View

Modifies this view by binding its accessibility element’s focus state to the given boolean state value.

func accessibilityFocused&lt;Value>(AccessibilityFocusState&lt;Value>.Binding, equals: Value) -> some View

Modifies this view by binding its accessibility element’s focus state to the given state value.

### Traits

func accessibilityAddTraits(AccessibilityTraits) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds the given traits to the view.

func accessibilityRemoveTraits(AccessibilityTraits) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Removes the given traits from this view.

### Identity

func accessibilityIdentifier(String) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Uses the string you specify to identify the view.

func accessibilityIdentifier(String, isEnabled: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Uses the string you specify to identify the view.

### Color inversion

func accessibilityIgnoresInvertColors(Bool) -> some View

Sets whether this view should ignore the system Smart Invert setting.

### Content descriptions

func accessibilityTextContentType(AccessibilityTextContentType) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets an accessibility text content type.

func accessibilityHeading(AccessibilityHeadingLevel) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets the accessibility level of this heading.

### VoiceOver

func speechAdjustedPitch(Double) -> some View

Raises or lowers the pitch of spoken text.

func speechAlwaysIncludesPunctuation(Bool) -> some View

Sets whether VoiceOver should always speak all punctuation in the text view.

func speechAnnouncementsQueued(Bool) -> some View

Controls whether to queue pending announcements behind existing speech rather than interrupting speech in progress.

func speechSpellsOutCharacters(Bool) -> some View

Sets whether VoiceOver should speak the contents of the text view character by character.

### Charts

func accessibilityChartDescriptor&lt;R>(R) -> some View

Adds a descriptor to a View that represents a chart to make the chart’s contents accessible to all users.

### Large content

func accessibilityShowsLargeContentViewer() -> some View

Adds a default large content view to be shown by the large content viewer.

func accessibilityShowsLargeContentViewer&lt;V>(() -> V) -> some View

Adds a custom large content view to be shown by the large content viewer.

### Quick actions

func accessibilityQuickAction&lt;Style, Content>(style: Style, content: () -> Content) -> some View

Adds a quick action to be shown by the system when active.

func accessibilityQuickAction&lt;Style, Content>(style: Style, isActive: Binding&lt;Bool>, content: () -> Content) -> some View

Adds a quick action to be shown by the system when active.

## See Also

### Configuring view elements

Appearance modifiers

Configure a view’s foreground and background styles, controls, and visibility.

Text and symbol modifiers

Manage the rendering, selection, and entry of text in your view.

Auxiliary view modifiers

Add and configure supporting views, like toolbars and context menus.

Chart view modifiers

Configure charts that you declare with Swift Charts.

