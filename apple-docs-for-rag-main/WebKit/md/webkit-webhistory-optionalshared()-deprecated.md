

- WebKit
- WebHistory
-  optionalShared() Deprecated

Type Method

# optionalShared()

Returns a shared web history object, if one exists.

macOS 10.3–10.14Deprecated

``` source
class func optionalShared() -> WebHistory!
```

## Return Value

A shared web history object initialized with the default web history file, or `nil` if one was not previously specified using the setOptionalShared(_:) method.

## See Also

### Related Documentation

func load(from: URL!) throws

Loads the contents of the specified web history file.

Deprecated

WebKit Objective-C Programming Guide

### Accessing Shared History Objects

class func setOptionalShared(WebHistory!)

Sets the web history object to share.

Deprecated

