

- Screen Time
-  STWebHistory 

Class

# STWebHistory

The object you use to delete web-usage data.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+

``` source
class STWebHistory
```

## Overview

This class provides an easy way for you to delete web history, including:

- All history

- History associated to a specific URL

- History during a specific time interval

## Topics

### Initializers

init(bundleIdentifier: String) throws

Creates a web history instance to delete web-usage data associated to the bundle identifier you specify.

init(bundleIdentifier: String, profileIdentifier: STWebHistory.ProfileIdentifier?) throws

Creates a web history instance to delete web-usage data associated to the bundle identifier and profile identifier you specify.

init(profileIdentifier: STWebHistory.ProfileIdentifier?)

Creates a web history instance to delete web-usage data associated to the profile identifier you specify.

### Instance methods

func deleteAllHistory()

Deletes all web history associated with the bundle identifier you specified during initialization.

func deleteHistory(during: DateInterval)

Deletes web history that occurred during the date interval you specify.

func deleteHistory(for: URL)

Deletes all the web history for the URL you specify.

### Structures

struct ProfileIdentifier

An identifier representing a web history profile.

### Instance Methods

func fetchAllHistory(completionHandler: (Set&lt;URL>?, (any Error)?) -> Void)

Fetches all web history associated with the bundle identifier and profile identifier you specified during initialization.

func fetchHistory(during: DateInterval, completionHandler: (Set&lt;URL>?, (any Error)?) -> Void)

Fetches web history that occurred during the date interval you specify.

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

