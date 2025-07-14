

- DriverKit
-  IOCommandPool 

Class

# IOCommandPool

DriverKitiOSiPadOSmacOS

``` source
class IOCommandPool;
```

## Overview

The IOCommandPool class is used to manipulate a pool of commands which inherit from IOCommand. The caller must put commands in the pool by creating the command (via the controller’s factory method or a memory allocation) and calling the returnCommand method with the newly created command as its argument.

## Topics

### Instance Methods

free

gatedGetCommand

gatedReturnCommand

getCommand

init

initWithQueue

returnCommand

### Type Methods

withQueue

## Relationships

### Inherits From

- OSObject

## See Also

### Data Types

IOCallOnceBlock

IOCallOnceFlag

IOCommand

IOCommandPoolPtr

IOCommandPtr

IODMACommand

An object that converts memory references to I/O bus addresses.

IODMACommandSpecification

IODispatchAction

IOHistogramReporter_IVars

IOReportLegendEntry

IOReporter_IVars

IOSimpleReporter_IVars

IOStateReporter_IVars

IOStateReporter_valueSelector

IVarsInvalidator

