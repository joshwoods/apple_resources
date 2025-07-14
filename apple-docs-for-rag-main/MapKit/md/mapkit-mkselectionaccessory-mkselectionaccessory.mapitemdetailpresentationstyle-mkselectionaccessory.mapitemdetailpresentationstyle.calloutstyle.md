

- MapKit
- MKSelectionAccessory
- MKSelectionAccessory.MapItemDetailPresentationStyle
-  MKSelectionAccessory.MapItemDetailPresentationStyle.CalloutStyle 

Enumeration

# MKSelectionAccessory.MapItemDetailPresentationStyle.CalloutStyle

The style to use for a map item detail callout presentation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum CalloutStyle
```

## Overview

In Swift, use MKSelectionAccessory.MapItemDetailPresentationStyle.CalloutStyle.full for map views on iPadOS and macOS. Use a sheet presentation to display full detail place information on iOS.

In Objective-C, use MKSelectionAccessory.MapItemDetailPresentationStyle.CalloutStyle.full for map views on iPadOS and macOS. Use a sheet presentation to display full detail place information on iOS.

## Topics

### Enumeration Cases

case automatic

A value that allows the framework to choose an appropriate callout style automatically.

case compact

A compact, space-saving callout style.

case full

A rich, detailed callout style that is suitable for large map views.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Place information

protocol MKMapItemDetailViewControllerDelegate

The methods that you use to receive events from an associated map view controller.

class MKMapItemDetailViewController

An object that displays detailed information about a map item.

class MapItemDetailPresentationStyle

The type of map item detail accessory presentation to use.

class MKSelectionAccessory

The type of accessory to display for a selected annotation.

