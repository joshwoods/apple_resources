

- UIKit
- UIApplicationDelegate
-  applicationDidFinishLaunching(\_:) Deprecated

Instance Method

# applicationDidFinishLaunching(\_:)

Tells the delegate when the app has finished launching.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func applicationDidFinishLaunching(_ application: UIApplication)
```

Deprecated

Use application(_:didFinishLaunchingWithOptions:) instead.

## Parameters 

`application`  

The singleton app object.

## Discussion

Don’t use this method in your apps; instead, use the application(_:willFinishLaunchingWithOptions:) and application(_:didFinishLaunchingWithOptions:) methods.

Your implementation of this method creates your app’s user interface and initializes the app’s data structures. If your app persists its state between launches, you would also use this method to restore your app to its previous state.

After calling this method, the app also posts a didFinishLaunchingNotification notification to give interested objects a chance to respond to the initialization cycle.

## See Also

### Deprecated

Deprecated symbols

Symbols that are no longer supported.

