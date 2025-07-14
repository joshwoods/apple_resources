

- Safari Services
- SFSafariViewController
- SFSafariViewController.Configuration
-  entersReaderIfAvailable 

Instance Property

# entersReaderIfAvailable

A value that specifies whether Safari should enter Reader mode, if it is available.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var entersReaderIfAvailable: Bool { get set }
```

## Discussion

Set the value to true if Reader mode should be entered automatically when it is available for the webpage; otherwise, false. The default value is false. Set this configuration property instead of initializing a view controller with init(url:entersReaderIfAvailable:).

## See Also

### Configuring a Safari View Controller

var barCollapsingEnabled: Bool

var eventAttribution: UIEventAttribution?

An object you use to send tap event attribution data to the browser for Private Click Measurement.

