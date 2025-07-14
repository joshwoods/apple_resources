

- HealthKit
- Workouts and activity rings
-  Creating a workout route 

Article

# Creating a workout route

Record the user’s route during a workout.

## Overview

Your app can create a route (for example, the user’s path when walking, running, or cycling) and associate it with a workout in HealthKit. During the workout, your app can track the user, gathering a series of location updates. These updates represent both the user’s location (longitude, latitude, and altitude) and the update’s time. Other apps can then use these locations to plot the route on a map, or to calculate metrics not already provided by HealthKit (for example, the user’s speed over specific intervals during the workout).

To create a workout route:

1.  **Request permissions.** Before starting a workout, your app must request permission to use both the required HealthKit data types and Core Location updates.

2.  **Start the workout.** Setup the route builder object and start tracking the user’s location.

3.  **Add locations to the builder.** As your app receives location updates from Core Location, filter and smooth the updates as needed, and add them to the route builder.

4.  **End the workout.** Stop tracking the user’s location. Save the workout to the HealthKit store.

5.  **Finish the route.** Tell the route builder to save the route and associates it with the workout.

### Request Permissions

As noted in Setting up HealthKit, you must request permission from the user before using any data in HealthKit. Specifically for route data, you must request permission to read and share both HKWorkout and HKWorkoutRoute samples.

You must also request permission to use location services before your app receives location updates from Core Location. For more information on requesting permission to use location services, see CLLocationManager.

### Start the Workout

When the user starts a new workout, begin tracking the user’s location using a CLLocationManager object from the Core Location framework. After you call the location manager’s startUpdatingLocation() method, the location manager’s delegate begins receiving updates containing the user’s current location.

```
// Start tracking the user.
locationManager.desiredAccuracy = kCLLocationAccuracyBest
locationManager.startUpdatingLocation()
```

Next, create and store a route builder for the workout. During the workout, you incrementally add locations from the Core Location updates to the route builder, which then creates the route from the accumulated data.

```
// Create the route builder.
routeBuilder = HKWorkoutRouteBuilder(healthStore: store, device: nil)
```

### Add Locations to the Builder

As your app receives location updates from Core Location, filter and smooth the locations, and then call insertRouteData(_:completion:) to add the locations to the route builder.

```
// MARK: - CLLocationManagerDelegate Methods.
func locationManager(_ manager: CLLocationManager, didUpdateLocations locations: [CLLocation]) {

    // Filter the raw data.
    let filteredLocations = locations.filter { (location: CLLocation) -> Bool in
        location.horizontalAccuracy 

Because raw Core Location data can contain a significant amount of noise, your app needs to filter out any inaccurate locations before adding them to the route builder. Don’t add any locations whose accuracy is greater than 50 meters. For best results, try to keep the time between locations to 3 seconds or less.

### End the Workout

When the user ends the workout, stop tracking the user and save the workout to the HealthKit store. For more information on saving workouts, see Saving data to HealthKit.

### Finish the Route

After saving the workout, add any remaining locations to the route builder and call finishRoute(with:metadata:completion:).

```
// Create, save, and associate the route with the provided workout.
routeBuilder.finishRoute(with: myWorkout, metadata: myMetadata) { (newRoute, error) in

    guard newRoute != nil else {
        // Handle any errors here.
        return
    }

    // Optional: Do something with the route here.
}
```

The builder then processes the route data. If there are no errors, the builder saves the workout route to the HealthKit store and associates it with the provided workout. It then calls the completion handler and passes in the newly created route object.

If an error occurs, the builder calls the completion handler and passes an error object instead. Your app must handle the error and either try again or fail gracefully.

You can only associate a route with a single workout. After creating a route, you cannot change its workout.

## See Also

### Route data

Reading route data

Access the user’s route for a workout.

class HKWorkoutRouteBuilder

A builder object that incrementally constructs a workout route.

class HKWorkoutRoute

A sample that contains a workout’s route data.

struct HKWorkoutRouteQueryDescriptor

A query interface that reads the location data stored in a workout route using Swift concurrency.

class HKWorkoutRouteQuery

A query to access the location data stored in a workout route.

let HKWorkoutRouteTypeIdentifier: String

A series sample containing location data that defines the route the user took during a workout.

class HKSeriesBuilder

An abstract base class for building series samples.

class HKSeriesSample

An abstract base class that defines samples that contain a series of items.

