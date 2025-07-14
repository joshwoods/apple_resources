

- SwiftUI
- View
-  accessibilityRotor(\_:entries:entryID:entryLabel:) 

Instance Method

# accessibilityRotor(\_:entries:entryID:entryLabel:)

Create an Accessibility Rotor with the specified user-visible label and entries.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func accessibilityRotor(
    _ rotorLabel: Text,
    entries: [EntryModel],
    entryID: KeyPath,
    entryLabel: KeyPath
) -> some View where ID : Hashable
```

Show all declarations

## Parameters 

`rotorLabel`  

Localized label identifying this Rotor to the user.

`entries`  

An array of values that will be used to generate the entries of the Rotor.

`entryID`  

Key path on the entry type that can be used to generate an identifier for the Entry. The identifiers must match up with identifiers in `ForEach` or explicit `id` calls within the `ScrollView`.

`entryLabel`  

Key path on the entry type that can be used to get a user-visible label for every Rotor entry. This is used on macOS when the user opens the list of entries for the Rotor.

## Discussion

An Accessibility Rotor is a shortcut for Accessibility users to quickly navigate to specific elements of the user interface, and optionally specific ranges of text within those elements.

Using this modifier requires that the Rotor be attached to a `ScrollView`, or an Accessibility Element directly within a `ScrollView`, such as a `ForEach`. When the user navigates to entries from this Rotor, SwiftUI will automatically scroll them into place as needed.

In the following example, a Message application creates a Rotor allowing users to navigate to specifically the messages originating from VIPs.

```
// `messages` is a list of `Message`s that have a `subject` and a
// `uuid`. `vipMessages` is a filtered version of that list
// containing only messages from VIPs.
ScrollView {
    LazyVStack {
        ForEach(messages) { message in
            MessageView(message)
        }
    }
}
.accessibilityElement(children: .contain)
.accessibilityRotor("VIPs", entries: vipMessages,
    id: \.uuid, label: \.subject)
```

## See Also

### Working with rotors

func accessibilityRotor(_:entries:)

Create an Accessibility Rotor with the specified user-visible label, and entries generated from the content closure.

func accessibilityRotor(_:entries:entryLabel:)

Create an Accessibility Rotor with the specified user-visible label and entries.

func accessibilityRotor(_:textRanges:)

Create an Accessibility Rotor with the specified user-visible label and entries for each of the specified ranges. The Rotor will be attached to the current Accessibility element, and each entry will go the specified range of that element.

