

- HealthKit
- HKElectrocardiogramQuery
-  init(electrocardiogram:dataHandler:) 

Initializer

# init(electrocardiogram:dataHandler:)

Creates a new electrocardiogram query object.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
init(
    electrocardiogram: HKElectrocardiogram,
    dataHandler: @escaping (HKElectrocardiogramQuery, HKElectrocardiogram.VoltageMeasurement?, Bool, (any Error)?) -> Void
)
```

## Parameters 

`electrocardiogram`  

The electrocardiogram sample whose voltages you want to access.

`dataHandler`  

A block that the query calls repeatedly to return the voltage data. The handler takes the following parameters:

`query`  
The query that returned the results.

`voltageMeasurement`  
A voltage measurement.

`done`  
Indicates whether the query has additional voltage measurements to send.

`error`  
If an error occurred, this parameter contains information about the error. Otherwise it’s `nil`.

## Discussion

When you run the query, it calls the data handler once for each voltage measurement, passing the voltage data. On the last voltage measurement, it sets the `done` parameter to true. If an error occurs, it stops collecting voltage data and calls the data handler; it sets the `voltageMeasurement` parameter to `nil`, and passes in an NSError object that describes the error.

## See Also

### Accessing the Results

enum Result

Partial results for an electrocardiogram query.

