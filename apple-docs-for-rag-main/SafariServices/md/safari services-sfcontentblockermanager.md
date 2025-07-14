

- Safari Services
-  SFContentBlockerManager 

Class

# SFContentBlockerManager

A class that your app uses to interact with a content blocker extension.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.4+macOS 10.12+visionOS 1.0+

``` source
class SFContentBlockerManager
```

## Overview

Use this class to determine the state of your content blocker and reload the content-blocking rules used by Safari.

## Topics

### Acting Based on the State of Your Content Blocker

class func getStateOfContentBlocker(withIdentifier: String, completionHandler: (SFContentBlockerState?, (any Error)?) -> Void)

Determines the state of your content blocker.

### Reloading Your Content-Blocking Rules

class func reloadContentBlocker(withIdentifier: String, completionHandler: (((any Error)?) -> Void)?)

Tells Safari to reload the specified extension’s content-blocking rules.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Content blockers

Creating a content blocker

Create a content blocker for Safari in Xcode.

class SFContentBlockerState

The state of a content blocker extension.

