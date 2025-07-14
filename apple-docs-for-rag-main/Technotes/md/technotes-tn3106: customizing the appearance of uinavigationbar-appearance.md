

- Technotes
-  TN3106: Customizing the appearance of UINavigationBar 

Article

# TN3106: Customizing the appearance of UINavigationBar

Adopt UINavigationBarAppearance for a navigation bar background color that’s consistent on iOS 13 and later.

## Overview

UINavigationBar in iOS 15 introduces changes to its appearance settings. It extends the usage of its scrollEdgeAppearance, which by default produces a transparent background, to all navigation bar styles.

The iOS 13 SDK introduced an appearance settings class UINavigationBarAppearance. If you’re seeing a view controller with appearance issues like a black navigation bar or incorrect status bar content color when building with Xcode 13 and running on iOS 15, adopt `UINavigationBarAppearance`. For a view controller that scrolls its content, use it to apply both `standardAppearance` and `scrollEdgeAppearance` to the `UINavigationBar`.

## Configure the UINavigationBarAppearance

Consider an app that uses `UITableViewController`, and has the following code in `application(_ :didFinishLaunchingWithOptions:)`:

```
UINavigationBar.appearance().isTranslucent = false
UINavigationBar.appearance().barTintColor = .systemRed
```

In iOS 14.x or later, the navigation bar color turns transparent (showing the black background underneath), yet iOS 13 draws the navigation bar in `.systemRed`.

To standardize the navigation bar’s appearance between these versions of iOS, use the `UINavigationBarAppearance` API. Use the following example to apply an opaque navigation bar colored `.systemRed` with white title text. Setting the text color here is only an example and of course is optional.

```
@available(iOS 13.0, *)
func customNavBarAppearance() -> UINavigationBarAppearance {
    let customNavBarAppearance = UINavigationBarAppearance()

    // Apply a red background.
    customNavBarAppearance.configureWithOpaqueBackground()
    customNavBarAppearance.backgroundColor = .systemRed

    // Apply white colored normal and large titles.
    customNavBarAppearance.titleTextAttributes = [.foregroundColor: UIColor.white]
    customNavBarAppearance.largeTitleTextAttributes = [.foregroundColor: UIColor.white]

    // Apply white color to all the nav bar buttons.
    let barButtonItemAppearance = UIBarButtonItemAppearance(style: .plain)
    barButtonItemAppearance.normal.titleTextAttributes = [.foregroundColor: UIColor.white]
    barButtonItemAppearance.disabled.titleTextAttributes = [.foregroundColor: UIColor.lightText]
    barButtonItemAppearance.highlighted.titleTextAttributes = [.foregroundColor: UIColor.label]
    barButtonItemAppearance.focused.titleTextAttributes = [.foregroundColor: UIColor.white]
    customNavBarAppearance.buttonAppearance = barButtonItemAppearance
    customNavBarAppearance.backButtonAppearance = barButtonItemAppearance
    customNavBarAppearance.doneButtonAppearance = barButtonItemAppearance

    return customNavBarAppearance
}
```

## Configure the entire app

To apply this appearance to the navigation bar throughout the entire app:

```
func application(_ application: UIApplication, didFinishLaunchingWithOptions launchOptions: [UIApplication.LaunchOptionsKey: Any]?) -> Bool {
    let newNavBarAppearance = customNavBarAppearance()

    let appearance = UINavigationBar.appearance()
    appearance.scrollEdgeAppearance = newNavBarAppearance
    appearance.compactAppearance = newNavBarAppearance
    appearance.standardAppearance = newNavBarAppearance
    if #available(iOS 15.0, *) {
        appearance.compactScrollEdgeAppearance = newNavBarAppearance
    }

    return true
}
```

## Configure a view controller

To apply this appearance to the navigation bar of an individual view controller:

```
override func viewDidLoad() {
    super.viewDidLoad()

    let newNavBarAppearance = customNavBarAppearance()
    navigationController!.navigationBar.scrollEdgeAppearance = newNavBarAppearance
    navigationController!.navigationBar.compactAppearance = newNavBarAppearance
    navigationController!.navigationBar.standardAppearance = newNavBarAppearance
    if #available(iOS 15.0, *) {
        navigationController!.navigationBar.compactScrollEdgeAppearance = newNavBarAppearance
    }
}
```

If you’re using storyboards, instead configure both the appearance of the navigation bar and the elements within that bar.

To change the appearance of the navigation bar:

Choose “standard” and “scroll edge appearances” for the navigation bar, by setting the appearance proxy of `UINavigationBar`: “Standard”, and “ScrollEdge” appearances.

1.  Open the project’s storyboard file.

2.  Select the `UINavigationBar` from your `UINavigationController` scene.

3.  In the Attributes Inspector pane turn on these Appearances: “Standard”, “Compact”, “Scroll Edge”, and “Compact Scroll Edge”.

4.  For all four appearances, set the “Background” to “System Red Color”, for example.

Change the color of the title and button elements:

1.  Change the bar button items color: set the View’s “Tint” color to “White Color”.

2.  Change the Standard Text Attributes “Title” from “Inherited” to “Custom”.

3.  Change the Standard Title Attributes “Title Color” from “Default” to “White Color”. Repeat steps 2 and 3 for: Scroll Edge and Compact Scroll Edge appearances.

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

