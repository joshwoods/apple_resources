

- SwiftUI
- View
-  accessibilityRotor(\_:entries:) 

Instance Method

# accessibilityRotor(\_:entries:)

Create an Accessibility Rotor with the specified user-visible label, and entries generated from the content closure.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func accessibilityRotor(
    _ label: Text,
    @AccessibilityRotorContentBuilder entries: @escaping () -> Content
) -> some View where Content : AccessibilityRotorContent
```

Show all declarations

## Parameters 

`label`  

Localized label identifying this Rotor to the user.

`entries`  

Content used to generate Rotor entries. This can include AccessibilityRotorEntry structs, as well as constructs such as if and ForEach.

## Discussion

An Accessibility Rotor is a shortcut for Accessibility users to quickly navigate to specific elements of the user interface, and optionally specific ranges of text within those elements.

In the following example, a Message application creates a Rotor allowing users to navigate to specifically the messages originating from VIPs.

```
// `messages` is a list of `Identifiable` `Message`s.

ScrollView {
    LazyVStack {
        ForEach(messages) { message in
            MessageView(message)
        }
    }
}
.accessibilityElement(children: .contain)
.accessibilityRotor("VIPs") {
    // Not all the MessageViews are generated at once, the model knows
    // about all the messages.
    ForEach(messages) { message in
        // If the Message is from a VIP, make a Rotor entry for it.
        if message.isVIP {
            AccessibilityRotorEntry(message.subject, id: message.id)
        }
    }
}
```

## See Also

### Working with rotors

func accessibilityRotor(_:entries:entryID:entryLabel:)

Create an Accessibility Rotor with the specified user-visible label and entries.

func accessibilityRotor(_:entries:entryLabel:)

Create an Accessibility Rotor with the specified user-visible label and entries.

func accessibilityRotor(_:textRanges:)

Create an Accessibility Rotor with the specified user-visible label and entries for each of the specified ranges. The Rotor will be attached to the current Accessibility element, and each entry will go the specified range of that element.

