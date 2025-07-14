

- UIKit
- UIApplication
-  setAlternateIconName(\_:completionHandler:) 

Instance Method

# setAlternateIconName(\_:completionHandler:)

Changes the icon the system displays for the app.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+tvOS 10.2+visionOS 1.0+

``` source
@MainActor
func setAlternateIconName(
    _ alternateIconName: String?,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
@MainActor
func setAlternateIconName(_ alternateIconName: String?) async throws
```

## Parameters 

`alternateIconName`  

The name of the alternate icon, as declared in the `CFBundleAlternateIcons` key of your app’s `Info.plist` file. Specify `nil` if you want to display the app’s primary icon, which you declare using the `CFBundlePrimaryIcon` key. Both keys are subentries of the `CFBundleIcons` key in your app’s `Info.plist` file.

`completionHandler`  

The handler to execute with the results. After attempting to change your app’s icon, the system reports the results by calling your handler. The handler executes on a UIKit-provided queue, and not necessarily on your app’s main queue. The handler has no return value and takes the following parameter:

error  
On success, the value of this parameter is `nil`. If an error occurred, this parameter contains the error object indicating what happened and the value of the alternateIconName property remains unchanged.

## Discussion

Use this method to change your app’s icon to its primary icon or to one of its alternate icons. You can change the icon only if the value of the supportsAlternateIcons property is true.

You must configure your app’s primary icon asset in the “App Icons and Launch Images” section of the General pane or set it directly using the “Primary App Icon Set Name” build setting. You specify the names of additional icon assets available to your app using the “Alternate App Icon Sets” build setting. Xcode uses these setting to generate the entries for CFBundlePrimaryIcon and CFBundleAlternateIcons under the top-level key CFBundleIcons. For more information, see Build settings reference and Configuring your app icon.

Note

This method still sets the alternate icon in compatible iPad and iPhone apps running in visionOS. Support for alternate icons is unavailable in apps you build using the visionOS SDK, and calling this method has no effect.

## See Also

### Managing the app’s icon

var supportsAlternateIcons: Bool

A Boolean value that indicates whether the app is allowed to change its icon.

var alternateIconName: String?

The name of the icon the system displays for the app.

