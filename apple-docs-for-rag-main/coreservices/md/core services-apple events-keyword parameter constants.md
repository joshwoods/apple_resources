

- Core Services
- Apple Events
-  Keyword Parameter Constants 

# Keyword Parameter Constants

Specify keyword values for Apple event parameters, as well as information for the `AEManagerInfo` function to retrieve. Some common key word values are shown here.

## Overview

These constants are keyword constants for Apple event parameters. An Apple event consists of attributes (which identify the Apple event and denote its task) and, often, parameters (which contain information to be used by the target application). Taken together, the attributes of an Apple event denote the task to be performed on any data specified in the Apple event’s parameters.

Keywords are arbitrary names used by the Apple Event Manager to keep track of various descriptors. Your application cannot examine the contents of an Apple event directly. Instead, you call Apple Event Manager routines such as those described in Getting Data or Descriptors From Apple Events and Apple Event Records to request attributes and parameters by keyword.

See also Keyword Attribute Constants.

## Topics

### Constants

var keyDirectObject: AEKeyword

Direct parameter. Usually specifies the data to be acted upon by the target application.

var keyErrorNumber: AEKeyword

Error number. Often used to extract error information from a reply Apple event.

var keyErrorString: AEKeyword

Error string. Often used to extract error information from a reply Apple event to display to the user.

var keyProcessSerialNumber: AEKeyword

Process serial number. See also AEManagerInfo(_:_:).

var keyPreDispatch: AEKeyword

A predispatch handler (an Apple event handler that the Apple Event Manager calls immediately before it dispatches an Apple event). See also Managing Special Handler Dispatch Tables.

var keySelectProc: AEKeyword

You pass this value in the `functionClass` parameter of the AEManagerInfo(_:_:) function to disable the Object Support Library. Disabling the Object Support Library is not recommended.

var keyAERecorderCount: AEKeyword

Used with the `keyword` parameter of the AEManagerInfo(_:_:) function. If you pass this value, on return, the `result` parameter supplies the number of processes that are currently recording Apple events.

var keyAEVersion: AEKeyword

Used with the `keyword` parameter of the AEManagerInfo(_:_:) function. If you pass this value, on return, the `result` parameter supplies version information for the Apple Event Manager, in NumVersion format.

