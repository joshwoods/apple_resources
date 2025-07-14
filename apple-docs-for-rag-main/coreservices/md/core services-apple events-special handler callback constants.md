

- Core Services
- Apple Events
-  Special Handler Callback Constants 

# Special Handler Callback Constants

Specify an object callback function to install, get, or remove from the special handler dispatch table.

## Overview

You use these constants with the AEInstallSpecialHandler(_:_:_:), AEGetSpecialHandler(_:_:_:), or AERemoveSpecialHandler(_:_:_:) functions.

## Topics

### Constants

var keyAERangeStart: AEKeyword

Specifies the first Apple event object in a desired range.

var keyAERangeStop: AEKeyword

Specifies the last Apple event object in the desired range.

var keyDisposeTokenProc: AEKeyword

Token disposal function. See OSLDisposeTokenProcPtr.

var keyAECompareProc: AEKeyword

Object-comparison function. See OSLCompareProcPtr.

var keyAECountProc: AEKeyword

Object-counting function. See OSLCountProcPtr.

var keyAEMarkTokenProc: AEKeyword

Mark token function. See OSLGetMarkTokenProcPtr.

var keyAEMarkProc: AEKeyword

Object-marking function. See OSLMarkProcPtr.

var keyAEAdjustMarksProc: AEKeyword

Mark-adjusting function. See OSLAdjustMarksProcPtr.

var keyAEGetErrDescProc: AEKeyword

Get error descriptor callback function. See OSLGetErrDescProcPtr.

