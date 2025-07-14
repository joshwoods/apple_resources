

- WebKit
- WKWebsiteDataStore
-  isPersistent 

Instance Property

# isPersistent

A Boolean value that indicates whether this object stores data to disk.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
@MainActor
var isPersistent: Bool { get }
```

## Discussion

The value of this property is true if the data store writes data to disk, or false if it doesn’t.

## See Also

### Inspecting data store properties

var identifier: UUID?

An identifier that uniquely identifies a data store.

