

- Kernel
- Hardware Families
- ATA
- IOATACommand
-  zeroCommand 

# zeroCommand

set to blank state, MUST call prior to re-use of this object

``` source
virtual void zeroCommand(
 void); 
```

## See Also

### Miscellaneous

getActualTransfer

The byte count on the ending result, as best as can be determined by the controller. May be zero, but partial transfer may have occurred on error in some cases.

getBuffer

the IOMemoryDescriptor used in this transaction.

getCommandInUse

returns true if IOATAController is still in control of the command.

getCylHi

Taskfile access. Registers are named in accordance with ATA Standards conventions

getCylLo

Taskfile access. Registers are named in accordance with ATA Standards conventions

getDevice_Head

Taskfile access. Registers are named in accordance with ATA Standards conventions

getEndErrorReg

If the error bit was set in the status register, the value of the error register is returned at the end of a command.

getEndStatusReg

the value of the status register on the end of the command.

getErrorReg

Taskfile access. Registers are named in accordance with ATA Standards conventions

getResult

IOReturn value of the result of this command. ATA family errors are defined in IOATATypes.h

getSectorCount

Taskfile access. Registers are named in accordance with ATA Standards conventions

getSectorNumber

Taskfile access. Registers are named in accordance with ATA Standards conventions

getStatus

Taskfile access. Registers are named in accordance with ATA Standards conventions

setBuffer

set the IIOMemoryDescriptor for this transaction.

setByteCount

set the byte count for this transaction. Should agree with the device command and the memory descriptor in use.

setCallbackPtr

set the function pointer to call when this command completes.

setCommand

Taskfile access. Registers are named in accordance with ATA Standards conventions

setCylHi

Taskfile access. Registers are named in accordance with ATA Standards conventions

setCylLo

Taskfile access. Registers are named in accordance with ATA Standards conventions

setDevice_Head

Taskfile access. Registers are named in accordance with ATA Standards conventions

setFeatures

Taskfile access. Registers are named in accordance with ATA Standards conventions

setFlags

set the flags for this command, as defined in IOATATypes.

setLBA28

convenience method that sets the taskfile registers into a 28-bit LBA address, with unit selected and LBA bit set. return err if param out of range, return kIOSuccess (kATANoErr) = 0 on return if successful

setOpcode

command opcode as defined in IOATATypes.

setPacketCommand

ATAPI command packet max size is 16 bytes. Makes deep copy of data.

setPosition

used to set an offset into the memory descriptor for this transfer.

setRegMask

used when accessing registers or reading registers on an error result. Mask is defined in IOATATypes.h

setSectorCount

Taskfile access. Registers are named in accordance with ATA Standards conventions

setSectorNumber

Taskfile access. Registers are named in accordance with ATA Standards conventions

setTimeoutMS

how long to allow this command to complete, in milliseconds, once issued to the hardware. if the time period expires, this command will return with a timeout error.

setTransferChunkSize

set the size of transfer between intervening interrupts. necessary when doing PIO Read/Write Multiple, etc. so the controller knows when to expect an interrupt during multi-sector data transfers.

setUnit

set the unit number for this command.

