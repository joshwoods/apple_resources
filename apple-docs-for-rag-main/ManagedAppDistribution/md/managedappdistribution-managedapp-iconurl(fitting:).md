

- ManagedAppDistribution
- ManagedApp
-  iconURL(fitting:) 

Instance Method

# iconURL(fitting:)

A URL for the icon of the app.

iOS 17.2+iPadOS 17.2+visionOS 2.4+

``` source
func iconURL(fitting size: CGSize) -> URL?
```

## Parameters 

`size`  

The size of the icon.

## Return Value

The URL of the icon.

## Discussion

The icon scales to fit the given size.

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

func screenshotURLs(fitting: CGSize) -> [URL]

An array of the app’s screenshot URLs.

