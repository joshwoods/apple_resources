

- System Configuration
-  kSCPropNetPPPAuthProtocol 

Global Variable

# kSCPropNetPPPAuthProtocol

The PPP key `AuthProtocol`, whose value is of type `CFArray`, containing elements of type `CFString`.

macOS 10.1+

``` source
let kSCPropNetPPPAuthProtocol: CFString
```

## Discussion

This key can be passed the following constants:

- `kSCValNetPPPAuthProtocolCHAP`, which has the value `CHAP`

- `kSCValNetPPPAuthProtocolEAP`, which has the value `EAP`

- `kSCValNetPPPAuthProtocolMSCHAP1`, which has the value `MSCHAP1`

- `kSCValNetPPPAuthProtocolMSCHAP2`, which has the value `MSCHAP2`

- `kSCValNetPPPAuthProtocolPAP`, which has the value `PAP`

## See Also

### Constants

let kSCPropNetPPPACSPEnabled: CFString

The PPP key `ACSPEnabled`, whose value is of type `CFNumber` and is equal to `0` or `1`.

let kSCPropNetPPPConnectTime: CFString

The PPP key `ConnectTime`, whose value is of type `CFNumber`.

let kSCPropNetPPPDeviceLastCause: CFString

The PPP key `DeviceLastCause`, whose value is of type `CFNumber`.

let kSCPropNetPPPDialOnDemand: CFString

The PPP key `DialOnDemand`, whose value is of type `CFNumber` and is equal to `0` or `1`.

let kSCPropNetPPPDisconnectOnFastUserSwitch: CFString

The PPP key `DisconnectOnFastUserSwitch`, whose value is of type `CFNumber` and is equal to `0` or `1`.

let kSCPropNetPPPDisconnectOnIdle: CFString

The PPP key `DisconnectOnIdle`, whose value is of type `CFNumber` and is equal to `0` or `1`.

let kSCPropNetPPPDisconnectOnIdleTimer: CFString

The PPP key `DisconnectOnIdleTimer`, whose value is of type `CFNumber`.

let kSCPropNetPPPDisconnectOnLogout: CFString

The PPP key `DisconnectOnLogout`, whose value is of type `CFNumber` and is equal to `0` or `1`.

let kSCPropNetPPPDisconnectOnSleep: CFString

The PPP key `DisconnectOnSleep`, whose value is of type `CFNumber` and is equal to `0` or `1`.

let kSCPropNetPPPDisconnectTime: CFString

The PPP key `DisconnectTime`, whose value is of type `CFNumber`.

let kSCPropNetPPPIdleReminderTimer: CFString

The PPP key `IdleReminderTimer`, whose value is of type `CFNumber`.

let kSCPropNetPPPIdleReminder: CFString

The PPP key `IdleReminder`, whose value is of type `CFNumber` and is equal to `0` or `1`.

let kSCPropNetPPPLastCause: CFString

The PPP key `LastCause`, whose value is of type `CFNumber`.

let kSCPropNetPPPLogfile: CFString

The PPP key `Logfile`, whose value is of type `CFString`.

let kSCPropNetPPPPlugins: CFString

The PPP key `Plugins`, whose value is of type `CFArray`, containing elements of type `CFString`.

Deprecated

