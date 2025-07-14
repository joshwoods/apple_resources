

- Core Services
- Apple Events
-  Callback Constants for the AEResolve Function 

# Callback Constants for the AEResolve Function

Specify supported callback features to the `AEResolve` function.

## Overview

You use these constants to supply a value for the `callbackFlags` parameter to the AEResolve(_:_:_:) function. This value specifies whether your application supports whose descriptors or provides marking callback functions. To obtain a value for this parameter, you can add together constants to set the appropriate bits, as shown in the following example (for an application that supports both whose tests and marking):

    AEDesc objectSpecifier; // Previously obtained object specifier.     AEDesc  resultToken;
    OSErr myErr;

    myErr = AEResolve (&amp;objectSpecifier,
                        kAEIDoWhose + kAEIDoMarking, &amp;resultToken)

AppleScript generates whose clauses from script statements such as the following:

tell application &quot;Finder&quot;
    every file in control panels folder whose file type is &quot;APPL&quot;
end tell

## Topics

### Constants

var kAEIDoMinimum: Int

The application does not handle whose tests or provide marking callbacks.

var kAEIDoWhose: Int

The application supports whose tests (supports key form `formWhose`).

var kAEIDoMarking: Int

The application provides marking callback functions. Marking callback functions are described in Apple Event Manager.

var kAEHandleSimpleRanges: Int

var kAEPassSubDescs: Int

var kAEResolveNestedLists: Int

var kAEUseRelativeIterators: Int

