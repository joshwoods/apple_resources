

- Kernel
- Hardware Families
- FireWire
-  FWSBP2FetchAgentWriteCallback 

Type Alias

# FWSBP2FetchAgentWriteCallback

macOS 10.0+

``` source
typedef void (*FWSBP2FetchAgentWriteCallback)(void *refCon, IOReturn status, IOFireWireSBP2ORB *orb);
```

## Parameters 

`refCon`  

Reference constant supplied when the notification was registered.

`status`  

Indicates success or failure of operation.

`orb`  

Indicates current last orb in chain.

## See Also

### Serial Bus Protocol 2

IOFireWireSBP2Login

Supplies the login maintenance and Normal Command ORB execution portions of the API.

IOFireWireSBP2ManagementORB

Supplies non login related management ORBs. Management ORBs can be executed independent of a login, if necessary. Management ORBs are created using the IOFireWireSBP2LUN interface.

IOFireWireSBP2ORB

Represents an SBP2 normal command ORB. Supplies the APIs for configuring normal command ORBs. This includes setting the command block and writing the page tables for I/O. The ORBs are executed using the submitORB method in IOFireWireSBP2Login.

FWSBP2LoginCallback

FWSBP2LoginCompleteParams

FWSBP2LoginCompleteParamsPtr

FWSBP2LoginResponse

FWSBP2LoginResponsePtr

FWSBP2LogoutCallback

FWSBP2LogoutCompleteParams

FWSBP2LogoutCompleteParamsPtr

FWSBP2ManagementCallback

FWSBP2NotifyCallback

FWSBP2NotifyParams

FWSBP2NotifyParamsPtr

FWSBP2ReconnectParams

FWSBP2ReconnectParamsPtr

FWSBP2StatusBlock

FWSBP2StatusCallback

