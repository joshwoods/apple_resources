

- HealthKit
- HKQuantitySeriesSampleBuilder
-  discard() 

Instance Method

# discard()

Discards all previously collected data and invalidates the builder.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 5.0+

``` source
func discard()
```

## See Also

### Ending the Collection

func finishSeries(metadata: [String : Any]?, completion: ([HKQuantitySample]?, (any Error)?) -> Void)

Finalizes the series and returns the resulting quantity samples.

func finishSeries(metadata: [String : Any]?, endDate: Date?, completion: ([HKQuantitySample]?, (any Error)?) -> Void)

Finalizes the series with the provided end date, and returns the resulting quantity samples.

