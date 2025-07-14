

- RealityKit
- RealityViewAttachmentBuilderContent
-  onOpenURL(perform:) 

Instance Method

# onOpenURL(perform:)

Registers a handler to invoke in response to a URL that your app receives.

RealityKitSwiftUIiOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
nonisolated
func onOpenURL(perform action: @escaping (URL) -> ()) -> some View
```

## Parameters 

`action`  

A closure that SwiftUI calls when your app receives a Universal Link or a custom URL. The closure takes the URL as an input parameter.

## Return Value

A view that handles incoming URLs.

## Discussion

Use this view modifier to receive URLs in a particular scene within your app. The scene that SwiftUI routes the incoming URL to depends on the structure of your app, what scenes are active, and other configuration. For more information, see `Scene/handlesExternalEvents(matching:)`.

UI frameworks traditionally pass Universal Links to your app using an NSUserActivity. However, SwiftUI passes a Universal Link to your app directly as a URL, which you receive using this modifier. To receive other user activities, like when your app participates in Handoff, use the `View/onContinueUserActivity(_:perform:)` modifier instead.

For more information about linking into your app, see Allowing apps and websites to link to your content.

