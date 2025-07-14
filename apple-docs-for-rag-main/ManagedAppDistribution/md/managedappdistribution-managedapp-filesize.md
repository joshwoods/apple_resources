

- ManagedAppDistribution
- ManagedApp
-  fileSize 

Instance Property

# fileSize

The size of the app in bytes.

iOS 17.2+iPadOS 17.2+visionOS 2.4+

``` source
let fileSize: Measurement?
```

## See Also

### Obtaining general information

let name: String

The app’s localized name.

let subtitle: String?

The app’s localized subtitle.

let description: String?

The app’s localized description.

func iconURL(fitting: CGSize) -> URL?

A URL for the icon of the app.

func screenshotURLs(fitting: CGSize) -> [URL]

An array of the app’s screenshot URLs.

