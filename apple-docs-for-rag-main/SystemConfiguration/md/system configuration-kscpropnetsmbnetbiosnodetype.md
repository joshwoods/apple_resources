

- System Configuration
-  kSCPropNetSMBNetBIOSNodeType 

Global Variable

# kSCPropNetSMBNetBIOSNodeType

The SMB key `NetBIOSNodeType`, whose value is of type `CFString`.

macOS 10.5+

``` source
let kSCPropNetSMBNetBIOSNodeType: CFString
```

## Discussion

This key can be passed the following constants:

- `kSCValNetSMBNetBIOSNodeTypeBroadcast`, which has the value `Broadcast`

- `kSCValNetSMBNetBIOSNodeTypePeer`, which has the value `Peer`

- `kSCValNetSMBNetBIOSNodeTypeMixed`, which has the value `Mixed`

- `kSCValNetSMBNetBIOSNodeTypeHybrid`, which has the value `Hybrid`

## See Also

### Constants

let kSCPropNetSMBNetBIOSName: CFString

The SMB key `NetBIOSName`, whose value is of type `CFString`.

let kSCPropNetSMBWINSAddresses: CFString

The SMB key `WINSAddresses`, whose value is of type `CFArray`, containing elements of type `CFString`.

let kSCPropNetSMBWorkgroup: CFString

The SMB key `Workgroup`, whose value is of type `CFString`.

