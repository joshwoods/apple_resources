

- AppKit
-  NSCollectionLayoutContainer 

Protocol

# NSCollectionLayoutContainer

A protocol used to provide information about the size and content insets of a layout’s container.

macOS 10.15+

``` source
@MainActor
protocol NSCollectionLayoutContainer : NSObjectProtocol
```

## Overview

In a section provider, you use the container property of the layout environment (NSCollectionLayoutEnvironment) to get information about the container of the layout, such as its size and content insets. Knowing about the container’s size while rendering the layout’s sections helps you make decisions about how to display the layout.

## Topics

### Getting content size

var contentSize: NSSize

The size of the container before content insets are applied.

**Required**

var effectiveContentSize: NSSize

The size of the container after content insets are applied.

**Required**

### Getting content insets

var contentInsets: NSDirectionalEdgeInsets

The amount of space added around the content of the container to adjust its final size.

**Required**

var effectiveContentInsets: NSDirectionalEdgeInsets

The amount of space added around the content of the container to adjust its final size after item content insets are applied.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Size and spacing

class NSCollectionLayoutDimension

An individual dimension representing an item’s width or height in a collection view.

class NSCollectionLayoutSize

The width and the height of an item in a collection view.

class NSCollectionLayoutSpacing

An object that defines the space between or around items in a collection view.

class NSCollectionLayoutEdgeSpacing

An object that defines the space around the edges of items in a collection view.

