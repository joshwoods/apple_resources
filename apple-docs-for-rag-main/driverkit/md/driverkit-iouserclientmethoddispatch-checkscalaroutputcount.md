

- DriverKit
- IOUserClientMethodDispatch
-  checkScalarOutputCount 

Instance Property

# checkScalarOutputCount

The expected number of scalar outputs.

DriverKitiOSiPadOSmacOS

``` source
uint32_t checkScalarOutputCount;
```

## Discussion

If the value of this field is kIOUserClientVariableStructureSize, ignore the value of the scalarOutputCount field. For all other values, the value in this property must equal the value in the scalarOutputCount field of the IOUserClientMethodArguments structure.

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

checkStructureOutputSize

The expected size of the scalar outputs.

