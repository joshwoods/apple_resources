

- FamilyControls
- FamilyActivityPicker
-  accessibilitySortPriority(\_:) 

Instance Method

# accessibilitySortPriority(\_:)

Sets the sort priority order for this view’s accessibility element, relative to other elements at the same level.

FamilyControlsSwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+watchOS 7.0+

``` source
nonisolated
func accessibilitySortPriority(_ sortPriority: Double) -> ModifiedContent
```

## Discussion

Higher numbers are sorted first. The default sort priority is zero.

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

