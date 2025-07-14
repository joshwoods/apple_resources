

- DriverKit
- IOUserClientMethodDispatch
-  checkCompletionExists 

Instance Property

# checkCompletionExists

An integer value indicating whether to check for the existence of a completion action.

DriverKitiOSiPadOSmacOS

``` source
uint32_t checkCompletionExists;
```

## Discussion

If the value of this field is a positive unsigned integer, the completion field must be set to a valid action. If the value is `0`, the completion field must be `NULL`. If the value of this field is -1U, the completion field is ignored.

## See Also

### Getting the Dispatch Properties

function

The function to call after validating all of the specified values.

checkScalarInputCount

The expected number of scalar inputs.

checkStructureInputSize

The expected size of the scalar inputs.

checkScalarOutputCount

The expected number of scalar outputs.

checkStructureOutputSize

The expected size of the scalar outputs.

