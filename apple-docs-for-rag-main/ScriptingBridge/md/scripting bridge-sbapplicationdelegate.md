

- Scripting Bridge
-  SBApplicationDelegate 

Protocol

# SBApplicationDelegate

This informal protocol defines a delegation method for handling Apple event errors that are sent from a target application to an SBApplication object.

Mac Catalyst 13.0+macOS 10.5+

``` source
protocol SBApplicationDelegate
```

## Overview

You must set a delegate for the SBApplication object using the delegate method. If you do not set a delegate and have the delegate handle the error in some way, SBApplication raises an exception.

## Topics

### Handling Errors

func eventDidFail(UnsafePointer&lt;AppleEvent>, withError: any Error) -> Any?

Sent by an `SBApplication` object when a target application returns an error Apple event.

**Required**

