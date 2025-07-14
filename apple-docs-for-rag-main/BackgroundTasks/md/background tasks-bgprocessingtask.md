

- Background Tasks
-  BGProcessingTask 

Class

# BGProcessingTask

A time-consuming processing task that runs while the app is in the background.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
class BGProcessingTask
```

## Mentioned in 

Choosing Background Strategies for Your App

## Overview

Use processing tasks for long data updates, processing data, and app maintenance. Although processing tasks can run for minutes, the system can interrupt the process. Add an expiration handler by setting expirationHandler for any required cleanup.

Executing processing tasks requires setting the `processing` UIBackgroundModes capability. For information on setting this capability, see BGTaskScheduler.

Processing tasks run only when the device is idle. The system terminates any background processing tasks running when the user starts using the device. Background refresh tasks aren’t affected.

## Relationships

### Inherits From

- BGTask

### Inherited By

- BGHealthResearchTask

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Task management

class BGAppRefreshTask

An object representing a short task typically used to refresh content that’s run while the app is in the background.

class BGTask

An abstract class representing a task that’s run while the app is in the background.

class BGHealthResearchTask

A time-consuming, necessary processing task that runs while the app is in the background to prepare data essential to a health research study.

