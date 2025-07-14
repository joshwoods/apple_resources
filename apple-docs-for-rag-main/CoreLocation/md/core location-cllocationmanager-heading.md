

- Core Location
- CLLocationManager
-  heading 

Instance Property

# heading

The most recently reported heading.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.15+watchOS 2.0+

``` source
@NSCopying
var heading: CLHeading? { get }
```

## Discussion

The value of this property is `nil` if heading updates have never been initiated.

## See Also

### Getting recent location and heading data

var location: CLLocation?

The most recently retrieved user location.

