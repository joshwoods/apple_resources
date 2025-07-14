

- DriverKit
- IOUserClientMethodDispatch
-  checkStructureOutputSize 

Instance Property

# checkStructureOutputSize

The expected size of the scalar outputs.

DriverKitiOSiPadOSmacOS

``` source
uint32_t checkStructureOutputSize;
```

## Discussion

If the value of this field is kIOUserClientVariableStructureSize, don’t validate the structure size. For all other values, the value in this property must equal the value in the structureOutputMaximumSize field of the IOUserClientMethodArguments structure.

## See Also

### Getting the Dispatch Properties

function

The function to call after validating all of the specified values.

checkCompletionExists

An integer value indicating whether to check for the existence of a completion action.

checkScalarInputCount

The expected number of scalar inputs.

checkStructureInputSize

The expected size of the scalar inputs.

checkScalarOutputCount

The expected number of scalar outputs.

