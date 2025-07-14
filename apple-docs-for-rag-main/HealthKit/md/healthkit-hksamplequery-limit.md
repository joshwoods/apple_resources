

- HealthKit
- HKSampleQuery
-  limit 

Instance Property

# limit

The maximum number of samples that this query returns.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
var limit: Int { get }
```

## Discussion

This property’s value sets the maximum number of samples that the query returns upon completion.

If you are specifically interested in retrieving only new samples (samples added since the last query), consider using an HKAnchoredObjectQuery query instead.

## See Also

### Getting Property Data

var sortDescriptors: [NSSortDescriptor]?

The sort descriptors that specify the order of the results returned by this query.

