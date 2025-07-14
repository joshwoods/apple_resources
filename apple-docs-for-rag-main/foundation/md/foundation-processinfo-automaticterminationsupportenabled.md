

- Foundation
- ProcessInfo
-  automaticTerminationSupportEnabled 

Instance Property

# automaticTerminationSupportEnabled

A Boolean value indicating whether the app supports automatic termination.

macOS 10.7+

``` source
var automaticTerminationSupportEnabled: Bool { get set }
```

## Discussion

Without setting this property or setting the equivalent `Info.plist` key (`NSSupportsAutomaticTermination`), the methods disableAutomaticTermination(_:) and enableAutomaticTermination(_:) have no effect, although the counter tracking automatic termination opt-outs is still kept up to date to ensure correctness if this is called later. Currently, setting this property to false has no effect. This property should be set in the app delegate method applicationDidFinishLaunching(_:) or earlier.

## See Also

### Controlling Automatic Termination

func disableAutomaticTermination(String)

Disables automatic termination for the application.

func enableAutomaticTermination(String)

Enables automatic termination for the application.

