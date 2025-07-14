

- Group Activities
- GroupActivityMetadata
-  fallbackURL 

Instance Property

# fallbackURL

A URL that offers participants a way to identify or join the activity from a web browser.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var fallbackURL: URL?
```

## Mentioned in 

Defining your app’s SharePlay activities

## Discussion

Use this property to provide fallback behavior for users who don’t have your app installed on their device. For example, if your app runs only on iOS, use this property to supply activity-related information for users on a Mac. When your app isn’t available, the system opens the specified URL in Safari.

Important

Make sure that the URL in this property eventually leads to a webpage with the same content as the activity. Safari automatically synchronizes media playback for listen-together and watch-together experiences.

## See Also

### Presenting the activity

var title: String?

The localized string to display as the title of your activity.

var subtitle: String?

The localized string that provides additional information about the activity.

var previewImage: CGImage?

The image to display for the current activity.

