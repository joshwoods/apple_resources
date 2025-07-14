

- UIKit
- App and environment
- Scenes
- Preparing your UI to run in the background
-  About the background execution sequence 

Article

# About the background execution sequence

Learn the order in which your custom code is executed when your app moves to the background.

## Overview

An app may enter the background from one of several different starting points. System events can cause a suspended app to be returned to the background, or cause a not running app to be launched directly into the background. A foreground app transitions to the background when another app is launched or when the user returns to the Home screen.

### Handle background events

For apps that support one of the Background Modes capabilities, the system launches or resumes the app in the background to handle events associated with those capabilities. For example, the system might launch or resume the app to respond to a location update or to perform a background fetch.

If your app isn’t running when an event arrives, the system launches the app and moves it directly to the background, following this sequence:

1.  The system launches the app and follows the initialization sequence described in About the app launch sequence.

2.  UIKit calls the app delegate’s applicationDidEnterBackground(_:) method.

3.  UIKit delivers the event that caused the launch.

4.  The app’s snapshot is taken.

5.  The app may be suspended again.

If your app is in memory and suspended when an event arrives, the system resumes the app in the background, following this sequence:

1.  The system resumes the app.

2.  UIKit calls the app delegate’s applicationDidEnterBackground(_:) method.

3.  UIKit delivers the event that caused the launch.

4.  The app’s snapshot is taken.

5.  The app may be suspended again.

### Transition from the foreground

When another app is launched or the user returns to the Home screen, the foreground app moves to the background, following this sequence:

1.  The user exits the running app.

2.  UIKit calls the app delegate’s applicationWillResignActive(_:) method.

3.  UIKit calls the app delegate’s applicationDidEnterBackground(_:) method.

4.  The app’s snapshot is taken.

5.  The app may be suspended again.

## See Also

### Background execution

Using background tasks to update your app

Configure your app to perform tasks in the background to make efficient use of processing time and power.

Extending your app’s background execution time

Ensure that critical tasks finish when your app moves to the background.

