

- Kernel
- Hardware Families
- FireWire
-  IOFireWireAVCTargetSpace 

Class

# IOFireWireAVCTargetSpace

object to centralize the AVC Target mode support

macOS 10.3+

``` source
class IOFireWireAVCTargetSpace : IOFWPseudoAddressSpace
```

## Overview

## Topics

### Miscellaneous

getAVCTargetSpace

returns the IOFireWireAVCTargetSpace object for the given FireWire bus

init

initializes the IOFireWireAVCTargetSpace object

publishAVCUnitDirectory

Creates a local AVC Unit directory if it doesn't already exist

### DataTypes

ExpansionData

### Instance Variables

reserved

### Instance Methods

- activateWithUserClient

- addSubunit

- canConnectDestPlug

- connectTargetPlugs

- deactivateWithUserClient

- disconnectTargetPlugs

- doWrite

- findAVCRequestHandler

- getMetaClass

- getSubunitInfo

- getSubunitPlugSignalFormat

- getTargetPlugConnection

- handleConnectCommand

- handleConnectionsCommand

- handleDisconnectCommand

- handleInputPlugSignalFormatCommand

- handleOutputPlugSignalFormatCommand

- handlePlugInfoCommand

- handlePowerCommand

- handleSignalSourceCommand

- handleSubUnitInfoCommand

- handleUnitInfoCommand

- init

- installAVCCommandHandler

- pcrModified

- publishAVCUnitDirectory

- setSubunitPlugSignalFormat

- subUnitOfTypeCount

- targetSendAVCResponse

### Type Methods

+ getAVCTargetSpace

## Relationships

### Inherits From

- IOFWPseudoAddressSpace

## See Also

### AVC Support

IOFireWireAVCAsynchronousCommand

IOFireWireAVCCommand

AVCCommandHandlerInfo

AVCConnectionRecord

AVCSubunitInfo

AVCConnectTargetPlugsInParams

AVCConnectTargetPlugsOutParams

AVCGetTargetPlugConnectionInParams

AVCGetTargetPlugConnectionOutParams

AVCSubunitPlugRecord

AVCUnitPlugRecord

AVCUnitPlugs

