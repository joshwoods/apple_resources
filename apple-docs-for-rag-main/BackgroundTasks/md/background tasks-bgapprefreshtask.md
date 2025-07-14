

- Background Tasks
-  BGAppRefreshTask 

Class

# BGAppRefreshTask

An object representing a short task typically used to refresh content that’s run while the app is in the background.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
class BGAppRefreshTask
```

## Mentioned in 

Choosing Background Strategies for Your App

## Overview

Use app refresh tasks for updating your app with small bits of information, such as the latest stock values.

Executing app refresh tasks requires setting the `fetch` UIBackgroundModes capability. For information on setting this capability, see BGTaskScheduler.

## Relationships

### Inherits From

- BGTask

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Task management

class BGProcessingTask

A time-consuming processing task that runs while the app is in the background.

class BGTask

An abstract class representing a task that’s run while the app is in the background.

class BGHealthResearchTask

A time-consuming, necessary processing task that runs while the app is in the background to prepare data essential to a health research study.

