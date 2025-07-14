

- Local Authentication
- LAError
- LAError.Code
-  LAError.Code.systemCancel 

Case

# LAError.Code.systemCancel

The system canceled authentication.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+watchOS 3.0+

``` source
case systemCancel
```

## Discussion

This might happen if another app comes to the foreground while your app displays the authentication dialog.

## See Also

### Cancellation

case appCancel

The app canceled authentication.

case userCancel

The user tapped the cancel button in the authentication dialog.

