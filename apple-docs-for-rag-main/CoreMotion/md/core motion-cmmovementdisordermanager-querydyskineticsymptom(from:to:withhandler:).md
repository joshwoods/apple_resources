

- Core Motion
- CMMovementDisorderManager
-  queryDyskineticSymptom(from:to:withHandler:) 

Instance Method

# queryDyskineticSymptom(from:to:withHandler:)

Query for dyskinetic symptoms from the provided time interval.

watchOS 5.0+

``` source
func queryDyskineticSymptom(
    from fromDate: Date,
    to toDate: Date,
    withHandler handler: @escaping CMDyskineticSymptomResultHandler
)
```

## Parameters 

`fromDate`  

The start date and time of the query. The start must be within the last seven days.

`toDate`  

The end date and time of the query. The end must be within the last seven days, and must be after the start date.

`handler`  

A block for handling the dyskinetic symptom results returned by the query.

## Discussion

Use this method to asynchronously query for dyskinetic symptoms recorded by the monitorKinesias(forDuration:) method. The movement disorder manager keeps dyskinetic symptom results for only seven days after the time of recording.

After the manager retrieves the queried results, it calls your handler block from an anonymous background queue. Provide a completion handler to access and process these results.

## See Also

### Related Documentation

func monitorKinesias(forDuration: TimeInterval)

Calculate and store tremor and dyskinetic symptom results for the duration of the specified time interval.

### Querying for Movement Disorders

func queryTremor(from: Date, to: Date, withHandler: CMTremorResultHandler)

Query for tremor results from the provided time interval.

typealias CMTremorResultHandler

A completion handler for accessing and processing tremor results.

typealias CMDyskineticSymptomResultHandler

A completion handler for processing dyskinetic symptom results.

func lastProcessedDate() -> Date?

Returns the date of the most recently calculated results.

