

- RealityKit
- RealityViewContent
- RealityViewContent.Body
-  accessibilityRotor(\_:entries:) 

Instance Method

# accessibilityRotor(\_:entries:)

Create an Accessibility Rotor with the specified user-visible label, and entries generated from the content closure.

RealityKitSwiftUIiOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
nonisolated
func accessibilityRotor(
    _ labelKey: LocalizedStringKey,
    @AccessibilityRotorContentBuilder entries: @escaping () -> Content
) -> some View where Content : AccessibilityRotorContent
```

## Parameters 

`labelKey`  

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
    // Not all the MessageViews are generated at once, the model
    // knows about all the messages.
    ForEach(messages) { message in
        // If the Message is from a VIP, make a Rotor entry for it.
        if message.isVIP {
            AccessibilityRotorEntry(message.subject, id: message.id)
        }
    }
}
```

