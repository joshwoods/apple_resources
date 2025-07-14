

- DriverKit
- IOReporter_IVars
-  legendWith 

Static Method

# legendWith

DriverKitiOSiPadOSmacOS

``` source
static OSSharedPtr legendWith(OSArray * channelIDs, OSArray * channelNames, IOReportChannelType channelType, IOReportUnit unit);
```

## Parameters 

`channelIDs`  

- OSArray of OSNumber(uint64_t) channels IDs.

`channelNames`  

- parrallel OSArray of OSSymbol(rich names)

`channelType`  

- the type of all channels in this legend

`unit`  

- The unit for the quantity recorded by this reporter object

## Return Value

An IOReportLegendEntry object or NULL on failure

## Discussion

This static method is the main legend creation function. It is called by IOReporter sub-classes and is responsible for building an IOReportLegendEntry corresponding to this reporter object. This legend entry may be extended by the sub-class of IOReporter if required.

Locking: SAFE to call concurrently (no static globals), MAY BLOCK

