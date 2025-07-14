

- Core Location
-  CLDeviceOrientation 

Enumeration

# CLDeviceOrientation

Constants indicating the physical orientation of the device.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum CLDeviceOrientation
```

## Topics

### Device Orientations

case unknown

The orientation is currently not known.

case portrait

The device is in portrait mode, with the device held upright and the home button at the bottom.

case portraitUpsideDown

The device is in portrait mode but upside down, with the device held upright and the home button at the top.

case landscapeLeft

The device is in landscape mode, with the device held upright and the home button on the right side.

case landscapeRight

The device is in landscape mode, with the device held upright and the home button on the left side.

case faceUp

The device is held parallel to the ground with the screen facing upwards.

case faceDown

The device is held parallel to the ground with the screen facing downwards.

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

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

