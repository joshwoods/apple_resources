

- UIKit
- UIApplicationDelegate
-  application(\_:open:options:) 

Instance Method

# application(\_:open:options:)

Asks the delegate to open a resource specified by a URL, and provides a dictionary of launch options.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func application(
    _ app: UIApplication,
    open url: URL,
    options: [UIApplication.OpenURLOptionsKey : Any] = [:]
) -> Bool
```

## Parameters 

`app`  

Your singleton app object.

`url`  

The URL resource to open. This resource can be a network resource or a file. For information about the Apple-registered URL schemes, see Apple URL Scheme Reference.

`options`  

A dictionary of URL handling options. For information about the possible keys in this dictionary and how to handle them, see `UIApplicationOpenURLOptionsKey`. By default, the value of this parameter is an empty dictionary.

## Return Value

true if the delegate successfully handled the request or false if the attempt to open the URL resource failed.

## Mentioned in 

Enabling document sharing

## Discussion

This method is not called if your implementations return false from both the application(_:willFinishLaunchingWithOptions:) and application(_:didFinishLaunchingWithOptions:) methods. (If only one of the two methods is implemented, its return value determines whether this method is called.) If your app implements the applicationDidFinishLaunching(_:) method instead of application(_:didFinishLaunchingWithOptions:), this method is called to open the specified URL after the app has been initialized.

If a URL arrives while your app is suspended or running in the background, the system moves your app to the foreground prior to calling this method.

There is no equivalent notification for this delegation method.

## See Also

### Opening a URL-specified resource

struct OpenURLOptionsKey

Keys you use to access values in the options dictionary when opening a URL.

