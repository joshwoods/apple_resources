

- Application Services
-  AXUIElement.h 

API Collection

# AXUIElement.h

## Overview

See the Overview section above for header-level documentation.

### Overview

Assistive applications use the functions defined in this header file to communicate with and control accessible applications running in macOS.

Each accessible user interface element in an application is represented by an AXUIElementRef, which is a CFTypeRef. AXUIElementRefs (like all CFTypeRefs) can be used with all the Core Foundation polymorphic functions, such as CFRetain, CFRelease, and CFEqual(_:_:).

All functions defined in this header file return `kAXErrorSuccess` on success. If there is some sort of system memory failure, such as the failure to allocate an object, all functions can return `kAXErrorFailure`. In the unlikely event that some process does not fully support the accessibility API, a function can return `kAXErrorNotImplemented`.

In addition, some functions can return the following error codes:

`kAXErrorInvalidUIElement`  
The passed-in AXUIElementRef is invalid. All functions that include an AXUIElementRef parameter can return this error code.

`kAXErrorIllegalArgument`  
At least one of the arguments is illegal (for example, NIL passed in for a pointer).

`kAXErrorCannotComplete`  
There is a problem with messaging (such as when messaging to the server fails or when the accessible application is unresponsive or waiting for user input). All functions that perform messaging can return this error code.

`kAXErrorAPIDisabled`  
The accessibility API is disabled. All functions that perform messaging can return this error code.

For more information on the definition and use of accessibility objects and in macOS accessibility support in general, see Accessibility Programming Guide for OS X.

#### Included Headers

- \

- \

- \

## Topics

### Notification API

func AXObserverAddNotification(AXObserver, AXUIElement, CFString, UnsafeMutableRawPointer?) -> AXError

Registers the specified observer to receive notifications from the specified accessibility object.

func AXObserverCreate(pid_t, AXObserverCallback, UnsafeMutablePointer&lt;AXObserver?>) -> AXError

Creates a new observer that can receive notifications from the specified application.

func AXObserverCreateWithInfoCallback(pid_t, AXObserverCallbackWithInfo, UnsafeMutablePointer&lt;AXObserver?>) -> AXError

Creates a new observer that can receive notifications with an information dictionary from the specified application.

func AXObserverGetRunLoopSource(AXObserver) -> CFRunLoopSource

Returns the observer's run loop source.

func AXObserverGetTypeID() -> CFTypeID

Returns the unique type identifier for the AXObserverRef type.

func AXObserverRemoveNotification(AXObserver, AXUIElement, CFString) -> AXError

Removes the specified notification from the list of notifications the observer wants to receive from the accessibility object.

### Miscellaneous

func AXIsProcessTrusted() -> Bool

Returns whether the current process is a trusted accessibility client.

func AXIsProcessTrustedWithOptions(CFDictionary?) -> Bool

Returns whether the current process is a trusted accessibility client.

func AXUIElementCopyActionDescription(AXUIElement, CFString, UnsafeMutablePointer&lt;CFString?>) -> AXError

Returns a localized description of the specified accessibility object's action.

func AXUIElementCopyActionNames(AXUIElement, UnsafeMutablePointer&lt;CFArray?>) -> AXError

Returns a list of all the actions the specified accessibility object can perform.

func AXUIElementCopyAttributeNames(AXUIElement, UnsafeMutablePointer&lt;CFArray?>) -> AXError

Returns a list of all the attributes supported by the specified accessibility object.

func AXUIElementCopyAttributeValue(AXUIElement, CFString, UnsafeMutablePointer&lt;CFTypeRef?>) -> AXError

Returns the value of an accessibility object's attribute.

func AXUIElementCopyAttributeValues(AXUIElement, CFString, CFIndex, CFIndex, UnsafeMutablePointer&lt;CFArray?>) -> AXError

Returns an array of attribute values for the accessibility object's attribute, starting at the specified index.

func AXUIElementCopyElementAtPosition(AXUIElement, Float, Float, UnsafeMutablePointer&lt;AXUIElement?>) -> AXError

Returns the accessibility object at the specified position in top-left relative screen coordinates.

func AXUIElementCopyMultipleAttributeValues(AXUIElement, CFArray, AXCopyMultipleAttributeOptions, UnsafeMutablePointer&lt;CFArray?>) -> AXError

Returns the values of multiple attributes in the accessibility object.

func AXUIElementCopyParameterizedAttributeNames(AXUIElement, UnsafeMutablePointer&lt;CFArray?>) -> AXError

Returns a list of all the parameterized attributes supported by the specified accessibility object.

func AXUIElementCopyParameterizedAttributeValue(AXUIElement, CFString, CFTypeRef, UnsafeMutablePointer&lt;CFTypeRef?>) -> AXError

Returns the value of an accessibility object's parameterized attribute.

func AXUIElementCreateApplication(pid_t) -> AXUIElement

Creates and returns the top-level accessibility object for the application with the specified process ID.

func AXUIElementCreateSystemWide() -> AXUIElement

Returns an accessibility object that provides access to system attributes.

func AXUIElementGetAttributeValueCount(AXUIElement, CFString, UnsafeMutablePointer&lt;CFIndex>) -> AXError

Returns the count of the array of an accessibility object's attribute value.

func AXUIElementGetPid(AXUIElement, UnsafeMutablePointer&lt;pid_t>) -> AXError

Returns the process ID associated with the specified accessibility object.

func AXUIElementGetTypeID() -> CFTypeID

Returns the unique type identifier for the AXUIElementRef type.

func AXUIElementIsAttributeSettable(AXUIElement, CFString, UnsafeMutablePointer&lt;DarwinBoolean>) -> AXError

Returns whether the specified accessibility object's attribute can be modified.

func AXUIElementPerformAction(AXUIElement, CFString) -> AXError

Requests that the specified accessibility object perform the specified action.

func AXUIElementSetAttributeValue(AXUIElement, CFString, CFTypeRef) -> AXError

Sets the accessibility object's attribute to the specified value.

func AXUIElementSetMessagingTimeout(AXUIElement, Float) -> AXError

Sets the timeout value used in the accessibility API.

### Callbacks

See the Overview section above for header-level documentation.

typealias AXObserverCallback

typealias AXObserverCallbackWithInfo

### Data Types

See the Overview section above for header-level documentation.

struct AXCopyMultipleAttributeOptions

class AXObserver

class AXUIElement

A structure used to refer to an accessibility object.

