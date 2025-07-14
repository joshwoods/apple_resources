

- HealthKit
- HKHealthStore
-  preferredUnits(for:completion:) 

Instance Method

# preferredUnits(for:completion:)

Returns the user’s preferred units for the given quantity types.

iOS 8.2+iPadOS 8.2+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
func preferredUnits(
    for quantityTypes: Set,
    completion: @escaping ([HKQuantityType : HKUnit], (any Error)?) -> Void
)
```

``` source
func preferredUnits(for quantityTypes: Set) async throws -> [HKQuantityType : HKUnit]
```

## Parameters 

`quantityTypes`  

A set of HKQuantityType identifiers. These identifiers represent the quantity types to be examined. Before calling this method, your app must request read or share access to all the types in this set.

`completion`  

A block that this method calls as soon as it finishes looking up the preferred units. This block is passed the following parameters:

preferredUnits  
If the lookup is successful, this parameter contains a dictionary with `HKQuantityType` identifiers for the keys and HKUnit objects for the values. The keys match those passed to the `quantityTypes` parameter. If an error occurs, this parameter is set to `nil`.

error  
An error object. This method returns an error if the preferred units are inaccessible or if your app has not yet requested permission to access the quantity types; otherwise, this parameter is set to `nil`.

## Discussion

This method runs asynchronously. As soon as it finishes looking up the preferred units, it calls the completion block on an anonymous background queue.

By default, the preferred units are based on the device’s current locale. For example, in the US, the preferred units for the bodyMass identifier are pounds. Other regions may use kilograms or stones. However, users can change their preferred units in the Health app at any time.

Your app should present HealthKit data using the current preferred units (see the bloodGlucose results identifier for an exception). You should also observe the HKUserPreferencesDidChange notification, and update the user interface whenever the user changes his or her preferred units.

Note

The results returned by this method are based on your app’s permissions:

- If you have never requested access for a type, this method returns an authorization not determined error.

- If the user denied access to a type, this method returns the default units for the device’s current locale for that type.

- If the user granted either read or share access, this method returns the current preferred units for that type (which may or may not be the default units).

## See Also

### Accessing the preferred units

static let HKUserPreferencesDidChange: NSNotification.Name

Notifies observers whenever the user changes his or her preferred units.

