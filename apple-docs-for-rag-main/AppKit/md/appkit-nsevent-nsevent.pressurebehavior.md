

- AppKit
- NSEvent
-  NSEvent.PressureBehavior 

Enumeration

# NSEvent.PressureBehavior

These constants describe the behavior and progression of a pressure gesture.

macOS 10.10.3+

``` source
enum PressureBehavior
```

## Overview

These constants describe the behavior and progression of a pressure gesture. They allow you to configure how pressure from a pressure-sensitive device, such as the Force Touch trackpad, is interpreted by the system. For example, a drawing or painting app may adjust the behavior of pressure events to focus on variable pressure and prevent force clicks from occurring.

In most cases, a pressure gesture’s behavior goes into effect when the gesture event’s stage property reaches a value of `1` and remains in effect until the gesture event’s stage property reaches a value of `0`. This behavior corresponds to the behavior of simultaneously generated mouse-up and mouse-down events.

## Topics

### Constants

case unknown

A pressure gesture’s behavior is not known, perhaps because the input device does not support pressure gestures.

case primaryDefault

This is the default behavior when a pressure gesture’s behavior has not been explicitly configured. In OS X 10.10.3, this behavior defaults to the behavior of `NSPressureBehaviorPrimaryDeepClick`.

case primaryClick

A pressure gesture’s behavior begins on left mouse-down events. A maximum of one stage is supported, and a stage transition animation occurs when moving from stage 1 to stage 0. Actuations (haptic feedback the user feels) occur during mouse-down and mouse-up events when this behavior is configured. Note that the pressure gesture operates on a separate event stream from the mouse events.

case primaryGeneric

A pressure gesture’s behavior begins on left mouse-down events. A maximum of one stage is supported, and a stage transition animation occurs when moving from stage 1 to stage 0. Actuations occur during the mouse-down and mouse-up events when this behavior is configured. This configuration is ideal for drawing, painting, and general use. Variable pressure occurs throughout the course of the gesture. Note that the pressure gesture operates on a separate event stream from the mouse events.

case primaryAccelerator

A pressure gesture’s behavior begins on left mouse-down events. A maximum of one stage is supported, and a stage transition animation occurs when moving from stage 1 to stage 0. Actuations occur during the mouse-down and mouse-up events when this behavior is configured. This configuration uses specific pressure mappings that are ideal for controlling speed as variable pressure occurs between the mouse-down and mouse-up events. The NSAcceleratorButton class uses this behavior. Note that the pressure gesture operates on a separate event stream from the mouse events.

case primaryDeepClick

A pressure gesture’s behavior begins on left mouse-down events. Two stages are supported, and a stage transition animation may occur when moving between stages—from stage 1 to stage 0, stage 1 to stage 2, stage 2 to stage 1, and stage 2 to stage 0. With this behavior type, stage 2 becomes disabled once dragging occurs. When this behavior is configured, actuations occur during the mouse-down and mouse-up events, as well as when force click is activated and released when entering or exiting stage 2. This configuration is ideal for responding to force clicks. Note that the pressure gesture operates on a separate event stream from the mouse events.

case primaryDeepDrag

A pressure gesture’s behavior begins on left mouse-down events. Two stages are supported, and a stage transition animation may occur when moving between stages—from stage 1 to stage 0, stage 1 to stage 2, stage 2 to stage 1, or stage 2 to stage 0. Actuations occur during the mouse-down and mouse-up events, as well as during the transitions up and down between stage 1 and stage 2, when this behavior is configured. This configuration is ideal for responding to force clicks during drag operations. Note that the pressure gesture operates on a separate event stream from the mouse events.

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

### Getting pressure information

var pressure: Float

A normalized value that indicates the degree of pressure applied to an appropriate input device.

var stage: Int

A value that indicates the stage of a pressure gesture event.

var stageTransition: CGFloat

The transition value for the stage of a pressure gesture event.

var pressureBehavior: NSEvent.PressureBehavior

The behavior and progression for a pressure event.

