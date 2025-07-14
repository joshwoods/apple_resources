

- UIKit
- UIScene
- UIScene.ConnectionOptions
-  userActivities 

Instance Property

# userActivities

Information about user activities that you can use to configure your scene’s interface.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var userActivities: Set { get }
```

## Discussion

If this property contains one or more NSUserActivity objects, use those objects to configure your scene’s interface when the scene connects. These activity objects represent the user activities that are available at the time the scene connects, like from search results, other apps, or requestSceneSessionActivation(_:userActivity:options:errorHandler:). For example, if the user was browsing a web page, an activity object might contain the URL of that page.

This property doesn’t contain user activity objects related to Handoff. At connection time, UIKit delivers only the type of a Handoff interaction in the handoffUserActivityType property. Later, it calls additional methods of UISceneDelegate to deliver the NSUserActivity object itself.

