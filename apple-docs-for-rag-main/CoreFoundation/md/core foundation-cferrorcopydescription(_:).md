

- Core Foundation
-  CFErrorCopyDescription(\_:) 

Function

# CFErrorCopyDescription(\_:)

Returns a human-presentable description for a given error.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFErrorCopyDescription(_ err: CFError!) -> CFString!
```

## Parameters 

`err`  

The CFError to examine. If this is not a valid CFError, the behavior is undefined.

## Return Value

A localized, human-presentable description of `err`. This function never returns `NULL`. Ownership follows the The Create Rule.

## Discussion

This is a complete sentence or two which says what failed and why it failed. The structure of the description depends on the details provided in the user info dictionary. The rules for computing the return value are as follows:

1.  If the value in the user info dictionary for kCFErrorLocalizedDescriptionKey is not `NULL`, it returns that value as-is.

2.  If the value in the user info dictionary for kCFErrorLocalizedFailureReasonKey is not `NULL`, there will be an error generated from that.

The description is something like: “Operation could not be completed. “ + `kCFErrorLocalizedFailureReasonKey` 3. Generate a user-presentable string from kCFErrorDescriptionKey, the domain, and code.

The description is something like: “Operation could not be completed. Error domain/code occurred. “ or “Operation could not be completed. “ + `kCFErrorDescriptionKey` + “ (Error domain/code)”

Toll-free bridged instances of NSError might provide additional behaviors for manufacturing a description string.

You should not depend on the exact contents or format of the returned string, as it might change in different releases of the operating system.

When you create a CFError, you should try to make sure the return value is human-presentable and localized by providing a value for kCFErrorLocalizedDescriptionKey in the user info dictionary.

## See Also

### Getting Information About an Error

func CFErrorGetDomain(CFError!) -> CFErrorDomain!

Returns the error domain for a given CFError.

func CFErrorGetCode(CFError!) -> CFIndex

Returns the error code for a given CFError.

func CFErrorCopyUserInfo(CFError!) -> CFDictionary!

Returns the user info dictionary for a given CFError.

func CFErrorCopyFailureReason(CFError!) -> CFString!

Returns a human-presentable failure reason for a given error.

func CFErrorCopyRecoverySuggestion(CFError!) -> CFString!

Returns a human presentable recovery suggestion for a given error.

