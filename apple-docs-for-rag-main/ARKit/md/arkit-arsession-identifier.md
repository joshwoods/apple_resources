

- ARKit
- ARSession
-  identifier 

Instance Property

# identifier

A unique identifier of the running session.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var identifier: UUID { get }
```

## Discussion

This property might change after you call the run function, but not immediately. Therefore, to get the new value, listen for its change using key-value observation.

```
// Use key-value observation to monitor my ARSession's identifier.
var sessionIDObservation: NSKeyValueObservation?
...
sessionIDObservation = observe(
    .arView.session.identifier,
    options: [.old, .new]) { 
        object, change in
        print("SessionID changed to: \(change.newValue!)")
    }
```

## See Also

### Configuring and running a session

func run(ARConfiguration, options: ARSession.RunOptions)

Starts AR processing for the session with the specified configuration and options.

struct RunOptions

Options for transitioning an AR session’s current state when you change its configuration.

var configuration: ARConfiguration?

An object that defines motion and scene tracking behaviors for the session.

func pause()

Pauses processing in the session.

