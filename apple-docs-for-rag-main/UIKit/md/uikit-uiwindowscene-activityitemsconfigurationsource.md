

- UIKit
- UIWindowScene
-  activityItemsConfigurationSource 

Instance Property

# activityItemsConfigurationSource

An object that can provide shareable items for a scene.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
weak var activityItemsConfigurationSource: (any UIActivityItemsConfigurationProviding)? { get set }
```

## Discussion

When a user asks Siri to “share this” on iOS, or clicks an NSSharingServicePickerToolbarItem in the toolbar of an app built with Mac Catalyst, the system asks the current scene or view controller what to share. You can supply multiple representations of the current content, such as a file, image, and URL.

You can implement this property or provide configurations from view controllers with activityItemsConfiguration.

If you don’t provide a UIActivityItemsConfiguration in either of these ways, the system may fall back to sharing either the webpageURL of your app’s current user activity or a screenshot of the scene.

## See Also

### Sharing content

protocol UIActivityItemsConfigurationProviding

An interface that provides a source for shareable content to fulfill user requests to share current content.

