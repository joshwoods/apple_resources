

- Kernel
- Hardware Families
- ATA
- IOExtendedLBA
-  zeroData 

# zeroData

convenience method that zeros out the lba, sector count, features, device, and command member variables

``` source
virtual void zeroData(
 void); 
```

## See Also

### Miscellaneous

getCommand

Taskfile access. Registers are named in accordance with ATA Standards conventions

getDevice

Taskfile access. Registers are named in accordance with ATA Standards conventions

getExtendedLBA

convenience method that gets a 48-bit LBA

getFeatures16

Taskfile access. Registers are named in accordance with ATA Standards conventions

getLBAHigh16

convenience method that gets the high 16 bits of a 48-bit LBA

getLBALow16

convenience method that gets the lower 16 bits of a 48-bit LBA

getLBAMid16

convenience method that gets the middle 16 bits of a 48-bit LBA

getSectorCount16

Taskfile access. Registers are named in accordance with ATA Standards conventions

setCommand

Taskfile access. Registers are named in accordance with ATA Standards conventions

setDevice

Taskfile access. Registers are named in accordance with ATA Standards conventions

setExtendedLBA

convenience method that sets the taskfile registers into a 48-bit LBA address, along with sector count, and unit selected and LBA bit set

setFeatures16

Taskfile access. Registers are named in accordance with ATA Standards conventions

setLBAHigh16

convenience method that sets the high 16 bits of a 48-bit LBA

setLBALow16

convenience method that sets the lower 16 bits of a 48-bit LBA

setLBAMid16

convenience method that sets the middle 16 bits of a 48-bit LBA

setSectorCount16

Taskfile access. Registers are named in accordance with ATA Standards conventions

