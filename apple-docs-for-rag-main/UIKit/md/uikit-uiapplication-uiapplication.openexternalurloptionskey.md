

- UIKit
- UIApplication
-  UIApplication.OpenExternalURLOptionsKey 

Structure

# UIApplication.OpenExternalURLOptionsKey

Options for opening a URL.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
struct OpenExternalURLOptionsKey
```

## Topics

### URL options

static let universalLinksOnly: UIApplication.OpenExternalURLOptionsKey

URLs must be universal links and have an app configured to open them.

### Measuring ad taps

static let eventAttribution: UIApplication.OpenExternalURLOptionsKey

An object you use to send tap event attribution data to the browser for Private Click Measurement.

### Initializers

init(rawValue: String)

Creates a new instance with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Opening a URL resource

func open(URL, options: [UIApplication.OpenExternalURLOptionsKey : Any], completionHandler: ((Bool) -> Void)?)

Attempts to asynchronously open the resource at the specified URL.

func canOpenURL(URL) -> Bool

Returns a Boolean value that indicates whether an app is available to handle a URL scheme.

