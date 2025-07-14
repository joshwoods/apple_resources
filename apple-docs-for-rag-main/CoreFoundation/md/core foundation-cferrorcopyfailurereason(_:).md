

- Core Foundation
-  CFErrorCopyFailureReason(\_:) 

Function

# CFErrorCopyFailureReason(\_:)

Returns a human-presentable failure reason for a given error.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFErrorCopyFailureReason(_ err: CFError!) -> CFString!
```

## Parameters 

`err`  

The CFError to examine. If this is not a valid CFError, the behavior is undefined.

## Return Value

A localized, human-presentable failure reason for `err`, or `NULL` if no user-presentable string is available. Ownership follows the The Create Rule.

## Discussion

The failure reason is a complete sentence which describes why the operation failed. In many cases this will be just the “because” part of the description (but as a complete sentence, which makes localization easier). For example, an error description “Could not save file ‘Letter’ in folder ‘Documents’ because the volume ‘MyDisk’ doesn’t have enough space.” might have a corresponding failure reason, “The volume ‘MyDisk’ doesn’t have enough space.”

By default, this function looks for a value for the kCFErrorLocalizedFailureReasonKey key in the user info dictionary. Toll-free bridged instances of `NSError` might provide additional behaviors for manufacturing this value.

When you create a CFError, you should try to make sure the return value is human-presentable and localized by providing a value for kCFErrorLocalizedFailureReasonKey in the user info dictionary.

## See Also

### Getting Information About an Error

func CFErrorGetDomain(CFError!) -> CFErrorDomain!

Returns the error domain for a given CFError.

func CFErrorGetCode(CFError!) -> CFIndex

Returns the error code for a given CFError.

func CFErrorCopyUserInfo(CFError!) -> CFDictionary!

Returns the user info dictionary for a given CFError.

func CFErrorCopyDescription(CFError!) -> CFString!

Returns a human-presentable description for a given error.

func CFErrorCopyRecoverySuggestion(CFError!) -> CFString!

Returns a human presentable recovery suggestion for a given error.

