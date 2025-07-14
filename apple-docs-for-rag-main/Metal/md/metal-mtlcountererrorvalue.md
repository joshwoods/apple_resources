

- Metal
-  MTLCounterErrorValue 

Global Variable

# MTLCounterErrorValue

A sentinel value for an entry in a counter sample buffer that indicates the entry’s data is invalid.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var MTLCounterErrorValue: UInt64 { get }
```

## Mentioned in 

Converting a GPU’s Counter Data into a Readable Format

## Discussion

A GPU driver typically sets entries to this value when it encounters an error resolving a counter’s data. The driver also uses this value for counters it doesn’t support within a counter set (see Confirming which Counters and Counter Sets a GPU Supports).

## See Also

### Counter Sample Data Output

Converting a GPU’s Counter Data into a Readable Format

Inspect and use the data within a GPU’s counter sample buffer by resolving it into a standard format.

struct MTLCounterResultTimestamp

The data structure for storing the data you resolve from a timestamp counter set.

struct MTLCounterResultStatistic

The data structure for storing the data you resolve from a statistic counter set.

struct MTLCounterResultStageUtilization

The data structure for storing the data you resolve from a stage-utilization counter set.

