

- Kernel
- IOKit Fundamentals
- Data Types
-  OSAction 

Class

# OSAction

macOS 10.15+

``` source
class OSAction : OSObject, OSActionInterface
```

## Topics

### Instance Methods

- Aborted

- Aborted_Impl

- Cancel

Cancels the execution of the action's callbacks.

- Dispatch

- EndWait

- GetReference

Returns a pointer to any additional memory allocated by the action object on your behalf.

- SetAbortedHandler

Install a handler for the system to call when no other processes reference the action object.

- Wait

- WillWait

- free

Performs any final cleanup for the action object.

- getMetaClass

### Type Methods

+ Aborted_Invoke

+ Create

Creates a new action object and configures it with your custom target object and callback method.

+ CreateWithTypeName

+ CreateWithTypeName_Call

+ CreateWithTypeName_Impl

+ CreateWithTypeName_Invoke

+ Create_Call

+ Create_Impl

+ Create_Invoke

## Relationships

### Inherits From

- OSActionInterface
- OSObject

## See Also

### Actions

OSActionInterface

