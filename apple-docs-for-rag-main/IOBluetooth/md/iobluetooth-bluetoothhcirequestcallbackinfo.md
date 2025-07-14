

- IOBluetooth
-  BluetoothHCIRequestCallbackInfo 

Structure

# BluetoothHCIRequestCallbackInfo

macOS

``` source
struct BluetoothHCIRequestCallbackInfo
```

## Topics

### Initializers

init()

init(userCallback: mach_vm_address_t, userRefCon: mach_vm_address_t, internalRefCon: mach_vm_address_t, asyncIDRefCon: mach_vm_address_t, reserved: mach_vm_address_t)

### Instance Properties

var asyncIDRefCon: mach_vm_address_t

var internalRefCon: mach_vm_address_t

var reserved: mach_vm_address_t

var userCallback: mach_vm_address_t

var userRefCon: mach_vm_address_t

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Structures

struct BluetoothAFHHostChannelClassification

struct BluetoothAFHResults

struct BluetoothAMPCommandRejectReason

struct BluetoothAMPCreatePhysicalLinkResponseStatus

struct BluetoothAMPDisconnectPhysicalLinkResponseStatus

struct BluetoothAMPDiscoverResponseControllerStatus

struct BluetoothAMPGetAssocResponseStatus

struct BluetoothAMPGetInfoResponseStatus

struct BluetoothAMPManagerCode

struct BluetoothAuthenticationRequirementsValues

struct BluetoothCompanyIdentifers

struct BluetoothDeviceAddress

struct BluetoothEnhancedSynchronousConnectionInfo

struct BluetoothEventFilterCondition

struct BluetoothFeatureBits

