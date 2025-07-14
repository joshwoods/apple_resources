

- App Clips
- APActivationPayload
-  url 

Instance Property

# url

The URL of the link that launched the App Clip.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var url: URL? { get }
```

## Discussion

Use `url` to retrieve data that’s passed to an App Clip on launch, and use the data to update the user interface of the App Clip.

The value of `url` is the same as the NSUserActivity webpageURL property. If you don’t need to verify the user’s location when they launch your App Clip, use `webpageURL` instead.

For more information, see Responding to invocations.

