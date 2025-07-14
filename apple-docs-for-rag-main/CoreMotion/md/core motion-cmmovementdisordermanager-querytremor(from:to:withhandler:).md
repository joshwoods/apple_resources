

- Core Motion
- CMMovementDisorderManager
-  queryTremor(from:to:withHandler:) 

Instance Method

# queryTremor(from:to:withHandler:)

Query for tremor results from the provided time interval.

watchOS 5.0+

``` source
func queryTremor(
    from fromDate: Date,
    to toDate: Date,
    withHandler handler: @escaping CMTremorResultHandler
)
```

## Parameters 

`fromDate`  

The start date and time of the query. The start must be within the last seven days.

`toDate`  

The end date and time of the query. The end must be within the last seven days, and must be after the start date.

`handler`  

A block for handling the tremor results returned by the query.

## Discussion

Use this method to asynchronously query for tremor results recorded by the monitorKinesias(forDuration:) method. The movement disorder manager keeps tremor results for only seven days after the time of recording.

After the manager retrieves the queried results, it calls your handler block from an anonymous background queue. Provide a completion handler to access and process these results.

## See Also

### Related Documentation

func monitorKinesias(forDuration: TimeInterval)

Calculate and store tremor and dyskinetic symptom results for the duration of the specified time interval.

### Querying for Movement Disorders

typealias CMTremorResultHandler

A completion handler for accessing and processing tremor results.

func queryDyskineticSymptom(from: Date, to: Date, withHandler: CMDyskineticSymptomResultHandler)

Query for dyskinetic symptoms from the provided time interval.

typealias CMDyskineticSymptomResultHandler

A completion handler for processing dyskinetic symptom results.

func lastProcessedDate() -> Date?

Returns the date of the most recently calculated results.

