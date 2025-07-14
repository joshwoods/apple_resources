

- DriverKit
-  IOUserClientMethodArguments 

Structure

# IOUserClientMethodArguments

Arguments to pass to IOConnectMethod calls.

DriverKitiOSiPadOSmacOS

``` source
struct IOUserClientMethodArguments;
```

## Discussion

Any argument may be passed as NULL if not passed by the caller.

## Topics

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

### Getting Type Information

IOUserClientScalarArray

Scalar Array Sizes

Output Maximum Size

Constant to denote a variable length structure argument to IOUserClient.

Version Information

## See Also

### Responding to Messages

ExternalMethod

Receive arguments from IOKit.framework IOConnectMethod calls.

IOUserClientMethodDispatch

A structure that specifies how to validate the arguments passed to a client method function.

IOUserClientMethodFunction

