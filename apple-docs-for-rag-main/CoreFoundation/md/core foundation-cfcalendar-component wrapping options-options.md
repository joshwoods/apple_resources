

- Core Foundation
- CFCalendar
-  Component Wrapping Options 

API Collection

# Component Wrapping Options

The wrapping option specifies overflow behavior for calendar components in calendrical calculations

## Overview

The wrapping option specifies overflow behavior for calendar components in calendrical calculations—see CFCalendarAddComponents and CFCalendarGetComponentDifference.

## Topics

### Constants

var kCFCalendarComponentsWrap: CFOptionFlags

Specifies that the components specified for calendar components should be incremented and wrap around to zero/one on overflow, but should not cause higher units to be incremented.

## See Also

### Constants

struct CFCalendarUnit

CFCalendarUnit constants are used to specify calendrical units, such as day or month, in various calendar calculations.

