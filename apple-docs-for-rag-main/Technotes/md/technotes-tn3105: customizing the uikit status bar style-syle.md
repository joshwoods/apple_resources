

- Technotes
-  TN3105: Customizing the UIKit status bar style 

Article

# TN3105: Customizing the UIKit status bar style

Configure the device’s status bar style to work well with your app’s user interface.

## Overview

Status bar content elements must be readable or visible to the user. Your app’s status bar style or UIStatusBarStyle should be set to a value that’s compatible with your app’s background color: lightContent or darkContent.

You control the `UIStatusBarStyle` at the app level or view controller level. At the app level choose a single `UIStatusBarStyle` that works well with its overall background color scheme. At the view controller level choose a `UIStatusBarStyle` that is most compatible with its specific background color.

If you find that your status bar elements aren’t visible, the problem might be that its background color is the same color as its content color (black elements on black background or white elements on white background). Users may also have a difficult time recognizing the status bar content when the background color is dark gray and its `UIStatusBarStyle` set to `darkContent`.

If you have a dark colored background, set the `UIStatusBarStyle` to `lightContent`. If you have a light colored background, set the `UIStatusBarStyle` to `darkContent`.

## Set a style for the entire app

For a single status bar style throughout your app, add UIViewControllerBasedStatusBarAppearance with a value of `false` to your `Info.plist`. Then add `UIStatusBarStyle` with the specific style. For example, to set a light content status bar, use the following:

```
UIStatusBarStyle
UIStatusBarStyleLightContent

UIViewControllerBasedStatusBarAppearance

```

## Set a style for each view controller

To allow individual view controllers to determine their status bar style, set `UIViewControllerBasedStatusBarAppearance` to `true`.

First, add the `UIViewControllerBasedStatusBarAppearance` property to the `Info.plist`:

```
UIViewControllerBasedStatusBarAppearance

```

Second, if your initial root view controller’s status bar style is light content, add the following to the `Info.plist`. This will make your initial view controller’s status bar style match up with the launch screen status bar style:

```
UIStatusBarStyle
UIStatusBarStyleLightContent
```

Third, override each view controller’s preferredStatusBarStyle() method. For example, to set the status bar’s content intended for use on dark backgrounds:

```

class ViewController: UIViewController {
   //..
    override var preferredStatusBarStyle: UIStatusBarStyle {
        return .lightContent
    }
    //..
}
```

If a particular view controller is embedded as a child or resides inside a UINavigationController stack, its parent or navigation controller determines the status bar style. If you want the containing view controller to give control of the status bar style to its children, override the childForStatusBarStyle property. For example:

```
class MyNavigationController: UINavigationController {
    // Return the visible child view controller which determines the status bar style.
    override var childForStatusBarStyle: UIViewController? { return visibleViewController }
}
```

For every `UINavigationController` defined in your storyboard that wants to give status bar style control over to its children, be sure to set its Custom Class name to match the `UINavigationController` subclass name on the Identity inspector.

It is not necessary to override the `childForStatusBarStyle` property when using UITabBarController. `UITabBarController` automatically forwards status bar style requests to its children.

When using this approach, any child view controller determines the status bar style that will match up with its color scheme or customization it uses with UINavigationBarAppearance. If you return `nil` or do not override this method, the status bar style for `self` is used. If the return value from this method changes, call the `setNeedsStatusBarAppearanceUpdate()` method.

## Revision History

- **2022-03-01** First published.

## See Also

### Latest

TN3182: Adding privacy tracking keys to your privacy manifest

Declare the tracking domains you use in your app or third-party SDK in a privacy manifest.

TN3183: Adding required reason API entries to your privacy manifest

Declare the APIs that can potentially fingerprint devices in your app or third-party SDK in a privacy manifest.

TN3184: Adding data collection details to your privacy manifest

Declare the data your app or third-party SDK collects in a privacy manifest.

TN3181: Debugging an invalid privacy manifest

Identify common configurations that cause unsuccessful privacy manifest validation with the App Store.

TN3180: Reverting to App Store Server Notifications V1

Migrate from version 2 to version 1 of App Store Server Notifications using the Modify an App endpoint.

TN3179: Understanding local network privacy

Learn how local network privacy affects your software.

TN3178: Checking for and resolving build UUID problems

Ensure that every Mach-O image has a UUID, and that every distinct Mach-O image has its own unique UUID.

TN3177: Understanding alternate audio track groups in movie files

Learn how alternate groups collect audio tracks, and how to choose which audio track to use in your app.

TN3111: iOS Wi-Fi API overview

Explore the various Wi-Fi APIs available on iOS and their expected use cases.

TN3176: Troubleshooting Apple Pay payment processing issues

Diagnose errors that occur when processing Apple Pay payments, identify common causes, and explore potential solutions.

TN3175: Diagnosing issues with displaying the Apple Pay button on your website

Diagnose common errors received while displaying the Apple Pay button on your website by identifying the underlying causes, and explore potential solutions.

TN3174: Diagnosing issues with the Apple Pay payment sheet on your website

Diagnose errors received while presenting the Apple Pay payment sheet on your website by identifying the underlying causes of common errors and explore their potential solutions.

TN3173: Troubleshooting issues with your Apple Pay merchant identifier configuration

Diagnose errors due to invalid Apple Pay merchant identifier configurations by identifying the underlying causes of common errors and explore their potential solutions.

TN3168: Making your App Clip available in the App Store

Learn how to configure your App Clip to prevent it from being unavailable in the App Store.

TN3124: Debugging coordinate space issues

Learn techniques to help debug any coordinate space issue.

