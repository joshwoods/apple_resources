

- Application Services
- AXUIElement.h
-  AXUIElementGetTypeID() 

Function

# AXUIElementGetTypeID()

Returns the unique type identifier for the AXUIElementRef type.

macOS 10.2+

``` source
func AXUIElementGetTypeID() -> CFTypeID
```

## Return Value

Returns a CFTypeID representing the AXUIElementRef type.

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

func AXUIElementIsAttributeSettable(AXUIElement, CFString, UnsafeMutablePointer&lt;DarwinBoolean>) -> AXError

Returns whether the specified accessibility object's attribute can be modified.

func AXUIElementPerformAction(AXUIElement, CFString) -> AXError

Requests that the specified accessibility object perform the specified action.

func AXUIElementSetAttributeValue(AXUIElement, CFString, CFTypeRef) -> AXError

Sets the accessibility object's attribute to the specified value.

func AXUIElementSetMessagingTimeout(AXUIElement, Float) -> AXError

Sets the timeout value used in the accessibility API.

