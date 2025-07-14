

- HealthKit
- HKQuery
-  predicateForSamples(withStart:end:options:) 

Type Method

# predicateForSamples(withStart:end:options:)

Returns a predicate for samples whose start and end dates fall within the specified time interval.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class func predicateForSamples(
    withStart startDate: Date?,
    end endDate: Date?,
    options: HKQueryOptions = []
) -> NSPredicate
```

## Parameters 

`startDate`  

The start date for the target time interval.

`endDate`  

The end date for the target time interval.

`options`  

A constant that specifies how the sample’s start and end date are compared with the target time interval. For a list of possible values, see HKQueryOptions.

## Return Value

A predicate for samples whose start and end dates fall within the specified time interval. This predicate works only with samples.

## Discussion

Use this convenience method to create a predicate that compares a sample’s start and end dates with a specified time interval. The following sample uses both the convenience method and a predicate format string to create equivalent predicates.

- Swift
- Objective-C

```
let timeInterval =
    HKQuery.predicateForSamplesWithStartDate(myStartDate,
                                             endDate: myEndDate, options: .None)

let explicitTimeInterval = NSPredicate(format: "%K >= %@ AND %K 

```
NSPredicate *timeInterval =
[HKQuery predicateForSamplesWithStartDate:myStartDate
                                  endDate:myEndDate
                                  options:HKQueryOptionNone];

NSPredicate *explicitTimeInterval =
[NSPredicate predicateWithFormat:@"%K >= %@ AND %K 

## See Also

### Related Documentation

let HKPredicateKeyPathEndDate: String

The key path for accessing the sample’s end date.

let HKPredicateKeyPathStartDate: String

The key path for accessing the sample’s start date.

var endDate: Date

The sample’s end date.

var startDate: Date

The sample’s start date.

### Creating sample predicates

struct HKQueryOptions

Constants that describe how a sample’s time period overlaps with the target time period.

