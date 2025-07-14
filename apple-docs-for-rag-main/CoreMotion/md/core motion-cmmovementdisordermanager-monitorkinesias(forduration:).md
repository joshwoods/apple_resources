

- Core Motion
- CMMovementDisorderManager
-  monitorKinesias(forDuration:) 

Instance Method

# monitorKinesias(forDuration:)

Calculate and store tremor and dyskinetic symptom results for the duration of the specified time interval.

watchOS 5.0+

``` source
func monitorKinesias(forDuration duration: TimeInterval)
```

## Parameters 

`duration`  

The monitoring duration in seconds. The maximum duration is seven days.

## Mentioned in 

Getting movement disorder symptom data

## Discussion

Call this method to begin monitoring, calculating, and storing tremor and dyskinetic symptom results. The manager stores results for a period of seven days after the time of recording. You can access the results at any time within that seven-day interval, after which they expire. To retrieve these results, call the queryTremor(from:to:withHandler:) and queryDyskineticSymptom(from:to:withHandler:) methods.

To determine whether the results are currently being monitored and calculated, call the monitorKinesiasExpirationDate() method. The maximum monitoring duration is seven days. In order to continue monitoring beyond the expiration date, you need to renew your subscription by calling monitorKinesias(forDuration:) again before the monitoring period expires. Note that repeated calls allow you to extend monitoring, but not shorten it.

## See Also

### Related Documentation

func queryTremor(from: Date, to: Date, withHandler: CMTremorResultHandler)

Query for tremor results from the provided time interval.

func queryDyskineticSymptom(from: Date, to: Date, withHandler: CMDyskineticSymptomResultHandler)

Query for dyskinetic symptoms from the provided time interval.

### Recording Movement Disorders

func monitorKinesiasExpirationDate() -> Date?

Returns the expiration date for the most recent monitoring period.

