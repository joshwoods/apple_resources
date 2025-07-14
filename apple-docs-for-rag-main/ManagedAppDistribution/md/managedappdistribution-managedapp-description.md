

- ManagedAppDistribution
- ManagedApp
-  description 

Instance Property

# description

The app’s localized description.

iOS 17.2+iPadOS 17.2+visionOS 2.4+

``` source
let description: String?
```

## See Also

### Obtaining general information

let name: String

The app’s localized name.

let subtitle: String?

The app’s localized subtitle.

let fileSize: Measurement&lt;UnitInformationStorage>?

The size of the app in bytes.

func iconURL(fitting: CGSize) -> URL?

A URL for the icon of the app.

func screenshotURLs(fitting: CGSize) -> [URL]

An array of the app’s screenshot URLs.

