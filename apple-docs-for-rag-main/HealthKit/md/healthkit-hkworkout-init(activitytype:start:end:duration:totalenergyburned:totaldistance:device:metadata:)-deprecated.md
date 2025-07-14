

- HealthKit
- HKWorkout
-  init(activityType:start:end:duration:totalEnergyBurned:totalDistance:device:metadata:) Deprecated

Initializer

# init(activityType:start:end:duration:totalEnergyBurned:totalDistance:device:metadata:)

Instantiates a new workout activity that includes the device that produced the sample data.

iOS 9.0–17.0DeprecatediPadOS 9.0–17.0DeprecatedMac Catalyst 13.0–16.0DeprecatedmacOS 13.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–10.0Deprecated

``` source
convenience init(
    activityType workoutActivityType: HKWorkoutActivityType,
    start startDate: Date,
    end endDate: Date,
    duration: TimeInterval,
    totalEnergyBurned: HKQuantity?,
    totalDistance: HKQuantity?,
    device: HKDevice?,
    metadata: [String : Any]?
)
```

Deprecated

Use HKWorkoutBuilder

## Parameters 

`workoutActivityType`  

The type of activity performed during the workout. For a complete list of activity types, see HKWorkoutActivityType.

`startDate`  

The date and time when the activity started.

`endDate`  

The date and time when the activity ended. This date must be equal to or later than the start date.

`duration`  

A time interval representing the workout’s actual duration. Passing a nonzero value sets the workout’s duration property. If you pass 0, this method calculates the duration property based on the workout’s start and end dates.

`totalEnergyBurned`  

A quantity using energy units, or `nil`. This property sets the workout’s totalEnergyBurned property. It represents the total active energy burned during the workout.

`totalDistance`  

A quantity using length units, or `nil`. This property sets the workout’s totalDistance property.

`device`  

The device that generated the data for this sample.

`metadata`  

The metadata dictionary contains extra information describing this workout. The dictionary’s keys are all NSString objects . The values may be NSString, NSNumber, or NSDate objects. For a complete list of predefined metadata keys, see Metadata Keys.

Using predefined keys helps facilitate sharing data between apps; however, you are also encouraged to create your own, custom keys as needed to extend the workout’s capabilities.

## Return Value

A workout object with the provided duration, total energy burned, total distance, device, and metadata properties. The workoutEvents property is set to `nil`.

## Discussion

This method returns a workout with the specified duration, total energy burned, total distance, device, and metadata. The workoutEvents property is set to `nil`.

If the total energy burned or total distance are non-zero values, create a set of corresponding samples that add up to the calculated totals. Associate these samples with the workout by calling the health store’s add(_:to:completion:) method.

- Swift
- Objective-C

```
let distance = HKQuantity(unit: HKUnit.mileUnit(), doubleValue: 5.2)
let energyBurned = HKQuantity(unit: HKUnit.kilocalorieUnit(), doubleValue: 259.0)

let device = HKDevice(name: deviceName,
                      manufacturer: manufacturerName,
                      model: modelName,
                      hardwareVersion: hardwareVersionNumber,
                      firmwareVersion: firmwareVersionNumber,
                      softwareVersion: softwareVersionNumber,
                      localIdentifier: localIdentifier,
                      UDIDeviceIdentifier: deviceIdentifier)

let metadata = [HKMetadataKeyIndoorWorkout:false]

let hike = HKWorkout(activityType: HKWorkoutActivityType.Hiking, startDate: start, endDate: end, duration: 9000, totalEnergyBurned: energyBurned, totalDistance: distance, device: device, metadata: metadata)

healthStore.saveObject(hike) { (success, error) -> Void in

    guard success else {
        // Perform proper error handling here...
        fatalError("*** An error occurred while saving this " +
            "workout: \(error?.localizedDescription)")
    }
}
```

```

HKQuantity *distance = [HKQuantity quantityWithUnit:[HKUnit mileUnit]
                                        doubleValue:5.2];

HKQuantity *energyBurned = [HKQuantity quantityWithUnit:[HKUnit kilocalorieUnit]
                                            doubleValue:259.0];

HKDevice *device = [[HKDevice alloc] initWithName:deviceName
                                     manufacturer:manufacturerName
                                            model:modelName
                                  hardwareVersion:hardwareVersionNumber
                                  firmwareVersion:firmwareVersionNumber
                                  softwareVersion:softwareVersionNumber
                                  localIdentifier:localIdentifier
                              UDIDeviceIdentifier:deviceIdentifier];

NSDictionary *metadata = @{HKMetadataKeyIndoorWorkout: @(NO)};

HKWorkout *hike = [HKWorkout workoutWithActivityType:HKWorkoutActivityTypeHiking
                                           startDate:start
                                             endDate:end
                                            duration:9000
                                   totalEnergyBurned:energyBurned
                                       totalDistance:distance
                                              device:device
                                            metadata:metadata];

[self.healthStore
 saveObject:hike
 withCompletion:^(BOOL success, NSError *error) {

     if (!success) {
         // Perform proper error handling here...
         NSLog(@"*** An error occurred while saving this "
               @"workout: %@ ***", error.localizedDescription);

         abort();
     }

 }];
```

## See Also

### Related Documentation

var workoutActivityType: HKWorkoutActivityType

The type of activity performed during the workout.

var totalDistance: HKQuantity?

The total distance traveled during the workout.

Deprecated

var duration: TimeInterval

The workout’s duration.

var metadata: [String : Any]?

The metadata for this HealthKit object.

var totalEnergyBurned: HKQuantity?

The total active energy burned during the workout.

Deprecated

var workoutEvents: [HKWorkoutEvent]?

An array of workout event objects.

### Creating workouts

convenience init(activityType: HKWorkoutActivityType, start: Date, end: Date)

Instantiates a new workout.

Deprecated

convenience init(activityType: HKWorkoutActivityType, start: Date, end: Date, duration: TimeInterval, totalEnergyBurned: HKQuantity?, totalDistance: HKQuantity?, metadata: [String : Any]?)

Instantiates a new workout that includes the energy burned, distance, and metadata for the workout.

Deprecated

convenience init(activityType: HKWorkoutActivityType, start: Date, end: Date, workoutEvents: [HKWorkoutEvent]?, totalEnergyBurned: HKQuantity?, totalDistance: HKQuantity?, metadata: [String : Any]?)

Instantiates a new workout whose duration is calculated based on the start and end dates and the provided workout events.

Deprecated

convenience init(activityType: HKWorkoutActivityType, start: Date, end: Date, workoutEvents: [HKWorkoutEvent]?, totalEnergyBurned: HKQuantity?, totalDistance: HKQuantity?, device: HKDevice?, metadata: [String : Any]?)

Instantiates a workout that includes both workout events and the device that produced the sample data.

Deprecated

convenience init(activityType: HKWorkoutActivityType, start: Date, end: Date, workoutEvents: [HKWorkoutEvent]?, totalEnergyBurned: HKQuantity?, totalDistance: HKQuantity?, totalFlightsClimbed: HKQuantity?, device: HKDevice?, metadata: [String : Any]?)

Instantiates a workout using a variety of data, including the number of flights of stairs climbed.

Deprecated

convenience init(activityType: HKWorkoutActivityType, start: Date, end: Date, workoutEvents: [HKWorkoutEvent]?, totalEnergyBurned: HKQuantity?, totalDistance: HKQuantity?, totalSwimmingStrokeCount: HKQuantity?, device: HKDevice?, metadata: [String : Any]?)

Instantiates a workout using a variety of data, including the number of strokes while swimming.

Deprecated

