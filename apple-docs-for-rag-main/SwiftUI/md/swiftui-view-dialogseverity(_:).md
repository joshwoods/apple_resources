

- SwiftUI
- View
-  dialogSeverity(\_:) 

Instance Method

# dialogSeverity(\_:)

macOS 13.0+watchOS 10.0+

``` source
nonisolated
func dialogSeverity(_ severity: DialogSeverity) -> some View
```

## Parameters 

`severity`  

The severity to use for confirmation dialogs and alerts.

## See Also

### Configuring a dialog

func dialogIcon(Image?) -> some View

Configures the icon used by dialogs within this view.

func dialogIcon(Image?) -> some Scene

Configures the icon used by alerts.

func dialogSeverity(DialogSeverity) -> some Scene

Sets the severity for alerts.

func dialogSuppressionToggle(isSuppressed: Binding&lt;Bool>) -> some View

Enables user suppression of dialogs and alerts presented within `self`, with a default suppression message on macOS. Unused on other platforms.

func dialogSuppressionToggle(isSuppressed: Binding&lt;Bool>) -> some Scene

Enables user suppression of an alert with a custom suppression message.

func dialogSuppressionToggle(_:isSuppressed:)

Enables user suppression of dialogs and alerts presented within `self`, with a custom suppression message on macOS. Unused on other platforms.

