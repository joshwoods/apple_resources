

- AppKit
- NSSharingServicePicker
- NSSharingServicePicker.CollaborationModeRestriction
-  init(disabledMode:alertTitle:alertMessage:alertDismissButtonTitle:alertRecoverySuggestionButtonTitle:alertRecoverySuggestionButtonLaunch:) 

Initializer

# init(disabledMode:alertTitle:alertMessage:alertDismissButtonTitle:alertRecoverySuggestionButtonTitle:alertRecoverySuggestionButtonLaunch:)

macOS 15.0+

``` source
init(
    disabledMode: NSSharingCollaborationMode,
    alertTitle: String,
    alertMessage: String,
    alertDismissButtonTitle: String,
    alertRecoverySuggestionButtonTitle: String,
    alertRecoverySuggestionButtonLaunch alertRecoverySuggestionButtonLaunchURL: URL
)
```

## Parameters 

`disabledMode`  

The disabled type of sharing

`alertTitle`  

The alert title

`alertMessage`  

The alert message

`alertDismissButtonTitle`  

The label on the default alert button

`alertRecoverySuggestionButtonTitle`  

The label on the optional recovery suggestion button on the alert

`alertRecoverySuggestionButtonLaunchURL`  

The URL that is opened when the optional recovery suggestion button is selected

