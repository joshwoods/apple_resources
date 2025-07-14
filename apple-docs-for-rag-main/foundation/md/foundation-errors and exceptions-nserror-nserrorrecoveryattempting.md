

- Foundation
- Errors and Exceptions
- NSError
-  NSErrorRecoveryAttempting 

# NSErrorRecoveryAttempting

A set of methods that provide options to recover from an error.

## Overview

The `NSErrorRecoveryAttempting` informal protocol provides methods that allow your application to attempt to recover from an error. These methods are invoked when an `NSError` object is returned that specifies the implementing object as the error `recoveryAttempter` and the user has selected one of the error’s localized recovery options. The method invoked depends on how the error is presented to the user. If the error is presented in a document-modal sheet, attemptRecovery(fromError:optionIndex:delegate:didRecoverSelector:contextInfo:) is invoked. If the error is presented in an application-modal dialog, attemptRecovery(fromError:optionIndex:) is invoked.

## Topics

### Attempting Recovery From Errors

func attemptRecovery(fromError error: any Error, optionIndex recoveryOptionIndex: Int, delegate: Any?, didRecoverSelector: Selector?, contextInfo: UnsafeMutableRawPointer?)

Implemented to attempt a recovery from an error noted in a document-modal sheet.

func attemptRecovery(fromError error: any Error, optionIndex recoveryOptionIndex: Int) -> Bool

Implemented to attempt a recovery from an error noted in an application-modal dialog.

## See Also

### Getting the Error Recovery Attempter

var recoveryAttempter: Any?

The object in the user info dictionary corresponding to the NSRecoveryAttempterErrorKey key.

