

- DriverKit
- IOUserClientMethodDispatch
-  function 

Instance Property

# function

The function to call after validating all of the specified values.

DriverKitiOSiPadOSmacOS

``` source
IOUserClientMethodFunction function;
```

## Discussion

If this property is `NULL` and all checks pass, the system returns `kIOReturnNoCompletion` for the caller to implement the method.

## See Also

### Getting the Dispatch Properties

checkCompletionExists

An integer value indicating whether to check for the existence of a completion action.

checkScalarInputCount

The expected number of scalar inputs.

checkStructureInputSize

The expected size of the scalar inputs.

checkScalarOutputCount

The expected number of scalar outputs.

checkStructureOutputSize

The expected size of the scalar outputs.

