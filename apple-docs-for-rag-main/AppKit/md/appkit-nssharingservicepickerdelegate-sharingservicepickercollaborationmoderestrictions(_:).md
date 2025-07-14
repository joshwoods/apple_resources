

- AppKit
- NSSharingServicePickerDelegate
-  sharingServicePickerCollaborationModeRestrictions(\_:) 

Instance Method

# sharingServicePickerCollaborationModeRestrictions(\_:)

Used to specify the case where the share picker should not support some modes of sharing even if they are supported by the items being shared. Disabling all possible modes at the same time is not supported behavior.

macOS 15.0+

``` source
optional func sharingServicePickerCollaborationModeRestrictions(_ sharingServicePicker: NSSharingServicePicker) -> [NSSharingServicePicker.CollaborationModeRestriction]?
```

