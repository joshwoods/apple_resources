

- Core Motion
-  CMDyskineticSymptomResultHandler 

Type Alias

# CMDyskineticSymptomResultHandler

A completion handler for processing dyskinetic symptom results.

watchOS 5.0+

``` source
typealias CMDyskineticSymptomResultHandler = ([CMDyskineticSymptomResult], (any Error)?) -> Void
```

## Parameters 

`dyskineticSymptomResult`  

An array of dyskinetic symptom results found by the query.

`error`  

If an error occurred, this parameter contains information about the error; otherwise it is `nil`.

## See Also

### Querying for Movement Disorders

func queryTremor(from: Date, to: Date, withHandler: CMTremorResultHandler)

Query for tremor results from the provided time interval.

typealias CMTremorResultHandler

A completion handler for accessing and processing tremor results.

func queryDyskineticSymptom(from: Date, to: Date, withHandler: CMDyskineticSymptomResultHandler)

Query for dyskinetic symptoms from the provided time interval.

func lastProcessedDate() -> Date?

Returns the date of the most recently calculated results.

