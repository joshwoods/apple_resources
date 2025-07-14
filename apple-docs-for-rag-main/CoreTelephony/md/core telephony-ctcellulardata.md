

- Core Telephony
-  CTCellularData 

Class

# CTCellularData

An object indicating whether the app can access cellular data.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+

``` source
class CTCellularData
```

## Overview

This property represents all access to cellular data. If the restrictedState is CTCellularDataRestrictedState.restricted, the app cannot use the cellular network.

## Topics

### Determining the Cellular Data Restricted State

var restrictedState: CTCellularDataRestrictedState

The current state of cellular data restrictions.

enum CTCellularDataRestrictedState

The possible states of the cellular data policy.

### Handling Policy Changes

var cellularDataRestrictionDidUpdateNotifier: CellularDataRestrictionDidUpdateNotifier?

A block that handles cellular data restriction state changes.

typealias CellularDataRestrictionDidUpdateNotifier

A block to provide updates on the app’s cellular data restriction state.

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

