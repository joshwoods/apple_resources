

- Core Motion
-  CMTremorResultHandler 

Type Alias

# CMTremorResultHandler

A completion handler for accessing and processing tremor results.

watchOS 5.0+

``` source
typealias CMTremorResultHandler = ([CMTremorResult], (any Error)?) -> Void
```

## Parameters 

`tremorResult`  

An array of tremor results found by the query.

`error`  

If an error occurred, this parameter contains information about the error; otherwise it is `nil`.

## See Also

### Querying for Movement Disorders

func queryTremor(from: Date, to: Date, withHandler: CMTremorResultHandler)

Query for tremor results from the provided time interval.

func queryDyskineticSymptom(from: Date, to: Date, withHandler: CMDyskineticSymptomResultHandler)

Query for dyskinetic symptoms from the provided time interval.

typealias CMDyskineticSymptomResultHandler

A completion handler for processing dyskinetic symptom results.

func lastProcessedDate() -> Date?

Returns the date of the most recently calculated results.

