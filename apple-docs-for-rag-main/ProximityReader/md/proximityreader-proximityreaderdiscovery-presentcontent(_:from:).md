

- ProximityReader
- ProximityReaderDiscovery
-  presentContent(\_:from:) 

Instance Method

# presentContent(\_:from:)

Presents a sheet that teaches merchants how to use the specified feature.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
final func presentContent(
    _ content: ProximityReaderDiscovery.Content,
    from viewController: UIViewController
) async throws
```

## Parameters 

`content`  

The topic to teach. You can get a list of available topics from the contentList property or fetch a topic for a specific subject using the content(for:) method.

`viewController`  

The view controller to use when presenting the sheet. Specify a currently visible view controller in your app.

## Discussion

Throws

This method throws a ProximityReaderDiscovery.ContentError if the sheet fails to appear.

Call this method when you want to display information about how to use ProximityReader features on a merchant’s iPhone. For example, you might use this method to display instructions for how the merchant uses Tap to Pay on iPhone. This method presents the requested information in a sheet on top of your app’s UI, which remains on-screen until the person dismiss it or an error occurs.

