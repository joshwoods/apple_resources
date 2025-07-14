

- WatchKit
- WKExtension
-  visibleInterfaceController 

Instance Property

# visibleInterfaceController

Returns the last visible interface controller.

watchOS 4.0+

``` source
@MainActor
var visibleInterfaceController: WKInterfaceController? { get }
```

## Discussion

Use this property to determine which interface controller is currently displayed by the app. For example, in the extension delegate’s handle(_:) method for a snapshot request, use this property to determine the user interface’s current contents, and make any changes before the snapshot is taken.

Or, when the app is launched due to a Handoff activity, use the handleUserActivity(_:) method’s `userInfo` dictionary to determine what to display. Then use the visibleInterfaceController property to determine whether to push or pop to a different interface controller.

This property contains the following values based on the app’s current state:

Just launched  
The app’s rootInterfaceController.

Running in the foreground  
The currently presented interface controller.

Running in the background  
The last interface controller presented by the app.

## See Also

### Getting the interface controllers

var rootInterfaceController: WKInterfaceController?

The app’s root interface controller.

