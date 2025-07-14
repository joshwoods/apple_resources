

- HealthKit
- HKQuantitySeriesSampleBuilder
-  finishSeries(metadata:endDate:completion:) 

Instance Method

# finishSeries(metadata:endDate:completion:)

Finalizes the series with the provided end date, and returns the resulting quantity samples.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 5.0+

``` source
func finishSeries(
    metadata: [String : Any]?,
    endDate: Date?,
    completion: @escaping ([HKQuantitySample]?, (any Error)?) -> Void
)
```

``` source
func finishSeries(
    metadata: [String : Any]?,
    endDate: Date?
) async throws -> [HKQuantitySample]
```

## Parameters 

`metadata`  

The metadata dictionary contains extra information describing all the samples created by the builder. The dictionary’s keys are all strings. The values may be strings, numbers, or date objects. For a complete list of predefined metadata keys, see Metadata Keys.

Using predefined keys helps facilitate sharing data between apps; however, you are also encouraged to create your own, custom keys as needed to extend the samples’ capabilities.

`endDate`  

The date when the sample ends. If `nil`, the builder uses the latest end date from the contained quantities.

The sample builder returns an HKError.Code.errorInvalidArgument error if the `endDate` is earlier than the builder’s startDate parameter, or is earlier than the end date of any of the quantities inserted into the builder.

`completion`  

A completion handler, called by the builder after it creates the samples.

The handler takes the following parameters:

**samples**  
The samples returned by the builder, or `nil` if an error occurs.

**error**  
If an error occurs, this contains an object that describes the error. Otherwise, it is `nil`.

## Discussion

Call finishSeries(metadata:endDate:completion:) after inserting all the quantities for the series. The series builder then creates one or more samples to represent the series, saves the samples to the HealthKit store, and then passes them to the completion handler.

Note

The series builder typically creates a single sample that contains all the inserted quantities; however, it may split the quantities up into multiple sample objects.

Calling this method before inserting any samples results in an error. Also, calling this method invalidates the series builder; you cannot call any other series builder methods after calling this method.

## See Also

### Ending the Collection

func discard()

Discards all previously collected data and invalidates the builder.

func finishSeries(metadata: [String : Any]?, completion: ([HKQuantitySample]?, (any Error)?) -> Void)

Finalizes the series and returns the resulting quantity samples.

