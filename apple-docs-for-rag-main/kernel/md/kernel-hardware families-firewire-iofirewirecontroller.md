

- Kernel
- Hardware Families
- FireWire
-  IOFireWireController 

Class

# IOFireWireController

macOS 10.0+

``` source
class IOFireWireController : IOFireWireBus
```

## Topics

### Instance Methods

- AddUnitDirectory

- AssignCycleMaster

- FWSpeed

- FWSpeed

- RemoveUnitDirectory

- UpdateROM

- activateAsyncStreamReceivers

- activateMultiIsochReceiveListener

- activatePHYPacketListener

- addAllocatedChannel

- addIRMAllocation

- addToIRMAllocationSet

- allocAddress

- allocAsyncStreamReceiver

- allocTrans

- allocTrans

- allocateIRMBandwidthInGeneration

- allocateIRMChannelInGeneration

- allocatePseudoAddress

- asyncLock

- asyncLock

- asyncLockResponse

- asyncPHYPacket

- asyncRead

- asyncRead

- asyncReadResponse

- asyncStreamWrite

- asyncWrite

- asyncWrite

- asyncWrite

- beginIOCriticalSection

- buildTopology

- checkForDuplicateGUID

- checkGeneration

- checkProgress

- clientDoneWithMultiIsochReceivePacket

- clipMaxRec2K

- closeGate

- copyMapper

- countNodeIDChildren

- createAsyncPHYCommand

- createAsyncStreamCommand

- createAsyncStreamCommand

- createAsyncStreamListener

- createAuxiliary

- createDelayedCmd

- createDummyRegistryEntry

- createIRMAllocation

- createInitialAddressSpace

- createIsochChannel

- createLocalIsochPort

- createMultiIsochReceiveListener

- createPHYPacketListener

- createPendingQ

- createPhysicalAddressSpace

- createPseudoAddressSpace

- createTimeoutQ

- deactivateAsyncStreamReceivers

- deactivateMultiIsochReceiveListener

- deactivatePHYPacketListener

- delayedStateCommandInUse

- destroyPendingQ

- destroyTimeoutQ

- disablePhyPortOnSleepForNodeID

- disableSoftwareBusResets

- doBusReset

- doLockSpace

- doReadSpace

- doWriteSpace

- enableSoftwareBusResets

- endIOCriticalSection

- enterBusResetDisabledState

- enterLoggingMode

- finalize

- findKeyswitchDevice

- finishedBusScan

- free

- freeAddress

- freeAllAsyncStreamReceiver

- freePseudoAddress

- freeSecurity

- freeTrans

- getAddressSpace

- getAfterResetHandledQ

- getAsyncStreamReceiver

- getBroadcastSpeed

- getBusCycleTime

- getBusPowerManager

- getCycleTime

- getCycleTimeAndUpTime

- getExtendedTCode

- getGeneration

- getIRMNodeID

- getLink

- getLocalNodeID

- getMetaClass

- getPendingQ

- getPhysicalAccessMode

- getPortNumberFromIndex

- getResetTime

- getRootDir

- getSecurityMode

- getTimeoutQ

- getWorkLoop

- handleARxReqIntComplete

- handleAsyncCompletion

- handleAsyncTimeout

- hopCount

- hopCount

- inGate

- init

- initSecurity

- isCompleteRequest

- isLockRequest

- isPhysicalAccessEnabledForNodeID

- isQuadRequest

- makeRoot

- maxPackLog

- maxPackLog

- nodeIDtoDevice

- nodeMustBeRoot

- nodeMustNotBeRoot

- openGate

- physicalAccessProcessBusReset

- poweredStart

- processBusReset

- processCycle64Int

- processLockRequest

- processPHYPacket

- processRcvPacket

- processSelfIDs

- processTimeout

- processWriteRequest

- readDeviceROM

- releaseIRMBandwidthInGeneration

- releaseIRMChannelInGeneration

- removeAllocatedChannel

- removeAsyncStreamListener

- removeAsyncStreamReceiver

- removeFromIRMAllocationSet

- removeIRMAllocation

- requestTerminate

- resetBus

- scanningBus

- setGapCount

- setNodeIDPhysicalFilter

- setNodeSpeed

- setNodeSpeed

- setNodeSpeed

- setPhysicalAccessMode

- setPowerState

- setSecurityMode

- start

- startBusScan

- stop

- suspendBus

- systemWillShutdown

- terminateDevice

- updateDevice

- updatePlane

- useHalfSizePackets

### Type Methods

+ clockTick

+ consoleLockInterestHandler

+ delayedStateChange

+ getLocalNode

+ readROMGlue

+ resetStateChange

+ serverKeyswitchCallback

## Relationships

### Inherits From

- IOFireWireBus

## See Also

### Interfaces

IOFireWireSerialBusProtocolTransport

SCSI Protocol Driver Family for FireWire SBP2 Devices.

IOFireWireSBP2Target

Serves as bridge between IOFireWireUnit and IOFireWireLUN.

IOFireWireBus

IOFireWireBus is a public class the provides access to general FireWire functionality...

