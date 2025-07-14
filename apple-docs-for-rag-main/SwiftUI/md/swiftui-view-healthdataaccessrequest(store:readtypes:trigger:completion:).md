

- SwiftUI
- View
-  healthDataAccessRequest(store:readTypes:trigger:completion:) 

Instance Method

# healthDataAccessRequest(store:readTypes:trigger:completion:)

Requests permission to read the specified HealthKit data types.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+watchOS 10.2+

``` source
@preconcurrency nonisolated
func healthDataAccessRequest(
    store: HKHealthStore,
    readTypes: Set,
    trigger: some Equatable,
    completion: @escaping (Result) -> Void
) -> some View
```

## Parameters 

`store`  

The HealthKit store where you’re requesting authorization.

`readTypes`  

An optional set containing the data types you want to read. This set can contain any concrete subclass of the HKObjectType class (any of the HKCharacteristicType, HKQuantityType, HKCategoryType, HKWorkoutType, or HKCorrelationType classes ). If the user grants permission, your app can read these data types from the HealthKit store.

`trigger`  

A value used to trigger the request. This value must be a State variable. Any change to the variable triggers a request.

`completion`  

A block that the system calls after the request is complete. The system passes the result parameter.

## Discussion

HealthKit performs this request asynchronously when you modify the trigger’s value. If you call this method with a new data type (a type of data that the user hasn’t previously granted or denied permission for in this app), the system automatically displays the authorization sheet when you modify the trigger’s value. The authorization sheet lists all the requested permissions. After the user finishes responding, HealthKit calls the completion block on a background queue. If the user has already chosen to grant or prohibit access to all of the types specified, HealthKit calls the completion when you modify the trigger without prompting the user.

- Authenticating on launch
- Full Swift file

```
@State private var trigger = false

var body: some Scene {
    WindowGroup {
        ContentView(enabled: $authenticated)
            .healthDataAccessRequest(store: store,
                                     readTypes: healthDataTypes,
                                     trigger: trigger) { result in
                switch result {

                case .success(_):
                    authenticated = true
                case .failure(let error):
                    // Handle the error here.
                    fatalError("*** An error occurred while requesting authentication: \(error) ***")
                }

                logger.debug("Authentication Complete.")
            }
            .onAppear() {
                trigger.toggle()
            }
    }
}
```

```
import SwiftUI
import HealthKit
import HealthKitUI
import os

let healthDataTypes: Set = [
    HKQuantityType.workoutType(),
    HKQuantityType(.heartRate),
    HKQuantityType(.activeEnergyBurned),
    HKQuantityType(.basalEnergyBurned),
    HKQuantityType(.distanceWalkingRunning),
    HKQuantityType(.stepCount)
]

private let logger = Logger(subsystem: "example.com.MyWorkoutApp",
                            category: "iOS App")

@main
struct MyApp: App {

    @State private var authenticated = false
    @State private var trigger = false

    let store = HKHealthStore()

    var body: some Scene {
        WindowGroup {
            ContentView(enabled: $authenticated)
                .healthDataAccessRequest(store: store,
                                         readTypes: healthDataTypes,
                                         trigger: trigger) { result in
                    switch result {

                    case .success(_):
                        authenticated = true
                    case .failure(let error):
                        // Handle the error here.
                        fatalError("*** An error occurred while requesting authentication: \(error) ***")
                    }

                    logger.debug("Authentication Complete.")
                }
                .onAppear() {
                    trigger.toggle()
                }
        }
    }
}
```

Customize the messages displayed on the permissions sheet by setting the following key:

- NSHealthShareUsageDescription customizes the message for reading data.

Warning

You must set the usage key, or your app crashes when you request authorization.

Set the key in the Target Properties list on the app’s Info tab.

After users set the permissions for your app, they can always change them using either the Settings or the Health app. Your app appears in the Health app’s Sources tab, even if the user didn’t allow permission to read data.

## See Also

### Accessing health data

func healthDataAccessRequest(store: HKHealthStore, objectType: HKObjectType, predicate: NSPredicate?, trigger: some Equatable, completion: (Result&lt;Bool, any Error>) -> Void) -> some View

Asynchronously requests permission to read a data type that requires per-object authorization (such as vision prescriptions).

func healthDataAccessRequest(store: HKHealthStore, shareTypes: Set&lt;HKSampleType>, readTypes: Set&lt;HKObjectType>?, trigger: some Equatable, completion: (Result&lt;Bool, any Error>) -> Void) -> some View

Requests permission to save and read the specified HealthKit data types.

func workoutPreview(WorkoutPlan, isPresented: Binding&lt;Bool>) -> some View

Presents a preview of the workout contents as a modal sheet

