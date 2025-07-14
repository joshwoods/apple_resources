

- DriverKit
-  mach_timebase_info 

Structure

# mach_timebase_info

DriverKitiOSiPadOSmacOS

``` source
struct mach_timebase_info;
```

## Overview

In general prefer to use the \ API clock_gettime_nsec_np(3), which deals in the same clocks (and more) in ns units. Conversion of ns to (resp. from) tick units as returned by the mach time APIs is performed by division (resp. multiplication) with the fraction returned by mach_timebase_info().

## Topics

### Instance Properties

denom

numer

## See Also

### Structures

IODMACommandSpecification

IOHistogramReportValues

IOHistogramSegmentConfig

IONormDistReportValues

IORPCMessageErrorReturnContent

IOReportChannel

IOReportChannelList

IOReportChannelType

IOReportElement

IOReportElementValues

IOReportInterest

IOReportInterestList

IOSimpleArrayReportValues

IOSimpleReportValues

IOStateReportValues

