

- Application Services
- Core Printing
-  User Cancellation Constant 

# User Cancellation Constant

A constant that specifies an error value that indicates the user canceled a printing operation.

## Overview

This constant is provided for compatibility with old applications and printer drivers that expect the `iPrAbort` error code to be returned when the user cancels a printing operation.

The default idle function checks for Command-period keyboard events during printing, and sets the error condition equal to `kPMCancel` if one occurs. Your application can check for this condition using the `PMSessionError` function, and should cancel the print job if `kPMCancel` is returned.

If you supply your own idle function (not needed in Mac OS 8, 9, or X), your function must check for Command-period keyboard events, and set the error condition using the function `PMSessionSetError`.

## Topics

### Constants

var kPMCancel: Int

Specifies that the user clicked the Cancel button in a Print or Page Setup dialog.

