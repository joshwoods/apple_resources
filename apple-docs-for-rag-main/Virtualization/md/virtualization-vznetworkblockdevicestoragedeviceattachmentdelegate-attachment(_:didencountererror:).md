

- Virtualization
- VZNetworkBlockDeviceStorageDeviceAttachmentDelegate
-  attachment(\_:didEncounterError:) 

Instance Method

# attachment(\_:didEncounterError:)

The method the attachment object calls when the NBD client encounters a nonrecoverable error.

macOS 14.0+

``` source
optional func attachment(
    _ attachment: VZNetworkBlockDeviceStorageDeviceAttachment,
    didEncounterError error: any Error
)
```

## Parameters 

`attachment`  

The attachment object calling the delegate method.

`error`  

An NSError that describes the nonrecoverable error.

## Discussion

After the attachment object calls this method, the NBD client is in a nonfunctional state.

## See Also

### Responding to connectivity changes

func attachmentWasConnected(VZNetworkBlockDeviceStorageDeviceAttachment)

The method the attachment object calls when the NBD client successfully connects or reconnects with the server.

