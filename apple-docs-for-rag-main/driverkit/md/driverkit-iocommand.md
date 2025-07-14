

- DriverKit
-  IOCommand 

Class

# IOCommand

DriverKitiOSiPadOSmacOS

``` source
class IOCommand;
```

## Overview

This class is an abstract class which represents an I/O command.

This class is an abstract class which represents an I/O command passed from a device driver to a controller. All controller commands (e.g. IOATACommand) should inherit from this class.

## Topics

### Instance Methods

CommandChain

free

init

### Type Methods

FromChain

## Relationships

### Inherits From

- OSObject

## See Also

### Data Types

IOCallOnceBlock

IOCallOnceFlag

IOCommandPool

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

