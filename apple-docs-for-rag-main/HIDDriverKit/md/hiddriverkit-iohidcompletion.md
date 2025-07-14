

- HIDDriverKit
-  IOHIDCompletion 

Structure

# IOHIDCompletion

A structure specifying the action to perform when a set/get report completes.

DriverKitmacOS

``` source
typedef struct IOHIDCompletion { ... } IOHIDCompletion;
```

## Topics

### Getting the Completion Handler Properties

target

The target to pass to the action function.

action

The function to call.

parameter

The parameter to pass to the action function.

## See Also

### Internal Structures

IOHIDCompletionAction

A function to call when a report operation completes.

HIDReportCommandType

The type of the report command for a DriverKit driver.

HIDActionType

