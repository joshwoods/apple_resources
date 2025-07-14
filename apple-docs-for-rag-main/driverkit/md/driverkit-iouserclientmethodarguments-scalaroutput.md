

- DriverKit
- IOUserClientMethodArguments
-  scalarOutput 

Instance Property

# scalarOutput

An array of scalars to return to the caller.

DriverKitiOSiPadOSmacOS

``` source
uint64_t * scalarOutput;
```

## See Also

### Getting the Method Arguments

version

selector

The index of the method you want to execute.

completion

An action for processing asynchronous data received from the service.

scalarInput

An array of scalars from the caller.

scalarInputCount

The number of scalars provided by the caller.

structureInput

A data object containing the structure input from the IOKit connect method.

structureInputDescriptor

A memory descriptor containing structure input from the IOKit connect method.

scalarOutputCount

The number of scalars to return to the caller.

structureOutput

A data object to return to the caller as structure output.

structureOutputDescriptor

An IOMemoryDescriptor specified by the caller for structure output.

structureOutputMaximumSize

The maximum size of the output structure that you specified.

