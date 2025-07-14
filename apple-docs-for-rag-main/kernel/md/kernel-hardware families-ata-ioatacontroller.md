

- Kernel
- Hardware Families
- ATA
-  IOATAController 

Class

# IOATAController

The base class for ata controller family. Provides the interface common to all ata bus controllers.

macOS 11.0+

``` source
class IOATAController : IOService
```

## Overview

The header doc for this class is incomplete. The source however is heavily commented and should be consulted until such time as complete header doc is available.

## Topics

### Miscellaneous

busCanDispatch

answers whether the bus is in state such that the next command can be dispatched.

dispatchNext

Causes the command at the front of the queue to dequeue, made the current command and begin execution.

handleCommand

Called by executeCommand() to handle the client command from the workloop context.

### DataTypes

ExpansionData

### Instance Variables

reserved

### Instance Methods

- ATAPISecondaryExists

- ATAPISlaveExistsDeprecated

- allocateDoubleBuffer

- asyncCommand

- asyncData

- asyncIO

- asyncStatus

- bitSigToNumeric

- busCanDispatch

- checkTimeout

- completeIO

- configureTFPointers

- dequeueFirstCommand

- determineATAPIState

- dispatchNext

- enqueueCommand

- executeCommand

- executeEventCallouts

- free

- getConfig

- getMetaClass

- handleBusReset

- handleCommand

- handleDeviceInterrupt

- handleExecIO

- handleOverrun

- handleQueueFlush

- handleRegAccess

- handleTimeout

- init

- issueCommand

- probe

- provideBusInfo

- readATAPIByteCount

- readExtRegister

- readExtRegister

- registerAccess

- scanForDrives

- selectConfig

- selectDevice

- selectIOTiming

- softResetBus

- start

- startDMA

- startTimer

- stopDMA

- stopTimer

- swapBytes16

- synchronousIO

- txDataIn

- txDataOut

- waitForU8Status

- writeExtRegister

- writeExtRegister

- writePacket

### Type Methods

+ executeCommandAction

+ timeoutOccured

## Relationships

### Inherits From

- IOService

