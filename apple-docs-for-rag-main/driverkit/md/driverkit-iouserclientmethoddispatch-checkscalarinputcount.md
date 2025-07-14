

- DriverKit
- IOUserClientMethodDispatch
-  checkScalarInputCount 

Instance Property

# checkScalarInputCount

The expected number of scalar inputs.

DriverKitiOSiPadOSmacOS

``` source
uint32_t checkScalarInputCount;
```

## Discussion

If the value of this field is kIOUserClientVariableStructureSize, ignore the value of the scalarInputCount field. For all other values, the value in this property must equal the value in the scalarInputCount field of the IOUserClientMethodArguments structure.

## See Also

### Getting the Dispatch Properties

function

The function to call after validating all of the specified values.

checkCompletionExists

An integer value indicating whether to check for the existence of a completion action.

checkStructureInputSize

The expected size of the scalar inputs.

checkScalarOutputCount

The expected number of scalar outputs.

checkStructureOutputSize

The expected size of the scalar outputs.

