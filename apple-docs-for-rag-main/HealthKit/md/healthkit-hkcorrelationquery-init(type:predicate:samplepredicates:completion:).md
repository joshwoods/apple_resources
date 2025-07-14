

- HealthKit
- HKCorrelationQuery
-  init(type:predicate:samplePredicates:completion:) 

Initializer

# init(type:predicate:samplePredicates:completion:)

Instantiates and returns a correlation query.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    type correlationType: HKCorrelationType,
    predicate: NSPredicate?,
    samplePredicates: [HKSampleType : NSPredicate]?,
    completion: @escaping (HKCorrelationQuery, [HKCorrelation]?, (any Error)?) -> Void
)
```

## Parameters 

`correlationType`  

The type of correlation to search for.

`predicate`  

A predicate that limits the results returned by the query. This predicate is compared with the correlation objects. Pass `nil` to receive all the correlations of the specified type.

`samplePredicates`  

A dictionary whose keys are HKSampleType instances, and whose values are NSPredicate instances. The query iterates over all the samples in the correlation. For each sample, it looks up the corresponding predicate based on the sample’s type and then evaluates that predicate against the sample. If the dictionary does not contain a matching sample type, the query treats it as a `nil` predicate, and accepts the sample.

Three things must be true if this query is going to match a correlation:

- The correlation object must match the provided predicate parameter.

- For each key in the sample predicate dictionary, the correlation must contain a sample whose type matches the key. In other words, the keys from the sample predicate dictionary define the set of required samples for the correlation.

- For each sample in the correlation, use the sample’s type to look up its predicate in the sample predicate dictionary. If the dictionary contains a matching predicate, the sample must match that predicate. If the dictionary does not contain a matching predicate, the sample is ignored (it can have any value).

`completion`  

A block that is called when the query finishes executing. This block takes the following parameters:

query  
A reference to the query that called this block.

correlations  
An array containing the correlations found by the query, or `nil` if an error occurs.

error  
If an error occurred, this parameter contains an object describing the error; otherwise, it is `nil`.

## Return Value

A newly initialized correlation object.

## Discussion

After instantiating the query, run it by calling the HKHealthStore class’s execute(_:) method. Queries run on a background thread. As soon as the query is complete, the results handler is executed on the background thread. You typically dispatch these results to the main thread to update the user interface.

