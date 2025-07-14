

- SwiftUI
- View
-  contactAccessButtonCaption(\_:) 

Instance Method

# contactAccessButtonCaption(\_:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
func contactAccessButtonCaption(_ caption: ContactAccessButton.Caption) -> some View
```

## See Also

### Managing contact access

func contactAccessButtonStyle(ContactAccessButton.Style) -> some View

func contactAccessPicker(isPresented: Binding&lt;Bool>, completionHandler: ([String]) -> ()) -> some View

Modally present UI which allows the user to select which contacts your app has access to.

