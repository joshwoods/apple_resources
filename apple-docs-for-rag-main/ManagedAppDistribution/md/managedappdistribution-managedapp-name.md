

- ManagedAppDistribution
- ManagedApp
-  name 

Instance Property

# name

The app’s localized name.

iOS 17.2+iPadOS 17.2+visionOS 2.4+

``` source
let name: String
```

## See Also

### Obtaining general information

let subtitle: String?

The app’s localized subtitle.

let description: String?

The app’s localized description.

let fileSize: Measurement&lt;UnitInformationStorage>?

The size of the app in bytes.

func iconURL(fitting: CGSize) -> URL?

A URL for the icon of the app.

func screenshotURLs(fitting: CGSize) -> [URL]

An array of the app’s screenshot URLs.

