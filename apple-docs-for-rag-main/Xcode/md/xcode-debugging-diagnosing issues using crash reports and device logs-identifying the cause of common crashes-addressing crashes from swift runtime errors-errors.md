

- Xcode
- Debugging
- Diagnosing issues using crash reports and device logs
- Identifying the cause of common crashes
-  Addressing crashes from Swift runtime errors 

Article

# Addressing crashes from Swift runtime errors

Identify the signs of a Swift runtime error, and address the crashes runtime errors cause.

## Overview

Swift uses memory safety techniques to catch programming mistakes early. Optionals require you to think about how best to handle a `nil` value. Type safety prevents casting an object to a type that doesn’t match the object’s actual type.

If you use the `!` operator to force unwrap an optional value that’s `nil`, or if you force a type downcast that fails with the `as!` operator, the Swift runtime catches these errors and intentionally crashes the app. If you can reproduce the runtime error, Xcode logs information about the issue to the console. On ARM processors, the exception info in the crash report looks like:

```
Exception Type:  EXC_BREAKPOINT (SIGTRAP)
...
Termination Signal: Trace/BPT trap: 5
Termination Reason: Namespace SIGNAL, Code 0x5
```

On Intel processors (including apps for macOS, Mac Catalyst, and the simulators for iOS, iPadOS, tvOS, and watchOS), the exception info in the crash report looks like:

```
Exception Type:        EXC_BAD_INSTRUCTION (SIGILL)
...
Exception Note:        EXC_CORPSE_NOTIFY

Termination Signal:    Illegal instruction: 4
Termination Reason:    Namespace SIGNAL, Code 0x4
```

### Identify the location of the error

The crash report shows the thread that encountered the runtime error, with a frame in the backtrace identifying the specific line of code.

```
Thread 0 Crashed:
0   MyCoolApp                         0x0000000100a71a88 @objc ViewController.viewDidLoad() (in MyCoolApp) (ViewController.swift:18)
1   MyCoolApp                         0x0000000100a71a40 @objc ViewController.viewDidLoad() (in MyCoolApp) (ViewController.swift:18)
2   UIKitCore                         0x00000001c569e920 -[UIViewController _sendViewDidLoadWithAppearanceProxyObjectTaggingEnabled] + 100
3   UIKitCore                         0x00000001c56a3430 -[UIViewController loadViewIfRequired] + 936
4   UIKitCore                         0x00000001c56a3838 -[UIViewController view] + 28
```

In this example, thread 0 encountered the error. Frame 0 of this thread shows that the runtime error occurs on line 18 of `ViewController.swift`, in the `viewDidLoad` method:

```
0   MyCoolApp                         0x0000000100a71a88 @objc ViewController.viewDidLoad() (in MyCoolApp) (ViewController.swift:18)
```

### Change your code

Look at the other frames in the backtrace to identify the exact function calls that produced the error, and determine whether you used a force unwrap or a forced downcast. A force unwrap uses the `!` operator. For example:

```
let image = UIImage(named: "aMissingIcon")!
print("Image size: \(image.size)")
```

Instead of the force unwrap, gracefully handle the `nil` value where it first appears in your code by using optional binding:

```
if let image = UIImage(named: "aMissingIcon") {
    print("Image size: \(image.size)")
}
```

See the Swift documentation for more information on Optionals.

For type casts, a forced downcast uses the `as!` operator. This example crashes if `library` contains something other than a `Song` type:

```
for item in library {
    let song = item as! Song
    print("Song: \(song.name), by \(song.artist)")
}
```

Instead of the forced downcast, gracefully handle the scenarios where the type of the object doesn’t match the expected type by using a conditional downcast:

```
for item in library {
    if let song = item as? Song {
         print("Song: \(song.name), by \(song.artist)")
    }
}
```

See the Swift documentation for more information on Type Casting.

## See Also

### Related Documentation

Analyzing a crash report

Identify clues in a crash report that help you diagnose problems.

### Runtime errors

Addressing language exception crashes

Identify the signs of a language exception, and address the crashes caused by uncaught language exceptions.

Reading an exception message

Understand and address the common reasons apps crash.

