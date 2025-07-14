

- Swift
- Optional
-  unsafelyUnwrapped 

Instance Property

# unsafelyUnwrapped

The wrapped value of this instance, unwrapped without checking whether the instance is `nil`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var unsafelyUnwrapped: Wrapped { get }
```

## Discussion

The `unsafelyUnwrapped` property provides the same value as the forced unwrap operator (postfix `!`). However, in optimized builds (`-O`), no check is performed to ensure that the current instance actually has a value. Accessing this property in the case of a `nil` value is a serious programming error and could lead to undefined behavior or a runtime error.

In debug builds (`-Onone`), the `unsafelyUnwrapped` property has the same behavior as using the postfix `!` operator and triggers a runtime error if the instance is `nil`.

The `unsafelyUnwrapped` property is recommended over calling the `unsafeBitCast(_:)` function because the property is more restrictive and because accessing the property still performs checking in debug builds.

Warning

This property trades safety for performance. Use `unsafelyUnwrapped` only when you are confident that this instance will never be equal to `nil` and only after you’ve tried using the postfix `!` operator.

## See Also

### Inspecting an Optional

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var debugDescription: String

A textual representation of this instance, suitable for debugging.

var customMirror: Mirror

The custom mirror for this instance.

