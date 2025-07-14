

- ARKit
-  ARGeoTrackingConfiguration 

Class

# ARGeoTrackingConfiguration

A configuration that tracks locations with GPS, map data, and a device’s compass.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class ARGeoTrackingConfiguration
```

## Overview

This configuration creates location anchors (ARGeoAnchor) that specify a particular latitude, longitude, and optionally, altitude to enable an app to track geographic areas of interest in an AR experience.

Important

The isSupported property returns true for this class on iOS 14 & iPadOS 14 devices that have an A12 chip or later and cellular (GPS) capability. Geotracking is available in specific geographic locations. To determine availability at the user’s location at runtime, call checkAvailability(completionHandler:).

Geotracking occurs exclusively outdoors. If a geotracking app navigates users between waypoints, your app needs to handle any events along a route. The user must have an internet connection, and you can provide them information about data usage, as described in ARGeoAnchor.

### Encourage User Safety

To keep your users’ focus on the road while traveling, discourage them from looking at the device when in motion, such as while riding a bike. Keep users informed when navigating through unfamiliar territory. For instance, you can recommend they steer clear of private property, or remind them to check their device’s battery level before beginning a long route.

### Refine the User’s Position with Imagery

To place location anchors with precision, geotracking requires a better understanding of the user’s geographic location than is possible with GPS alone. Based on the user’s GPS coordinates, ARKit downloads imagery that depicts the physical environment in that area. Apple collects this *localization imagery* in advance by capturing photos of the view from the street and recording the geographic position at each photo. By comparing the device’s current camera image with this imagery, the session matches the user’s precise geographic location with the scene’s local coordinates. For information about the user’s position in local space, see transform.

Localization imagery captures views from public streets and routes accessible by car, but doesn’t include images of gated or pedestrian-only areas.

Geotracking sessions use localization imagery in the ARGeoTrackingStatus.State.localizing state.

### Supported Areas and Cities

Localization imagery is available for specific areas, including the following U.S. cities:

Arizona  
Phoenix

California  
Alameda, Arden Arcade, Contra Costa, Los Angeles County, Marin County, Napa County, Orange County, Riverside, Roseville, Sacramento, San Bernadino, San Diego, San Francisco, San Jose, San Mateo, Santa Clara, Santa Cruz, Solano County, Sonoma County

Colorado  
Denver

Florida  
Clearwater, Miami, St. Petersburg, Tampa

Georgia  
Atlanta

Indiana  
Bloomington

Maryland  
Baltimore, Towson

Massachusetts  
Boston

Michigan  
Detroit, Livonia, Warren

Minnesota  
Minneapolis, St. Paul

Missouri  
St. Louis

Nevada  
Las Vegas

New Jersey  
Jersey City

New York  
New York City

Oregon  
Hillsboro, Portland

Pennsylvania  
Philadelphia, Pittsburgh

Texas  
Austin, Dallas, Houston, New Braunfels, San Antonio

Washington, D.C.  

Washington  
Seattle, Vancouver

Localization imagery is also available here:

Australia  
Sydney, Melbourne

Canada  
Vancouver, Montreal, Toronto

Japan  
Fukuoka, Hiroshima, Kyoto, Nagoya, Osaka, Tokyo, Yokohama

Singapore  

United Kingdom  
London

Tip

You can share an experience of geotracking with developers who live outside an area that supports it. Record a session in your app in an area that supports localization imagery for developers to create and test their geotracking app. For more information, see Recording and Replaying AR Session Data.

## Topics

### Creating a Configuration

init()

Initializes a new geotracking configuration.

### Checking Availability

class func checkAvailability(completionHandler: (Bool, (any Error)?) -> Void)

Determines if geotracking supports the user’s current location.

class func checkAvailability(at: CLLocationCoordinate2D, completionHandler: (Bool, (any Error)?) -> Void)

Determines if geotracking supports a particular location.

### Tracking Surfaces

var planeDetection: ARWorldTrackingConfiguration.PlaneDetection

A value that specifies whether and how the session automatically attempts to detect flat surfaces in the camera-captured image.

struct PlaneDetection

Options for whether and how the framework detects flat surfaces in captured images.

### Detecting or Tracking Images

var detectionImages: Set&lt;ARReferenceImage>!

A set of images that ARKit searches for in the user’s environment.

var maximumNumberOfTrackedImages: Int

The number of image anchors to monitor closely for position and orientation updates.

var automaticImageScaleEstimationEnabled: Bool

A flag that instructs the framework to estimate and set the scale of a detected or tracked image on your behalf.

### Detecting Real-World Objects

var detectionObjects: Set&lt;ARReferenceObject>

A set of 3D objects that the framework attempts to detect in the user’s environment.

### Creating Realistic Reflections

var environmentTexturing: ARWorldTrackingConfiguration.EnvironmentTexturing

An option that determines how the framework generates environment textures.

enum EnvironmentTexturing

The available environment texturing options for world tracking.

class AREnvironmentProbeAnchor

An object that provides environmental lighting information for a specific area of space in a world-tracking AR session.

var wantsHDREnvironmentTextures: Bool

A flag that instructs the framework to create environment textures in HDR format.

### Accessing App Clip Codes

Interacting with App Clip Codes in AR

Display content and provide services in an AR experience with App Clip Codes.

class var supportsAppClipCodeTracking: Bool

A flag that indicates if the device tracks App Clip Codes.

var appClipCodeTrackingEnabled: Bool

A Boolean value that indicates if the framework searches the physical environment for App Clip Codes.

class ARAppClipCodeAnchor

An anchor that tracks the position and orientation of an App Clip Code in the physical environment.

## Relationships

### Inherits From

- ARConfiguration

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Spatial Tracking

Understanding World Tracking

Discover features and best practices for building rear-camera AR experiences.

class ARWorldTrackingConfiguration

A configuration that tracks the position of a device in relation to objects in the environment.

class AROrientationTrackingConfiguration

A configuration that tracks only the device’s orientation using the rear-facing camera.

class ARPositionalTrackingConfiguration

A configuration that tracks only the device’s position in 3D space.

