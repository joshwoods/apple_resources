

- SwiftUI
- TabContent
-  accessibilityHint(\_:isEnabled:) 

Instance Method

# accessibilityHint(\_:isEnabled:)

Communicates to the user what happens after selecting the tab.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func accessibilityHint(
    _ hint: Text,
    isEnabled: Bool = true
) -> some TabContent
```

Show all declarations

## Parameters 

`hint`  

The accessibility hint to apply.

`isEnabled`  

If true the accessibility hint is applied; otherwise the accessibility hint is unchanged.

## Discussion

Provide a hint in the form of a brief phrase, like “Open shopping cart” or “Show downloaded attachments”.

```
var body: some View {
    TabView {
        Tab {
            MessagesView()
        } label: {
            Image(systemName: "play")
        }
        .accessibilityHint("Select videos to download")
    }
}
```

