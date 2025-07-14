

- DriverKit
- IOUserClientMethodArguments
-  selector 

Instance Property

# selector

The index of the method you want to execute.

DriverKitiOSiPadOSmacOS

``` source
uint64_t selector;
```

## Discussion

When calling one of the IOKit connection methods, such as `IOConnectMethodScalarIScalarO`, the value in this property represents the index of the method you want to execute.

## See Also

### Getting the Method Arguments

version

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

