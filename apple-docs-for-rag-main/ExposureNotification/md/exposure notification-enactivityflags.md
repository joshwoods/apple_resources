

- Exposure Notification
-  ENActivityFlags 

Structure

# ENActivityFlags

Activities that occur while the app isn’t running.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
struct ENActivityFlags
```

## Overview

Important

This symbol is available in iOS 12.5, and in iOS 13.6 and later.

## Topics

### Initializers

init(rawValue: UInt32)

Initialize the structure.

### Type Properties

static var periodicRun: ENActivityFlags

The property that specifies launching the app in the background for periodic operation in iOS 12.5.

static var preAuthorizedKeyReleaseNotificationTapped: ENActivityFlags

The property that specifies launching the app in the foreground to display preauthorized key-release information.

static var reserved1: ENActivityFlags

This property is reserved.

static var reserved2: ENActivityFlags

This property is reserved.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Activating the Manager

func activate(completionHandler: ENErrorHandler)

Prepares the manager for use.

var activityHandler: ENActivityHandler?

The handler that the framework invokes when the app activates a notification manager.

typealias ENActivityHandler

The handler the system invokes to report activities that occurred while the app wasn’t running.

func setExposureNotificationEnabled(Bool, completionHandler: ENErrorHandler)

Enables or disables exposure notification.

