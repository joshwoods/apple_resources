

- Swift
- Character
-  hash(into:) 

Instance Method

# hash(into:)

Hashes the essential components of this value by feeding them into the given hasher.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func hash(into hasher: inout Hasher)
```

## Parameters 

`hasher`  

The hasher to use when combining the components of this instance.

## See Also

### Describing a Character

var description: String

A textual representation of this instance.

var debugDescription: String

A textual representation of the character, suitable for debugging.

var customMirror: Mirror

A mirror that reflects the `Character` instance.

var customPlaygroundQuickLook: _PlaygroundQuickLook

A custom playground Quick Look for the `Character` instance.

Deprecated

