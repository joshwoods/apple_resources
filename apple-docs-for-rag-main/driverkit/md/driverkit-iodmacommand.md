

- DriverKit
-  IODMACommand 

Class

# IODMACommand

An object that converts memory references to I/O bus addresses.

DriverKitiOSiPadOSmacOS

``` source
class IODMACommand;
```

## Overview

The IODMACommand class supersedes IOMemoryCursor and greatly enhances the functionality and power of it. The command can be specified to output 64 bit physical addresses and also allows driver writers to bypass mapping hardware or get addresses suitable for non-snooped DMA.

The command is designed to be very easily subclassable. Most driver writers need to associate some DMA operations with their memory descriptor, and usually use a C structure for that purpose. This structure is often kept in a linked list. This IODMACommand has built-in `` linkage and can be derived and ‘public:’ variables added, giving the developer a structure that can associate a memory descriptor with a particular DMA command but will also allow the developer to generate that command and keep the state necessary for tracking it.

Create a pool of IODMACommand objects at driver initialization, and keep each command in an IOCommandPool when not in use. You may also maintain your own free list of objects if preferred. See the `` and `` for sample code on manipulating the command’s doubly linked list entries.

You can use an IODMACommand object in a ‘weak-linked’ manner. To do this you must avoid using any static member functions. Use the much slower, but safe, weakWithSpecification function. On success, the function returns a DMA command object, which you can use to clone as many commands as needed.

## Topics

### Creating a DMA Command

init

free

Create

### Performing Internal Operations

CompleteDMA

GetPreparation

PerformOperation

PrepareForDMA

## Relationships

### Inherits From

- OSObject

## See Also

### Data Types

IOCallOnceBlock

IOCallOnceFlag

IOCommand

IOCommandPool

IOCommandPoolPtr

IOCommandPtr

IODMACommandSpecification

IODispatchAction

IOHistogramReporter_IVars

IOReportLegendEntry

IOReporter_IVars

IOSimpleReporter_IVars

IOStateReporter_IVars

IOStateReporter_valueSelector

IVarsInvalidator

