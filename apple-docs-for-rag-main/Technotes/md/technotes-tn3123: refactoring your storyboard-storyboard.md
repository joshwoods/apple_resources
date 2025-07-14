

- Technotes
-  TN3123: Refactoring your storyboard 

Article

# TN3123: Refactoring your storyboard

Learn strategies and techniques for refactoring a single storyboard into multiple storyboards.

## Overview

A storyboard is used to graphically lay out your app’s user interface. You use Xcode’s Interface Builder to specify your interface using scenes, segues between scenes, and controls used to trigger the segues. At design time, you configure the content of your view controllers visually, and Xcode saves the data needed to recreate that interface in a storyboard file in your app’s bundle.

Over time, as your application’s UI evolves into a larger set of view controller scenes, it may become a challenge to manage and maintain that storyboard. This can be a further challenge when you need to design it with multiple team members. Two team members modifying the same storyboard could potentially cause source control problems. Improve the storyboard management process by separating your single storyboard file into individual storyboards. Storyboards are connected together using storyboard references.

## Benefits of using multiple storyboards

When a storyboard is refactored, you gain three benefits:

1.  Improved readability - View controller connections become more explicit and the segue connections are easier to trace.

2.  Reuse - A separate storyboard containing a view controller scene can be referenced and re-used in multiple parts of the app.

3.  Easier to manage - A large team may work more efficiently when each member manages their own UI. Dividing your storyboard can help avoid merge conflicts when you use a source code version control system like Git.

## Connect two storyboards using a storyboard reference

A view controller is connected to another by using a segue and a storyboard reference. This involves three stages.

1.  Create a separate storyboard containing an individual view controller and give that view controller a unique identifier.

2.  Back in the app’s Main storyboard, create a storyboard reference and set its storyboard and identifier created in step 1.

3.  Create a segue from the source view controller and connect it to the storyboard reference.

## Automatically refactor a storyboard using Xcode

For some UI elements Xcode helps refactor a single storyboard into multiple storyboards automatically.

To separate out a UITabBarController in iOS:

1.  Open the storyboard.

2.  Select the `UITabBarController` scene.

3.  Select Menu: Editor \> Refactor to Storyboard…

4.  Name and save the new storyboard file to your project.

The new storyboard file will contain the `UITabBarController`. The child view controllers are separated and linked through storyboard references using unique identifiers. Storyboard references link one storyboard to another.

To separate out a NSTabViewController in macOS:

1.  Open the storyboard.

2.  Select the `NSTabViewController` scene.

3.  Select Menu: Editor \> Refactor to Storyboard…

4.  Name and save the new storyboard file to your project.

The new storyboard file will contain the `NSTabViewController`. The child view controllers are separated and linked through storyboard references using unique identifiers.

## Manually refactor a storyboard

If you choose to refactor your storyboard yourself, for example if one UIViewController (VC1) presents another (VC2), do the following:

1.  Open the app’s Main storyboard file.

2.  Select the view controller scene you want to present, and copy it.

3.  Create new storyboard file: File \> New \> File… - choose Storyboard, name and save it “VC2”.

4.  With the VC2 storyboard open, paste the copied view controller.

5.  Select the copied view controller and select its Identify Inspector.

6.  Name its Storyboard ID as “VC2_identifier”.

7.  Go back to the Main storyboard.

8.  Remove the view controller scene you previously copied.

9.  Select Menu \> Show Library

10. Drag and drop a new Storyboard Reference from the Library window into the Main storyboard.

11. Select the dropped Storyboard Reference and select its Attributes Inspector.

12. Set the Storyboard to “VC2”.

13. Set the Referenced ID “VC2_identifier”.

14. Connect this Storyboard Reference via segue from VC1.

## Load storyboards programmatically

Segues connecting two view controller scenes within the same storyboard load the view controller automatically. When a single storyboard is refactored into separate storyboards, storyboard references load them automatically as well. You can, however, load view controller scenes manually using code. You use *storyboard instances* to do that. Storyboard instances come in two flavors: NSStoryboard for macOS, and UIStoryboard for iOS. These APIs on both platforms are similar.

## Load and open an NSWindowController programmatically with macOS

In macOS, an NSViewController is loaded separately, or through its NSWindowController.

```
let storyboard = NSStoryboard(name: "InspectorWindow", bundle: Bundle.main)
if let windController = storyboard.instantiateInitialController() as? NSWindowController {
    windController.window!.makeKeyAndOrderFront(self)
}
```

The window controller inside the “InspectorWindow” storyboard is to be set at the initial controller via “Is Initial Controller”.

## Load and present a UIViewController programmatically with iOS

Load by identifier:

```
let mainStoryboard: UIStoryboard = UIStoryboard(name: "DetailViewController", bundle: nil)
let viewController = mainStoryboard.instantiateViewController(withIdentifier: "DetailViewControllerID") as! UIViewController
self.present(viewController, animated: true, completion: nil)
```

Load by initial view controller:

```
let mainStoryboard: UIStoryboard = UIStoryboard(name: "DetailViewController", bundle: nil)
if let viewController = mainStoryboard.instantiateInitialViewController() {
    present(viewController, animated: true, completion: nil)
}
```

The view controller inside the “DetailViewControler” storyboard is to be set at the initial controller via “Is Initial Controller”.

## Load and present a UIViewController programmatically with SwiftUI

If you are developing a SwiftUI app, and you want to integrate an existing `UIViewController` subclass and its storyboard:

```
struct DetailView: View {
    var body: some View {
        DetailViewControllerRepresentable()
    }
}

final class DetailViewControllerRepresentable: UIViewControllerRepresentable {
    typealias UIViewControllerType = DetailViewController

    func makeUIViewController(context: Context) -> DetailViewController {
        let storyboard = UIStoryboard(name: "DetailViewController", bundle: nil)
        return storyboard.instantiateInitialViewController() as! DetailViewController
    }

    func updateUIViewController(_ uiViewController: DetailViewController, context: Context) { }
    func makeCoordinator() -> Coordinator { Coordinator(self) }

    class Coordinator: NSObject {
        private let parent: DetailViewControllerRepresentable
        init(_ parent: DetailViewControllerRepresentable) {
            self.parent = parent
        }
    }
}

class DetailViewController: UIViewController { }
```

## Revision History

- **2022-03-29** First published.

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

