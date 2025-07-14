

- Virtualization
- VZNetworkBlockDeviceStorageDeviceAttachmentDelegate
-  attachmentWasConnected(\_:) 

Instance Method

# attachmentWasConnected(\_:)

The method the attachment object calls when the NBD client successfully connects or reconnects with the server.

macOS 14.0+

``` source
optional func attachmentWasConnected(_ attachment: VZNetworkBlockDeviceStorageDeviceAttachment)
```

## Parameters 

`attachment`  

The attachment object calling the delegate method.

## Discussion

Connection with the server takes place when the VM is first started, and reconnection attempts take place when the connection times out or when the NBD client has encountered a recoverable error, such as an I/O error from the server. The Virtualization framework may call this method multiple times during a VM’s life cycle. Reconnections are transparent to the guest.

## See Also

### Responding to connectivity changes

func attachment(VZNetworkBlockDeviceStorageDeviceAttachment, didEncounterError: any Error)

The method the attachment object calls when the NBD client encounters a nonrecoverable error.

