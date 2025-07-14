

- Local Authentication
- LAError
- LAError.Code
-  LAError.Code.appCancel 

Case

# LAError.Code.appCancel

The app canceled authentication.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
case appCancel
```

## Discussion

You receive this error if you call the invalidate() method while authentication is in process.

## See Also

### Cancellation

case systemCancel

The system canceled authentication.

case userCancel

The user tapped the cancel button in the authentication dialog.

