

- SwiftUI
- View
-  contactAccessButtonStyle(\_:) 

Instance Method

# contactAccessButtonStyle(\_:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
func contactAccessButtonStyle(_ style: ContactAccessButton.Style) -> some View
```

## See Also

### Managing contact access

func contactAccessButtonCaption(ContactAccessButton.Caption) -> some View

func contactAccessPicker(isPresented: Binding&lt;Bool>, completionHandler: ([String]) -> ()) -> some View

Modally present UI which allows the user to select which contacts your app has access to.

