

- Kernel
- Hardware Families
- ATA
-  IOATABusCommand 

Class

# IOATABusCommand

macOS 11.0+

``` source
class IOATABusCommand : IOATACommand
```

## Overview

ATA Device (disk) drivers should use the superclass, IOATACommand and may not derive or use any subclass of IOATACommand.

IOATABusCommand is the subclass of IOATACommand used by IOATAControllers. Controller classes may override this class to provide additional fields as their needs dictate or may use this as a concrete class if it is sufficient.

IOATAControllers are always paired with specific IOATADevices and each specific subclass of IOATADevice is in turn the factory method for IOATACommands for use by disk drivers.

In this manner, mass-storage device drivers (disk drivers, clients of ATA bus controllers) see only the generalized interface of IOATADevice and the generalized interface of IOATACommand. This provides isolation from specific bus details for disk drivers and offers flexibility to controllers to add per-command fields and state variables for their own internal use.

## Topics

### Miscellaneous

allocateCmd

factory method to create an instance of this class used by subclasses of IOATADevice

executeCallback

call the completion callback function

getBuffer

get pointer to the memory descriptor for this transaction

getByteCount

return the byte count for this transaction to transfer.

getCallbackPtr

return the callback pointer

getFlags

return the flags for this command.

getOpcode

return the command opcode

getPacketData

return pointer to the array of packet data.

getPacketSize

return the size of atapi packet if any.

getPosition

the position within the memory buffer for the transaction.

getRegMask

get the register mask for desired regs

getTaskFilePtr

return the taskfile structure pointer.

getTimeoutMS

return the timeout value for this command

getTransferChunkSize

number of bytes between interrupts.

getUnit

return the unit id (0 primary, 1 secondary)

init

Zeroes all data, returns false if allocation fails. protected.

setActualTransfer

set the byte count of bytes actually transferred.

setCommandInUse

mark the command as being in progress.

setResult

set the result code

zeroCommand

set to blank state, call prior to re-use of this object

### DataTypes

ExpansionData

### Instance Variables

syncer

state

reserved

queueChain

### Instance Methods

- executeCallback

- getBuffer

- getByteCount

- getCallbackPtr

- getFlags

- getMetaClass

- getOpcode

- getPacketData

- getPacketSize

- getPosition

- getRegMask

- getTaskFilePtr

- getTimeoutMS

- getTransferChunkSize

- getUnit

- init

- setActualTransfer

- setCommandInUse

- setResult

- zeroCommand

### Type Methods

+ allocateCmd

## Relationships

### Inherits From

- IOATACommand

