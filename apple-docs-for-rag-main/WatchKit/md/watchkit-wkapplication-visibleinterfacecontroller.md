

- WatchKit
- WKApplication
-  visibleInterfaceController 

Instance Property

# visibleInterfaceController

Returns the last visible interface controller.

watchOS 7.0+

``` source
@MainActor
var visibleInterfaceController: WKInterfaceController? { get }
```

## Discussion

Use this property to determine which interface controller the app is currently displaying. For example, in the app delegate’s handle(_:) method for a snapshot request, use this property to determine the user interface’s current contents, and make any changes before the system takes the snapshot.

Or, when a Handoff activity launches the app, use the handleActiveWorkoutRecovery() method’s `userInfo` dictionary to determine what to display. Then use the visibleInterfaceController property to determine whether to push or pop to a different interface controller.

This property contains the following values based on the app’s current state:

Just launched  
The app’s rootInterfaceController.

Running in the foreground  
The currently presented interface controller.

Running in the background  
The last interface controller presented by the app.

## See Also

### Getting the interface controller

var rootInterfaceController: WKInterfaceController?

The app’s root interface controller.

