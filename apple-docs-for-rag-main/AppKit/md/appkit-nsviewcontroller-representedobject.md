

- AppKit
- NSViewController
-  representedObject 

Instance Property

# representedObject

The object whose value is presented in the receiver’s primary view.

macOS 10.5+

``` source
@MainActor
var representedObject: Any? { get set }
```

## Discussion

This property *retains* the object you provide to it; it does not *copy* it. In another words, a view controller has a *to-one* relationship with its represented object and does not own it as an attribute.

The representedObject property is key-value coding and key-value observing compliant. When you use the represented object as the file’s owner of a nib file, you can bind controls to the file’s owner using key paths that start with the string `representedObject`.

