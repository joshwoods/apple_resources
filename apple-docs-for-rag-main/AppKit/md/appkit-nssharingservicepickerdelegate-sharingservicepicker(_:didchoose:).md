

- AppKit
- NSSharingServicePickerDelegate
-  sharingServicePicker(\_:didChoose:) 

Instance Method

# sharingServicePicker(\_:didChoose:)

Tells the delegate that the person selected a sharing service for the current item.

macOS 10.8+

``` source
optional func sharingServicePicker(
    _ sharingServicePicker: NSSharingServicePicker,
    didChoose service: NSSharingService?
)
```

## Parameters 

`sharingServicePicker`  

The sharing service picker.

`service`  

The selected sharing service. Invoked to give the delegate to the sharing service that is about to be executed.

## Discussion

After someone chooses a service, the sharing service picker calls this method to let you know which service they picked. The sharing service receives the item sometime after this method returns.

## See Also

### Customizing Behavior

func sharingServicePicker(NSSharingServicePicker, delegateFor: NSSharingService) -> (any NSSharingServiceDelegate)?

Asks your delegate to provide an object that the selected sharing service can use as its delegate.

