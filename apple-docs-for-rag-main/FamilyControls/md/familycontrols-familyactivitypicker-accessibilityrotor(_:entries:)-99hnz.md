

- FamilyControls
- FamilyActivityPicker
-  accessibilityRotor(\_:entries:) 

Instance Method

# accessibilityRotor(\_:entries:)

Create an Accessibility Rotor replacing the specified system-provided Rotor.

FamilyControlsSwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+watchOS 8.0+

``` source
nonisolated
func accessibilityRotor(
    _ systemRotor: AccessibilitySystemRotor,
    @AccessibilityRotorContentBuilder entries: @escaping () -> Content
) -> some View where Content : AccessibilityRotorContent
```

## Parameters 

`systemRotor`  

The system-provided Rotor that will be overridden by this custom Rotor.

`entries`  

Content used to generate Rotor entries. This can include AccessibilityRotorEntry structs, as well as constructs such as if and ForEach.

## Discussion

An Accessibility Rotor is a shortcut for Accessibility users to quickly navigate to specific elements of the user interface, and optionally specific ranges of text within those elements. Replacing system Rotors this way is useful when the System Rotor does not automatically pick up elements that aren’t on-screen, such as elements far down in a `LazyVStack` or `List`.

In the following example, a Message application adds a Rotor allowing the user to navigate through all the ranges of text containing headings.

```
extension Message {
    // Ranges of special areas in the `content` text. Calculated
    // when `content` is set and then cached so that we don't have
    // to re-compute them.
    var contentHeadingRanges: [Range]
}

struct MessageContentView: View {
    TextEditor(.constant(message.content))
        .accessibilityRotor(.heading) {
            ForEach(range in message.contentHeadingRanges) {
                AccessibilityRotorEntry(textRange: range)
            }
        }
}
```

## See Also

### Accessibility Navigation

func accessibilityRotor&lt;Content>(Text, entries: () -> Content) -> some View

Create an Accessibility Rotor with the specified user-visible label, and entries generated from the content closure.

func accessibilityRotor&lt;L, Content>(L, entries: () -> Content) -> some View

Create an Accessibility Rotor with the specified user-visible label, and entries generated from the content closure.

func accessibilityRotor&lt;Content>(LocalizedStringKey, entries: () -> Content) -> some View

Create an Accessibility Rotor with the specified user-visible label, and entries generated from the content closure.

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

func accessibilityRotor(LocalizedStringKey, textRanges: [Range&lt;String.Index>]) -> some View

Create an Accessibility Rotor with the specified user-visible label and entries for each of the specified ranges. The Rotor will be attached to the current Accessibility element, and each entry will go the specified range of that element.

