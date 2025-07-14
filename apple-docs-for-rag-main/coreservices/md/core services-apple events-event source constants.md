

- Core Services
- Apple Events
-  Event Source Constants 

# Event Source Constants

Identify how an Apple event was delivered.

## Overview

For an example of how you might use these constants with the AEGetAttributePtr(_:_:_:_:_:_:_:) function, see the data type AEEventSource.

## Topics

### Constants

var kAEUnknownSource: Int

The source of the Apple event is unknown.

var kAEDirectCall: Int

The source of the Apple event is a direct call that bypassed the PPC Toolbox.

var kAESameProcess: Int

The source of the Apple event is the same application that received the event (the target application and the source application are the same).

var kAELocalProcess: Int

The source application is another process on the same computer as the target application.

var kAERemoteProcess: Int

The source application is a process on a remote computer on the network.

