

- Core Location
- CLHeading
-  z 

Instance Property

# z

The geomagnetic data (measured in microteslas) for the z-axis.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.7+watchOS 2.0+

``` source
var z: CLHeadingComponentValue { get }
```

## Discussion

This value represents the z-axis deviation from the magnetic field lines being tracked by the device.

## See Also

### Getting the raw heading data

var x: CLHeadingComponentValue

The geomagnetic data (measured in microteslas) for the x-axis.

var y: CLHeadingComponentValue

The geomagnetic data (measured in microteslas) for the y-axis.

typealias CLHeadingComponentValue

A type used to report magnetic differences reported by the onboard hardware.

