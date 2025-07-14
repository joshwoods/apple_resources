

- SwiftUI
-  ZStackContent3D 

Structure

# ZStackContent3D

A type that adds spacing to a ZStack.

visionOS 2.0+

``` source
@frozen
struct ZStackContent3D where Content : View
```

## Overview

You don’t create this type directly. SwiftUI creates it for you when you use the `ZStack(alignment:spacing:content)` initializer.

## Topics

### Initializers

init(spacing: CGFloat?, content: Content)

### Instance Properties

var content: Content

var spacing: CGFloat?

## Relationships

### Conforms To

- Copyable
- View

  Conforms when `Content` conforms to `View`.

