

- Kernel
- Hardware Families
- FireWire
-  IOFWReadQuadCommand 

Class

# IOFWReadQuadCommand

An easier to use version of IOFWReadCommand for use when the data to be transferred is an integer number of quads. Note that block read requests will be used for transfers greater than one quad unless setMaxPacket(4) is called.

macOS 10.0+

``` source
class IOFWReadQuadCommand : IOFWAsyncCommand
```

## Topics

### Instance Methods

- createMemberVariables

- destroyMemberVariables

- execute

- free

- getMetaClass

- gotPacket

- initAll

- initAll

- reinit

- reinit

- setPingTime

## Relationships

### Inherits From

- IOFWAsyncCommand

