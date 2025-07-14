

- DriverKit
-  OSReportWithBacktrace 

Function

# OSReportWithBacktrace

Generates a backtrace and message for debugging.

DriverKitiOSiPadOSmacOS

``` source
void OSReportWithBacktrace(const char * str, ...);
```

## Parameters 

`str`  

Printf-Like arguments to be logged, along with the backtrace of the caller.

## Discussion

Generates a backtrace and message for debugging. May be inoperative on release OS builds.

## See Also

### Additional Utilities

OSSynchronizeIO

Performs an `mfence` instruction on Intel-based Mac computers.

