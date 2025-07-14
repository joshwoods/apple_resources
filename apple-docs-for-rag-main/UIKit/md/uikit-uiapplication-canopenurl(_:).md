

- UIKit
- UIApplication
-  canOpenURL(\_:) 

Instance Method

# canOpenURL(\_:)

Returns a Boolean value that indicates whether an app is available to handle a URL scheme.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
nonisolated
func canOpenURL(_ url: URL) -> Bool
```

## Parameters 

`url`  

A URL (Universal Resource Locator). At runtime, the system determines if the device has an installed app registered to handle the URL’s scheme. The device can have more than one app registered to handle a scheme.

The URL can have a common scheme such as `http`, `https`, `tel`, or `facetime`, or a custom scheme. For information about supported schemes, see Apple URL Scheme Reference.

## Return Value

false if the device doesn’t have an installed app registered to handle the URL’s scheme, or if you haven’t declared the URL’s scheme in your `Info.plist` file; otherwise, true.

## Discussion

When this method returns true, iOS guarantees subsequent calls to the open(_:options:completionHandler:) method with the same URL will successfully launch an app that can handle the URL. The return value doesn’t indicate the validity of the URL, whether the specified resource exists, or, in the case of a universal link, whether the device has an installed app registered to respond to the universal link.

You can call this method safely on a thread that isn’t the main thread.

Important

If you link your app on or after iOS 9.0, you must declare the URL schemes you pass to this method by adding the `LSApplicationQueriesSchemes` key to your app’s `Info.plist` file. This method always returns false for undeclared schemes, even if the device doesn’t have a registered app installed. Apps linked on or after iOS 15 are limited to a maximum of 50 entries in the `LSApplicationQueriesSchemes` key. To learn more about the key, see LSApplicationQueriesSchemes.

If you link your app against an earlier version of iOS but it is running in iOS 9.0 or later, you can call this method up to 50 times. After reaching that limit, subsequent calls always return false. If the user reinstalls or upgrades the app, iOS resets the limit.

Unlike this method, the open(_:options:completionHandler:) method isn’t constrained by the `LSApplicationQueriesSchemes` requirement. If an app is available to handle the URL, the system will launch it, even if you haven’t declared the scheme.

Using universal links instead of custom URL schemes removes the need to use this method to validate target links; if no app is available to handle a universal link, iOS routes it to the person’s default browser, allowing the associated website to respond. For more information on universal links, see Allowing apps and websites to link to your content.

## See Also

### Related Documentation

func openURL(URL) -> Bool

Attempts to open the resource at the specified URL.

Deprecated

### Opening a URL resource

func open(URL, options: [UIApplication.OpenExternalURLOptionsKey : Any], completionHandler: ((Bool) -> Void)?)

Attempts to asynchronously open the resource at the specified URL.

struct OpenExternalURLOptionsKey

Options for opening a URL.

