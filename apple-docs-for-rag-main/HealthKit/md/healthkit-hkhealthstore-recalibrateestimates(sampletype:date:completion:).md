

- HealthKit
- HKHealthStore
-  recalibrateEstimates(sampleType:date:completion:) 

Instance Method

# recalibrateEstimates(sampleType:date:completion:)

Recalibrates the prediction algorithm used to calculate the specified sample type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 13.0+visionOS 1.0+watchOS 8.0+

``` source
func recalibrateEstimates(
    sampleType: HKSampleType,
    date: Date,
    completion: @escaping (Bool, (any Error)?) -> Void
)
```

``` source
func recalibrateEstimates(
    sampleType: HKSampleType,
    date: Date
) async throws
```

## Parameters 

`sampleType`  

The sample type to recalibrate.

`date`  

The effective date for the recalibration.

`completion`  

A completion block that the system calls after recalibrating the data used by the prediction algorithm. The system passes the following parameters:

`success`  
A Boolean value that indicates whether the system successfully recalibrated the sample type’s estimates.

`error`  
If `success` is false, this parameter contains error information; otherwise, it’s `nil`.

## Discussion

Your app can use this method to recalibrate HealthKitʼs prediction algorithms after an event that may significantly affect their results. For example, you can recalibrate the sixMinuteWalkTestDistance type to use only data collected after a mobility-impacting health event, such as surgery or an injury. Recalibrating sixMinuteWalkTestDistance after such an event may yield more accurate estimates during the recovery period.

Warning

Before calling this method, your app must include the `com.apple.developer.healthkit.recalibrate-estimates` entitlement. Also, you must request both share and read access to all the data types you pass to the `sampleType` parameter. If you haven’t completed all of these steps, recalibration fails with an HKError.Code.errorAuthorizationDenied error.

Check the HKSampleType class’s allowsRecalibrationForEstimates method to see if a given sample type supports recalibrating the algorithm.

The following sample code recalibrates the estimates for the six-minute walk test.

```
// Access the HealthKit Store.
let healthStore = HKHealthStore()

// Get the six-minute walk test type.
let sixMinuteWalkType = HKQuantityType(.sixMinuteWalkTestDistance)

// Verify that the type supports resetting estimates.
if sixMinuteWalkType.allowsRecalibrationForEstimates {

    // Reset the estimate.
    healthStore.recalibrateEstimates(sampleType: sixMinuteWalkType, date: Date()) { (success, error) in

        // Check the success value.
        if !success {
            if let error = error {
                // Handle errors here.
            }
        }
    }
}
```

