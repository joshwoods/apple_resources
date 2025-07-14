

- UIKit
-  UISheetPresentationControllerDetentResolutionContext 

Protocol

# UISheetPresentationControllerDetentResolutionContext

A context for resolving custom detent values.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
@MainActor
protocol UISheetPresentationControllerDetentResolutionContext : NSObjectProtocol
```

## Overview

A context of this type is available in the `resolver` closure of custom(identifier:resolver:) (Swift) or customDetentWithIdentifier:resolver: (Objective-C).

## Topics

### Accessing the properties of the context

var containerTraitCollection: UITraitCollection

The trait collection of the sheet’s container view.

**Required**

var maximumDetentValue: CGFloat

The maximum value of a detent.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Creating a custom detent

static func custom(identifier: UISheetPresentationController.Detent.Identifier?, resolver: (any UISheetPresentationControllerDetentResolutionContext) -> CGFloat?) -> UISheetPresentationController.Detent

Creates a custom detent for a sheet by computing its value according to the properties of the provided context.

func resolvedValue(in: any UISheetPresentationControllerDetentResolutionContext) -> CGFloat?

Resolves a detent to its value.

