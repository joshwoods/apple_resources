

- Core Location
-  CLLocationManager 

Class

# CLLocationManager

The object you use to start and stop the delivery of location-related events to your app.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class CLLocationManager
```

## Mentioned in 

Determining the proximity to an iBeacon device

Getting heading and course information

Converting between coordinates and user-friendly place names

Getting the current location of a device

Configuring your app to use location services

## Overview

A CLLocationManager object is the central place to manage your app’s location-related behaviors. Use a location-manager object to configure, start, and stop location services. You might use these services to:

- Track large or small changes in the user’s current location with a configurable degree of accuracy.

- Report heading changes from the onboard compass.

- Monitor geographical regions of interest and generate events when someone enters or leaves those regions.

- Report the range to nearby Bluetooth beacons.

Create one or more location-manager objects in your app and use them where you need location data. After you create a location-manager object, configure it so that Core Location knows how often to report location changes. In particular, configure the distanceFilter and desiredAccuracy properties with values that reflect your app’s needs.

A CLLocationManager object reports all location-related updates to its delegate object, which is an object that conforms to the CLLocationManagerDelegate protocol. Assign the delegate immediately when you configure your location manager, because the system reports the app’s authorization status to the delegate’s locationManagerDidChangeAuthorization(_:) method after the location manager finishes initializing itself. Core Location calls the methods of your delegate object using the RunLoop of the thread on which you initialized the CLLocationManager object. That thread must itself have an active RunLoop, like the one found in your app’s main thread.

For more information, see Configuring your app to use location services.

## Topics

### Determining the availability of services

class func significantLocationChangeMonitoringAvailable() -> Bool

Returns a Boolean value indicating whether the significant-change location service is available on the device.

class func headingAvailable() -> Bool

Returns a Boolean value indicating whether the location manager is able to generate heading-related events.

var isAuthorizedForWidgetUpdates: Bool

A Boolean value that indicates whether a widget is eligible to receive location updates.

var accuracyAuthorization: CLAccuracyAuthorization

A value that indicates the level of location accuracy the app has permission to use.

class func isMonitoringAvailable(for: AnyClass) -> Bool

Returns a Boolean value indicating whether the device supports region monitoring using the specified class.

class func isRangingAvailable() -> Bool

Returns a Boolean value indicating whether the device supports ranging of beacons that use the iBeacon protocol.

class func locationServicesEnabled() -> Bool

Returns a Boolean value indicating whether location services are enabled on the device.

### Receiving data from location services

var delegate: (any CLLocationManagerDelegate)?

The delegate object to receive update events.

protocol CLLocationManagerDelegate

The methods you use to receive events from an associated location-manager object.

### Requesting authorization for location services

func requestWhenInUseAuthorization()

Requests the user’s permission to use location services while the app is in use.

func requestAlwaysAuthorization()

Requests the user’s permission to use location services regardless of whether the app is in use.

func requestTemporaryFullAccuracyAuthorization(withPurposeKey: String, completion: (((any Error)?) -> Void)?)

Requests permission to temporarily use location services with full accuracy and reports the results to the provided completion handler.

func requestTemporaryFullAccuracyAuthorization(withPurposeKey: String)

Requests permission to temporarily use location services with full accuracy.

var authorizationStatus: CLAuthorizationStatus

The current authorization status for the app.

enum CLAuthorizationStatus

Constants that indicate the app’s authorization to use location services.

NSLocationDefaultAccuracyReduced

A Boolean value that indicates whether the app requests reduced location accuracy by default.

NSLocationAlwaysAndWhenInUseUsageDescription

A message that tells the user why the app is requesting access to the user’s location information at all times.

### Specifying distance and accuracy

var distanceFilter: CLLocationDistance

The minimum distance in meters the device must move horizontally before an update event is generated.

let CLLocationDistanceMax: CLLocationDistance

A constant indicating the maximum distance.

let kCLDistanceFilterNone: CLLocationDistance

A constant indicating that all movement should be reported.

typealias CLLocationDistance

A distance in meters from an existing location.

var desiredAccuracy: CLLocationAccuracy

The accuracy of the location data that your app wants to receive.

typealias CLLocationAccuracy

The accuracy of a geographical coordinate.

### Running the standard location service

func startUpdatingLocation()

Starts the generation of updates that report the user’s current location.

func stopUpdatingLocation()

Stops the generation of location updates.

func requestLocation()

Requests the one-time delivery of the user’s current location.

var pausesLocationUpdatesAutomatically: Bool

A Boolean value that indicates whether the location-manager object may pause location updates.

var allowsBackgroundLocationUpdates: Bool

A Boolean value that indicates whether the app receives location updates when running in the background.

var showsBackgroundLocationIndicator: Bool

A Boolean value that indicates whether the status bar changes its appearance when an app uses location services in the background.

var activityType: CLActivityType

The type of activity the app expects the user to typically perform while in the app’s location session.

enum CLActivityType

Constants that indicate the type of activity associated with location updates.

### Running the significant change location service

func startMonitoringSignificantLocationChanges()

Starts the generation of updates based on significant location changes.

func stopMonitoringSignificantLocationChanges()

Stops the delivery of location events based on significant location changes.

### Running the visits location service

func startMonitoringVisits()

Starts the delivery of visit-related events.

func stopMonitoringVisits()

Stops the delivery of visit-related events.

### Running the heading service

func startUpdatingHeading()

Starts the generation of updates that report the user’s current heading.

func stopUpdatingHeading()

Stops the generation of heading updates.

func dismissHeadingCalibrationDisplay()

Dismisses the heading calibration view from the screen immediately.

var headingFilter: CLLocationDegrees

The minimum angular change in degrees required to generate new heading events.

let kCLHeadingFilterNone: CLLocationDegrees

A constant indicating that all header values should be reported.

typealias CLLocationDegrees

A latitude or longitude value specified in degrees.

var headingOrientation: CLDeviceOrientation

The device orientation to use when computing heading values.

enum CLDeviceOrientation

Constants indicating the physical orientation of the device.

### Running the region-monitoring service

var monitoredRegions: Set&lt;CLRegion>

The set of shared regions monitored by all location-manager objects.

var maximumRegionMonitoringDistance: CLLocationDistance

The largest boundary distance that can be assigned to a region.

### Performing beacon ranging

func startRangingBeacons(satisfying: CLBeaconIdentityConstraint)

Starts the delivery of notifications for the specified beacon constraints.

func stopRangingBeacons(satisfying: CLBeaconIdentityConstraint)

Stops the delivery of notifications for the specified beacon constraints.

var rangedBeaconConstraints: Set&lt;CLBeaconIdentityConstraint>

The set of beacon constraints currently being tracked using ranging.

### Monitoring location push notifications

func startMonitoringLocationPushes(completion: ((Data?, (any Error)?) -> Void)?)

Starts monitoring for the delivery of Apple Push Notification service (APNs) location pushes, and provides a device-specific token for sending pushes.

func stopMonitoringLocationPushes()

Stops monitoring for Apple Push Notification service (APNs) location pushes.

### Getting recent location and heading data

var location: CLLocation?

The most recently retrieved user location.

var heading: CLHeading?

The most recently reported heading.

### Deferring location updates

let CLTimeIntervalMax: TimeInterval

A value representing an unlimited amount of time.

### Deprecated

Deprecated symbols

Review unsupported symbols and their replacements.

### Instance Methods

func requestHistoricalLocations(purposeKey: String, sampleCount: Int, completionHandler: ([CLLocation], (any Error)?) -> Void)

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Essentials

Configuring your app to use location services

Prepare your app to start collecting location data.

Supporting live updates in SwiftUI and Mac Catalyst apps

Enable background events by adding lifecycle event support.

class CLBackgroundActivitySession

An object that manages a visual indicator that keeps your app in use in the background, allowing it to receive updates or events.

struct CLLocationUpdate

A structure that contains the location information the framework delivers with each update.

Adopting live updates in Core Location

Simplify location delivery using asynchronous events in Swift.

Monitoring location changes with Core Location

Define boundaries and act on user location updates.

