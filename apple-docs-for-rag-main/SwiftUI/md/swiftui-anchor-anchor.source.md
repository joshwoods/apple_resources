

- SwiftUI
- Anchor
-  Anchor.Source 

Structure

# Anchor.Source

A type-erased geometry value that produces an anchored value of a given type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct Source
```

## Overview

SwiftUI passes anchored geometry values around the view tree via preference keys. It then converts them back into the local coordinate space using a GeometryProxy value.

## Topics

### Getting point anchor sources

static func point(CGPoint) -> Anchor&lt;Value>.Source

static func unitPoint(UnitPoint) -> Anchor&lt;Value>.Source

### Getting rectangle anchor sources

static func rect(CGRect) -> Anchor&lt;Value>.Source

Returns an anchor source rect defined by `r` in the current view.

static var bounds: Anchor&lt;CGRect>.Source

An anchor source rect defined as the entire bounding rect of the current view.

### Getting top anchor sources

static var topLeading: Anchor&lt;CGPoint>.Source

static var top: Anchor&lt;CGPoint>.Source

static var topTrailing: Anchor&lt;CGPoint>.Source

### Getting middle anchor sources

static var leading: Anchor&lt;CGPoint>.Source

static var center: Anchor&lt;CGPoint>.Source

static var trailing: Anchor&lt;CGPoint>.Source

### Getting bottom anchor sources

static var bottomTrailing: Anchor&lt;CGPoint>.Source

static var bottom: Anchor&lt;CGPoint>.Source

static var bottomLeading: Anchor&lt;CGPoint>.Source

### Creating an anchor source

init(_:)

## Relationships

### Conforms To

- Sendable

