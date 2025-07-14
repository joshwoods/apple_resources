

- Swift
- Optional
-  hash(into:) 

Instance Method

# hash(into:)

Hashes the essential components of this value by feeding them into the given hasher.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func hash(into hasher: inout Hasher)
```

Available when `Wrapped` conforms to `Hashable`.

## Parameters 

`hasher`  

The hasher to use when combining the components of this instance.

## See Also

### Inspecting an Optional

var unsafelyUnwrapped: Wrapped

The wrapped value of this instance, unwrapped without checking whether the instance is `nil`.

var debugDescription: String

A textual representation of this instance, suitable for debugging.

var customMirror: Mirror

The custom mirror for this instance.

