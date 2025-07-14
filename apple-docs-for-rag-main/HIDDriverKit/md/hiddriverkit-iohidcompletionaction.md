

- HIDDriverKit
-  IOHIDCompletionAction 

Type Alias

# IOHIDCompletionAction

A function to call when a report operation completes.

DriverKitmacOS

``` source
typedef void (*)(void *, void *, int, unsigned int) IOHIDCompletionAction;
```

## Parameters 

`target`  

The target specified in the `IOHIDCompletion` struct.

`parameter`  

The parameter specified in the `IOHIDCompletion` struct.

`status`  

The completion status.

## See Also

### Internal Structures

IOHIDCompletion

A structure specifying the action to perform when a set/get report completes.

HIDReportCommandType

The type of the report command for a DriverKit driver.

HIDActionType

