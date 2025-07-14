

- ClockKit
-  CLKComplicationTemplateUtilitarianSmallRingText Deprecated

Class

# CLKComplicationTemplateUtilitarianSmallRingText

A template for displaying text encircled by a configurable progress ring.

watchOS 2.0–9.0Deprecated

``` source
class CLKComplicationTemplateUtilitarianSmallRingText
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.utilitarianSmall family.

## Topics

### Creating the Template

init(textProvider: CLKTextProvider, fillFraction: Float, ringStyle: CLKComplicationRingStyle)

Creates a new template from the provided text, fill fraction, and ring style.

### Setting the Complication Data

var textProvider: CLKTextProvider

The text to display in the complication.

var ringStyle: CLKComplicationRingStyle

The style of the progress ring.

var fillFraction: Float

The fraction of the ring to fill.

## Relationships

### Inherits From

- CLKComplicationTemplate

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Utilitarian small

class CLKComplicationTemplateUtilitarianSmallFlat

A template for displaying an image and text in a single line.

Deprecated

class CLKComplicationTemplateUtilitarianSmallRingImage

A template for displaying an image encircled by a configurable progress ring

Deprecated

class CLKComplicationTemplateUtilitarianSmallSquare

A template for displaying a single square image.

Deprecated

