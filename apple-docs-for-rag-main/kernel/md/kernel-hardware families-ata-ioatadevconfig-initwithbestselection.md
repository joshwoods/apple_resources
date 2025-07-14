

- Kernel
- Hardware Families
- ATA
- IOATADevConfig
-  initWithBestSelection 

# initWithBestSelection

Handy initializer: pass the 512-byte result of the Identify Device or Identify Packet Device in endian-order for your platform (byte-swapped on PPC) and the IOATABusInfo object for the bus. The object will initialize all fields and select the best transfer modes that match on bus and device. If the return value was 0 (success or noErr), then a matching mode is supported. Examine the PIO and UDMA/DMA fields and to generate the apropriate SET FEATURES parameters for your drive and send this initialised object to the IOATAController when requesting a speed configuration. failure means no supported transfer modes matched between bus and device info.

``` source
IOReturn initWithBestSelection(
 const UInt16 *identifyData,
 IOATABusInfo *busInfo); 
```

## Parameters 

`identifyData`  

512 bytes of data obtained from the device via IDENTIFY DEVICE or IDENTIFY PACKET DEVICE command.

`busInfo`  

pointer to an IOATAbusInfo object obtained from a previous atanub-\>provideBusInfo() call.

## Return Value

kIOSuccess (0) when a matching transfer mode is available between the device and controller.

## See Also

### Miscellaneous

atadevconfig

static creator function.

bitSigToNumeric

converts a bit-significant field to a numerical value. Note that a bit field of 0x00 has no defined result.

getDMACycleTime

getDMAMode

getPacketConfig

getPIOCycleTime

getPIOMode

getUltraMode

setDMACycleTime

setDMAMode

setPacketConfig

For ATAPI devices, if the device asserts interrupt after the Packet Command when it is ready to accept the packet, set this value to true (mostly older devices). If the device accepts the packet only by asserting DRQ bit in status, then set this value false. Tells the bus controller whether to wait for packet acceptance or set pending interrupt.

setPIOCycleTime

setPIOMode

setUltraMode

