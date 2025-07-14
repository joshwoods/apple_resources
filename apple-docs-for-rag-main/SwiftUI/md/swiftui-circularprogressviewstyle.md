

- SwiftUI
-  CircularProgressViewStyle 

Structure

# CircularProgressViewStyle

A progress view that uses a circular gauge to indicate the partial completion of an activity.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
struct CircularProgressViewStyle
```

## Overview

On watchOS, and in widgets and complications, a circular progress view appears as a gauge with the accessoryCircularCapacity style. If the progress view is indeterminate, the gauge is empty.

In cases where no determinate circular progress view style is available, circular progress views use an indeterminate style.

Use circular to construct the circular progress view style.

## Topics

### Creating the progress view style

init()

Creates a circular progress view style.

### Deprecated initializers

init(tint: Color)

Creates a circular progress view style with a tint color.

Deprecated

## Relationships

### Conforms To

- ProgressViewStyle

## See Also

### Supporting types

struct DefaultProgressViewStyle

The default progress view style in the current context of the view being styled.

struct LinearProgressViewStyle

A progress view that visually indicates its progress using a horizontal bar.

