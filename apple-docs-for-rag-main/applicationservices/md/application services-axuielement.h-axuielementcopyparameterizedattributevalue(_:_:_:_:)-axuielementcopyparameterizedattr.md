

- Application Services
- AXUIElement.h
-  AXUIElementCopyParameterizedAttributeValue(\_:\_:\_:\_:) 

Function

# AXUIElementCopyParameterizedAttributeValue(\_:\_:\_:\_:)

Returns the value of an accessibility object's parameterized attribute.

macOS 10.3+

``` source
func AXUIElementCopyParameterizedAttributeValue(
    _ element: AXUIElement,
    _ parameterizedAttribute: CFString,
    _ parameter: CFTypeRef,
    _ result: UnsafeMutablePointer
) -> AXError
```

## Parameters 

`element`  

The AXUIElementRef representing the accessibility object.

`parameterizedAttribute`  

The parameterized attribute.

`parameter`  

The parameter.

`result`  

On return, the value of the parameterized attribute.

## Return Value

If unsuccessful, `AXUIElementCopyParameterizedAttributeValue` may return one of the following error codes, among others:

`kAXErrorAttributeUnsupported` or `kAXErrorParameterizedAttributeUnsupported`  
The specified AXUIElementRef does not support the specified parameterized attribute.

`kAXErrorNoValue`  
The specified parameterized attribute does not have a value.

`kAXErrorIllegalArgument`  
One or more of the arguments is an illegal value.

`kAXErrorInvalidUIElement`  
The AXUIElementRef is invalid.

`kAXErrorCannotComplete`  
The function cannot complete because messaging has failed in some way.

`kAXErrorNotImplemented`  
The process does not fully support the accessibility API.

## See Also

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

