

- Kernel
- Hardware Families
- FireWire
-  IOFWWriteQuadCommand 

Class

# IOFWWriteQuadCommand

An easier to use version of IOFWWriteCommand for use when the data to be transferred is small and an integer number of quads. Note that block read requests will be used for transfers greater than one quad unless setMaxPacket(4) is called. kMaxWriteQuads is the largest legal number of quads that this object can be asked to transfer (the data is copied into an internal buffer in init() and reinit()).

macOS 10.0+

``` source
class IOFWWriteQuadCommand : IOFWAsyncCommand
```

## Topics

### Instance Methods

- createMemberVariables

- createMemoryDescriptor

- destroyMemberVariables

- destroyMemoryDescriptor

- execute

- free

- getMetaClass

- gotPacket

- initAll

- initAll

- initWithController

- reinit

- reinit

- setDeferredNotify

- setQuads

## Relationships

### Inherits From

- IOFWAsyncCommand

