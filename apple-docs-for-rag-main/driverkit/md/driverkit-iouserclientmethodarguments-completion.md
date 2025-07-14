

- DriverKit
- IOUserClientMethodArguments
-  completion 

Instance Property

# completion

An action for processing asynchronous data received from the service.

DriverKitiOSiPadOSmacOS

``` source
OSAction * completion;
```

## Discussion

The system retains this method only during the invocation of ExternalMethod. Retain this method yourself if you intend to use it outside of that invocation.

## See Also

### Getting the Method Arguments

version

selector

The index of the method you want to execute.

scalarInput

An array of scalars from the caller.

scalarInputCount

The number of scalars provided by the caller.

structureInput

A data object containing the structure input from the IOKit connect method.

structureInputDescriptor

A memory descriptor containing structure input from the IOKit connect method.

scalarOutput

An array of scalars to return to the caller.

scalarOutputCount

The number of scalars to return to the caller.

structureOutput

A data object to return to the caller as structure output.

structureOutputDescriptor

An IOMemoryDescriptor specified by the caller for structure output.

structureOutputMaximumSize

The maximum size of the output structure that you specified.

