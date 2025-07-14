

- SwiftUI
-  Subview 

Structure

# Subview

An opaque value representing a subview of another view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct Subview
```

## Overview

Access to a `Subview` can be obtained by using `ForEach(subviews:)` or `Group(subviews:)`.

Subviews are proxies to the resolved view they represent, meaning that modifiers applied to the original view will be applied before modifiers applied to the subview, and the view is resolved using the environment of its container, *not* the environment of the its subview proxy. Additionally, because subviews must represent a single leaf view, or container, a subview may represent a view after the application of styles. As such, attempting to apply a style to it may have no affect.

## Topics

### Structures

struct ID

A unique identifier for a subview.

### Instance Properties

var containerValues: ContainerValues

The container values associated with the given subview.

var id: Subview.ID

The unique identifier of the view.

## Relationships

### Conforms To

- Identifiable
- View

## See Also

### Accessing a container’s subviews

struct SubviewsCollection

An opaque collection representing the subviews of view.

struct SubviewsCollectionSlice

func containerValue&lt;V>(WritableKeyPath&lt;ContainerValues, V>, V) -> some View

Sets a particular container value of a view.

struct ContainerValues

A collection of container values associated with a given view.

protocol ContainerValueKey

A key for accessing container values.

