

- Virtualization
-  VZVirtualMachineView 

Class

# VZVirtualMachineView

A view that allows user interaction with a VM.

macOS 12.0+

``` source
@MainActor
class VZVirtualMachineView
```

## Overview

The `VZVirtualMachineView` is a UI element that shows the contents of the VM frame buffer that you can optionally configure to respond to changes in the host’s display settings. If the VM configuration includes a keyboard and a pointing device, the view forwards keyboard and mouse events to the VM through those devices.

## Topics

### Configuring the VM

var automaticallyReconfiguresDisplay: Bool

A Boolean value that indicates whether the graphics display associated with this view automatically reconfigures with respect to view changes.

var capturesSystemKeys: Bool

A Boolean value that determines whether the system should send certain system keyboard shortcuts to the guest instead of the host.

var virtualMachine: VZVirtualMachine?

The VM to display in the view.

## Relationships

### Inherits From

- NSView

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification

## See Also

### Runtime

class VZVirtualMachine

An object that manages the overall state and configuration of your VM.

class VZLinuxRosettaDirectoryShare

The Linux directory share for Rosetta.

