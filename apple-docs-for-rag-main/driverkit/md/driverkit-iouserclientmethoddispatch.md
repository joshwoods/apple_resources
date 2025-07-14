

- DriverKit
-  IOUserClientMethodDispatch 

Structure

# IOUserClientMethodDispatch

A structure that specifies how to validate the arguments passed to a client method function.

DriverKitiOSiPadOSmacOS

``` source
struct IOUserClientMethodDispatch;
```

## Discussion

Used this structure to specify the validation checks to perform on the fields of the IOUserClientMethodArguments structure passed to an IOUserClientMethodFunction.

## Topics

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

checkStructureOutputSize

The expected size of the scalar outputs.

## See Also

### Responding to Messages

ExternalMethod

Receive arguments from IOKit.framework IOConnectMethod calls.

IOUserClientMethodArguments

Arguments to pass to IOConnectMethod calls.

IOUserClientMethodFunction

