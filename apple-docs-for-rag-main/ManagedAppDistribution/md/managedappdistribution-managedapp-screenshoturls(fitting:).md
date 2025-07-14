

- ManagedAppDistribution
- ManagedApp
-  screenshotURLs(fitting:) 

Instance Method

# screenshotURLs(fitting:)

An array of the app’s screenshot URLs.

iOS 17.2+iPadOS 17.2+visionOS 2.4+

``` source
func screenshotURLs(fitting size: CGSize) -> [URL]
```

## Parameters 

`size`  

The size of the screenshots.

## Return Value

The URLs of the screenshots.

## Discussion

The screenshots scale to fit the given size.

## See Also

### Obtaining general information

let name: String

The app’s localized name.

let subtitle: String?

The app’s localized subtitle.

let description: String?

The app’s localized description.

let fileSize: Measurement&lt;UnitInformationStorage>?

The size of the app in bytes.

func iconURL(fitting: CGSize) -> URL?

A URL for the icon of the app.

