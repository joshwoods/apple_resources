

- DriverKit
- IOUserClientMethodDispatch
-  checkStructureInputSize 

Instance Property

# checkStructureInputSize

The expected size of the scalar inputs.

DriverKitiOSiPadOSmacOS

``` source
uint32_t checkStructureInputSize;
```

## Discussion

If the value of this field is kIOUserClientVariableStructureSize, don’t validate the structure size. For all other values, the value in this property must equal the value in either the structureInput or structureInputDescriptor fields of the IOUserClientMethodArguments structure.

## See Also

### Getting the Dispatch Properties

function

The function to call after validating all of the specified values.

checkCompletionExists

An integer value indicating whether to check for the existence of a completion action.

checkScalarInputCount

The expected number of scalar inputs.

checkScalarOutputCount

The expected number of scalar outputs.

checkStructureOutputSize

The expected size of the scalar outputs.

