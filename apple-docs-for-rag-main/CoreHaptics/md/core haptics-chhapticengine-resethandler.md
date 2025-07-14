

- Core Haptics
- CHHapticEngine
-  resetHandler 

Instance Property

# resetHandler

A block that the haptic engine calls after recovering from a haptic server error.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
var resetHandler: CHHapticEngine.ResetHandler { get set }
```

## Discussion

If the handler has to reset itself after a server failure, the system calls this block asynchronously. In this block, release all haptic pattern players and recreate them. The system preserves CHHapticPattern objects and CHHapticEngine properties across restarts. Consider trying to restart the engine inside the reset block.

- Swift
- Objective-C

```
self.hapticEngine.resetHandler = {
    print("Engine reset --> Restarting!")
    do {
        try self.hapticEngine.start()
    } catch {
        print("Failed to restart the engine: \(error)")
    }
}
```

```
self.hapticEngine.resetHandler = ^{ 
    NSLog(@"Engine reset --> Restarting!");
    [self.hapticEngine startAndReturnError:&error];
};
```

Callbacks to this block arrive on a non-main thread, so handle them in a thread-safe manner.

## See Also

### Handling Haptic Engine Resets

typealias ResetHandler

A typealias for the block that the haptic engine calls after being reset.

