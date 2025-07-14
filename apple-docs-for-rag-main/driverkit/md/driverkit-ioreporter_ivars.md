

- DriverKit
-  IOReporter_IVars 

Structure

# IOReporter_IVars

DriverKitiOSiPadOSmacOS

``` source
struct IOReporter_IVars;
```

## Topics

### Instance Properties

channelDimension

channelNames

channelType

configLock

driver_id

elements

enableCounts

enabled

nChannels

nElements

reporterConfigIsLocked

reporterIsLocked

reporterLock

swapElements

swapEnableCounts

unit

### Instance Methods

IOReporter_IVars

Establishes the parameters of all channels for this reporter instance

copyChannelIDs

copyElementValues

getChannelIndex

getChannelIndices

getElementValues

getFirstElementIndex

handleAddChannelSwap

handleConfigureReport

handleCreateLegend

handleSwapCleanup

handleSwapPrepare

handleUpdateReport

lockReporter

lockReporterConfig

setElementValues

unlockReporter

unlockReporterConfig

updateChannelValues

updateReportChannel

Internal method to extract channel data to a destination.

valid

IOReporter_IVars

### Type Methods

legendWith

## Relationships

### Inherited By

- IOHistogramReporter_IVars
- IOSimpleReporter_IVars
- IOStateReporter_IVars

## See Also

### Data Types

IOCallOnceBlock

IOCallOnceFlag

IOCommand

IOCommandPool

IOCommandPoolPtr

IOCommandPtr

IODMACommand

An object that converts memory references to I/O bus addresses.

IODMACommandSpecification

IODispatchAction

IOHistogramReporter_IVars

IOReportLegendEntry

IOSimpleReporter_IVars

IOStateReporter_IVars

IOStateReporter_valueSelector

IVarsInvalidator

