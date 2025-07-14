

- AppKit
- NSApplication
-  delegate 

Instance Property

# delegate

The app delegate object.

macOS

``` source
@MainActor
weak var delegate: (any NSApplicationDelegate)? { get set }
```

## Discussion

The app object and app delegate work in tandem to manage the app’s overall behavior. Typically, the delegate is configured automatically by the Xcode project templates.

## See Also

### Managing the App’s Behavior

protocol NSApplicationDelegate

A set of methods that manage your app’s life cycle and its interaction with common system services.

