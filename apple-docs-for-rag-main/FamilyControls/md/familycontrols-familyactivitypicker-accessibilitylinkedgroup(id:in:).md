

- FamilyControls
- FamilyActivityPicker
-  accessibilityLinkedGroup(id:in:) 

Instance Method

# accessibilityLinkedGroup(id:in:)

Links multiple accessibility elements so that the user can quickly navigate from one element to another, even when the elements are not near each other in the accessibility hierarchy.

FamilyControlsSwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+watchOS 7.0+

``` source
nonisolated
func accessibilityLinkedGroup(
    id: ID,
    in namespace: Namespace.ID
) -> some View where ID : Hashable
```

## Parameters 

`id`  

A hashable identifier used to separate sets of linked elements within the same namespace. Elements with matching `namespace` and `id` will be linked together.

`namespace`  

The namespace to use to organize linked accessibility elements. All elements marked with `accessibilityLink` in this namespace and with the specified `id` will be linked together.

## Discussion

This can be useful to allow quickly jumping between content in a list and the same content shown in a detail view, for example. All elements marked with `accessibilityLinkedGroup` with the same namespace and identifier will be linked together.

## See Also

### Accessibility Navigation

func accessibilityRotor&lt;Content>(Text, entries: () -> Content) -> some View

Create an Accessibility Rotor with the specified user-visible label, and entries generated from the content closure.

func accessibilityRotor&lt;L, Content>(L, entries: () -> Content) -> some View

Create an Accessibility Rotor with the specified user-visible label, and entries generated from the content closure.

func accessibilityRotor&lt;Content>(LocalizedStringKey, entries: () -> Content) -> some View

Create an Accessibility Rotor with the specified user-visible label, and entries generated from the content closure.

func accessibilityRotor&lt;Content>(AccessibilitySystemRotor, entries: () -> Content) -> some View

Create an Accessibility Rotor replacing the specified system-provided Rotor.

func accessibilityRotor&lt;L, EntryModel, ID>(L, entries: [EntryModel], entryID: KeyPath&lt;EntryModel, ID>, entryLabel: KeyPath&lt;EntryModel, String>) -> some View

Create an Accessibility Rotor with the specified user-visible label and entries.

func accessibilityRotor&lt;EntryModel, ID>(Text, entries: [EntryModel], entryID: KeyPath&lt;EntryModel, ID>, entryLabel: KeyPath&lt;EntryModel, String>) -> some View

Create an Accessibility Rotor with the specified user-visible label and entries.

func accessibilityRotor&lt;EntryModel, ID>(LocalizedStringKey, entries: [EntryModel], entryID: KeyPath&lt;EntryModel, ID>, entryLabel: KeyPath&lt;EntryModel, String>) -> some View

Create an Accessibility Rotor with the specified user-visible label and entries.

func accessibilityRotor&lt;EntryModel, ID>(AccessibilitySystemRotor, entries: [EntryModel], entryID: KeyPath&lt;EntryModel, ID>, entryLabel: KeyPath&lt;EntryModel, String>) -> some View

Create an Accessibility Rotor replacing the specified system-provided Rotor.

func accessibilityRotor&lt;EntryModel>(Text, entries: [EntryModel], entryLabel: KeyPath&lt;EntryModel, String>) -> some View

Create an Accessibility Rotor with the specified user-visible label and entries.

func accessibilityRotor&lt;EntryModel>(LocalizedStringKey, entries: [EntryModel], entryLabel: KeyPath&lt;EntryModel, String>) -> some View

Create an Accessibility Rotor with the specified user-visible label and entries.

func accessibilityRotor&lt;EntryModel>(AccessibilitySystemRotor, entries: [EntryModel], entryLabel: KeyPath&lt;EntryModel, String>) -> some View

Create an Accessibility Rotor replacing the specified system-provided Rotor.

func accessibilityRotor&lt;L, EntryModel>(L, entries: [EntryModel], entryLabel: KeyPath&lt;EntryModel, String>) -> some View

Create an Accessibility Rotor with the specified user-visible label and entries.

func accessibilityRotor(Text, textRanges: [Range&lt;String.Index>]) -> some View

Create an Accessibility Rotor with the specified user-visible label and entries for each of the specified ranges. The Rotor will be attached to the current Accessibility element, and each entry will go the specified range of that element.

func accessibilityRotor(AccessibilitySystemRotor, textRanges: [Range&lt;String.Index>]) -> some View

Create an Accessibility Rotor replacing the specified system-provided Rotor. The Rotor will be attached to the current Accessibility element, and each entry will go the specified range of that element.

func accessibilityRotor&lt;L>(L, textRanges: [Range&lt;String.Index>]) -> some View

Create an Accessibility Rotor with the specified user-visible label and entries for each of the specified ranges. The Rotor will be attached to the current Accessibility element, and each entry will go the specified range of that element.

