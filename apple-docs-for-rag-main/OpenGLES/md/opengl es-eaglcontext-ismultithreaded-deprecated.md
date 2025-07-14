

- OpenGL ES
- EAGLContext
-  isMultiThreaded Deprecated

Instance Property

# isMultiThreaded

A Boolean value that determines whether OpenGL ES defers work to another thread.

iOS 7.1–12.0DeprecatediPadOS 7.1–12.0DeprecatedMac Catalyst 7.1–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
var isMultiThreaded: Bool { get set }
```

## Discussion

Set the value of this property to true to enable multithreading in OpenGL ES. A multithreaded OpenGL ES context automatically creates a worker thread and transfers some of its calculations to that thread. When you enable multithreading on a multicore device, internal OpenGL ES calculations performed on the CPU act in parallel with your app, improving performance.

When the value of this property is false (the default), OpenGL ES performs any CPU-based calculations for a command on the thread it was called from.

If the current device does not support multithreaded OpenGL ES, the value of this property is always false—attempting to set the value to true has no effect.

Note

Enabling multithreading has both costs and benefits to performance—you should choose a concurrency strategy that provides the most benefit to your app. For details, see Concurrency and OpenGL ES in OpenGL ES Programming Guide.

