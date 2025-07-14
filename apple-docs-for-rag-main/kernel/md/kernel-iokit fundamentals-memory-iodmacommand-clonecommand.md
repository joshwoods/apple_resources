

- Kernel
- IOKit Fundamentals
- Memory
- IODMACommand
-  cloneCommand 

# cloneCommand

Creates a new command based on the specification of the current one.

``` source
virtual IODMACommand *cloneCommand(
 void *refCon = 0); 
```

## Return Value

Returns a new memory cursor if successfully created and initialised, 0 otherwise.

## Overview

Factory function to create and initialise an IODMACommand in one operation. The current command's specification will be duplicated in the new object, but however none of its state will be duplicated. This means that it is safe to clone a command even if it is currently active and running, however you must be certain that the command to be duplicated does have a valid reference for the duration.

## See Also

### Creating a DMA Command

withSpecification

Creates and initializes a DMA command in one operation.

+ withSpecification

Creates and initializes an DMA command in one operation.

+ withSpecification

Creates and initializes an DMA command in one operation.

initWithSpecification

Primary initializer for the DMA command object.

- initWithSpecification

Primary initializer for the DMA command object.

- initWithSpecification

Primary initializer for the DMA command object.

weakWithSpecification

Creates and initializes an DMA command object in one operation if this version of the operating system supports it.

+ withRefCon

- initWithRefCon

- cloneCommand

Creates a new command based on the specification of the current one.

- init

- free

MappingOptions

Mapping types to indicate the desired mapper type for translating memory descriptors into I/O DMA Bus addresses.

SynchronizeOptions

Options for the synchronize method.

