

- Kernel
- Hardware Families
- HID
-  IOHIDCompletionAction 

Type Alias

# IOHIDCompletionAction

Function called when set/get report completes

macOS 10.15+

``` source
typedef void (*IOHIDCompletionAction)(void *target, void *parameter, IOReturn status, uint32_t bufferSizeRemaining);
```

## Parameters 

`target`  

The target specified in the IOHIDCompletion struct.

`parameter`  

The parameter specified in the IOHIDCompletion struct.

`status`  

Completion status

## See Also

### Reports

IOHIDReportType

Describes different type of HID reports.

HIDReportCommandType

IOHIDCompletion

Struct specifying action to perform when set/get report completes.

