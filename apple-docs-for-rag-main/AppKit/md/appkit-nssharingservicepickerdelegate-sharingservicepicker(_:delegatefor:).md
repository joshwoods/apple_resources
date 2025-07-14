

- AppKit
- NSSharingServicePickerDelegate
-  sharingServicePicker(\_:delegateFor:) 

Instance Method

# sharingServicePicker(\_:delegateFor:)

Asks your delegate to provide an object that the selected sharing service can use as its delegate.

macOS 10.8+

``` source
optional func sharingServicePicker(
    _ sharingServicePicker: NSSharingServicePicker,
    delegateFor sharingService: NSSharingService
) -> (any NSSharingServiceDelegate)?
```

## Parameters 

`sharingServicePicker`  

The sharing service picker.

`sharingService`  

The selected sharing service.

## Return Value

An object that adopts the NSSharingServiceDelegate protocol.

## Discussion

The sharing service assigns the returned object to its delegate property.

## See Also

### Customizing Behavior

func sharingServicePicker(NSSharingServicePicker, didChoose: NSSharingService?)

Tells the delegate that the person selected a sharing service for the current item.

