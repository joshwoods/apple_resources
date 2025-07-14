

- SwiftUI
- TabContent
-  accessibilityValue(\_:isEnabled:) 

Instance Method

# accessibilityValue(\_:isEnabled:)

Adds a textual description of the value that the tab contains.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func accessibilityValue(
    _ valueDescription: Text,
    isEnabled: Bool = true
) -> some TabContent
```

Show all declarations

## Parameters 

`valueDescription`  

The accessibility value to apply.

`isEnabled`  

If true the accessibility value is applied; otherwise the accessibility value is unchanged.

## Discussion

Use this method to describe the value represented by a tab, but only if that’s different than the tab’s label such as when an icon represent information about a tab.

```
var body: some View {
    TabView {
        Tab {
            MessagesView()
        } label: {
            Text("Messages")
        }
        .badge(30)
        .accessibilityValue("30 Unread")
    }
}
```

