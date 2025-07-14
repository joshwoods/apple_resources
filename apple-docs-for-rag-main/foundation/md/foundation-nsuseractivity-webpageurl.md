

- Foundation
- NSUserActivity
-  webpageURL 

Instance Property

# webpageURL

The URL of the webpage to load in a browser to continue the activity.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var webpageURL: URL? { get set }
```

## Mentioned in 

Creating a user activity object

## Discussion

When no suitable app is installed on a resuming device and the webpageURL property is set, the specified webpage is loaded and the user activity is continued in a web browser.

If your activity’s content can be restored on the web or you support Safari universal links, be sure to set this property so that the system can resume the activity in Safari or your app. After setting the webpageURL property on an activity for which isEligibleForSearch is true, also set the requiredUserInfoKeys property, using the keys of the userInfo dictionary that must be stored. If you don’t also set the requiredUserInfoKeys property, the userInfo dictionary will be empty when the activity is restored.

If isEligibleForSearch is true for this activity and you’re using both NSUserActivity and web markup to index the same item, set webpageURL to the relevant URL on your website to avoid showing duplicate results in Spotlight. The NSUserActivity API does not perform any modifications to the URL that you specify. URL components, such as the query string and the fragment identifier, are used for matching the item against pages that are indexed by Applebot.

Note

The scheme of the webpageURL must be `http` or `https`. Any other scheme throws an exception.

## See Also

### Continuing web browsing

var referrerURL: URL?

The URL of the webpage that linked to the webpage URL.

