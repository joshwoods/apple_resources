

- Kernel
- Hardware Families
- ATA
- IOATABusInfo
-  supportsExtendedLBA 

# supportsExtendedLBA

Supports 48-bit LBA if true. Used by clients of ATAControllers to find out about the bus.

``` source
bool supportsExtendedLBA(
 void ); 
```

## See Also

### Miscellaneous

atabusinfo

factory method

getDMAModes

bit-significant map of DMA mode(s) supported on the bus. Used by clients of ATAControllers to find out about the bus.

getPIOModes

returns the bit-significant map of PIO mode(s) supported on the bus. Used by clients of ATAControllers to find out about the bus.

getSocketType

returns the socket type, internal fixed, media-bay, PC-Card Used by clients of ATAControllers to find out about the bus

getUltraModes

bit-significant map of Ultra mode(s) supported on the bus. Used by clients of ATAControllers to find out about the bus.

getUnits

How many devices are present on bus. Used by clients of ATAControllers to find out about the bus.

maxBlocksExtended

The maximum number of 512-byte blocks this controller supports in a single Extended LBA transfer. Some controllers may be limited to less than the maximum sector count allowed under extended LBA protocol.

setDMAModes

Bit significant map of supported transfer modes. Set by ATAControllers.

setDMAQueued

Set true if supports DMA Queued Feature. Set by ATAControllers.

setExtendedLBA

Set true for supports 48-bit LBA. Set by ATAControllers.

setMaxBlocksExtended

value set by controllers to indicate the maximum number of blocks allowed in a single transfer of data. Some dma engines may not be capable of supporting the full 16-bit worth of sector count allowed under 48 bit extended LBA. Default is 256 blocks, same as standard ATA.

setOverlapped

Set true for supports overlapped packet feature set. Set by ATAControllers.

setPIOModes

Bit significant map of supported transfer modes. Set by ATAControllers.

setSocketType

internal fixed, media-bay, PC-Card. Set by ATAControllers.

setUltraModes

Bit significant map of supported transfer modes. Set by ATAControllers.

setUnits

set to indicate how many devices are on this bus. Set by ATAControllers.

supportsDMA

True = DMA supported on bus - inferred by looking at the DMA mode bits. Used by clients of ATAControllers to find out about the bus.

supportsDMAQueued

Supports DMA Queued Feature set if true. Used by clients of ATAControllers to find out about the bus.

supportsOverlapped

Supports overlapped packet feature set if true. Used by clients of ATAControllers to find out about the bus.

zeroData

set this object to a blank state.

