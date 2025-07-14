

- AppKit
-  NSUserInterfaceCompression 

Protocol

# NSUserInterfaceCompression

A protocol that describes how a UI control should redisplay when space is restricted.

macOS

``` source
protocol NSUserInterfaceCompression
```

## Overview

A control that adopts this protocol has the ability to resize itself when space is at a premium.

## Topics

### Compressing the UI

func compress(withPrioritizedCompressionOptions: [NSUserInterfaceCompressionOptions])

Compress the view by applying the specified compression options.

**Required**

### Querying Compression Status

func minimumSize(withPrioritizedCompressionOptions: [NSUserInterfaceCompressionOptions]) -> NSSize

Returns the minimum size a view can achieve by applying the supplied compression options.

**Required**

var activeCompressionOptions: NSUserInterfaceCompressionOptions

The compression options that are currently applied to the view.

**Required**

## Relationships

### Conforming Types

- NSButton
- NSPopUpButton
- NSSegmentedControl
- NSStatusBarButton

