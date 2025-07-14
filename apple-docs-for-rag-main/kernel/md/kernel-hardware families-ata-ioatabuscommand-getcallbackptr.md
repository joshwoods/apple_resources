

- Kernel
- Hardware Families
- ATA
- IOATABusCommand
-  getCallbackPtr 

# getCallbackPtr

return the callback pointer

``` source
virtual IOATACompletionFunction* getCallbackPtr (
 void ); 
```

## See Also

### Miscellaneous

allocateCmd

factory method to create an instance of this class used by subclasses of IOATADevice

executeCallback

call the completion callback function

getBuffer

get pointer to the memory descriptor for this transaction

getByteCount

return the byte count for this transaction to transfer.

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

