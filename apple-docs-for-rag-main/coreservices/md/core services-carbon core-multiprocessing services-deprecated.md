

- Core Services
- Carbon Core
-  Multiprocessing Services Deprecated

API Collection

# Multiprocessing Services

Support multitasking in your app.

Deprecated

In macOS 10.8 and later, use Grand Central Dispatch (GCD) or POSIX threads instead. For more information, see Concurrency Programming Guide, the Dispatch framework reference, and Threading Programming Guide.

## Overview

Multiprocessing Services is an API that lets you create preemptive tasks in your application that can run on one or more microprocessors. Unlike the cooperative threads created by the Thread Manager, Multiprocessing Services automatically divides processor time among the available tasks, so that no particular task can monopolize the system. This document is relevant to you if you want to add multitasking capability to your Mac OS applications.

In macOS, Carbon supports Multiprocessing Services with the following restrictions:

- Debugging functions are not implemented. Use the mach APIs provided by the system to implement debugging services.

- Opaque notification IDs are local to your process; they are not globally addressable across processes.

- Global memory allocation is not supported.

### Gestalt Constants

You can determine which system software calls are preemptively-safe for Multiprocessing Services by using the preemptive function attribute selectors defined in the Gestalt Manager. For more information, see Gestalt Manager.

## Topics

### Result Codes

Result codes defined for Multiprocessing Services are listed below.

var kMPIterationEndErr: Int

var kMPPrivilegedErr: Int

var kMPProcessCreatedErr: Int

var kMPProcessTerminatedErr: Int

var kMPTaskCreatedErr: Int

var kMPTaskBlockedErr: Int

The desired task is blocked.

var kMPTaskStoppedErr: Int

The desired task is stopped.

var kMPDeletedErr: Int

The desired notification the function was waiting upon was deleted.

var kMPTimeoutErr: Int

The designated timeout interval passed before the function could take action.

var kMPInsufficientResourcesErr: Int

Could not complete task due to unavailable Multiprocessing Services resources. Note that many functions return this value as a general error when the desired action could not be performed.

var kMPInvalidIDErr: Int

Invalid ID value. For example, an invalid message queue ID was passed to `MPNotifyQueue`.

