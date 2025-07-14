

- AVFoundation
- AVCaptureDevice
-  AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions 

Structure

# AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions

A structure that defines the conditions in which to restrict camera switching.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+

``` source
struct PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions
```

## Overview

Use these constants to control the conditions that allow fallback camera selection when you set the value of the primaryConstituentDeviceSwitchingBehavior property to AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior.restricted.

When triggered by one or more enabled conditions, fallback camera switching waits for exposure and focus to stabilize before deciding which camera to use as the primary constituent device.

Whenever videoZoomChanged isn’t included in the restricted switching behavior conditions, AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior.restricted still allows camera selection when a change in video zoom factor makes a camera eligible or ineligible for selection as the activePrimaryConstituent.

When the video zoom factor decreases to below the switch-over zoom factor of the active primary constituent device, the system selects a different camera to satisfy the requested zoom factor.

When the video zoom factor increases and crosses a camera’s switch-over zoom factor, this camera becomes eligible to set as the activePrimaryConstituent. If exposure and focus allow, this camera then becomes the new active primary constituent device. Similar to the videoZoomChanged this also waits for exposure and focus to stabilize. Otherwise the activePrimaryConstituent remains unchanged.

## Topics

### Switching Behavior Conditions

static var exposureModeChanged: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions

Restrict switching to a fallback camera only when the device’s exposure mode changes.

static var focusModeChanged: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions

Restrict switching to a fallback camera only when the device’s focus mode changes.

static var videoZoomChanged: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions

Restrict switching to a fallback camera only when the device’s video zoom changes.

### Initializers

init(rawValue: UInt)

Creates a switching behavior condition with an unsigned integer value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Restricting Camera Switching

func setPrimaryConstituentDeviceSwitchingBehavior(AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior, restrictedSwitchingBehaviorConditions: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions)

Sets the switching behavior of the primary constituent device.

var primaryConstituentDeviceSwitchingBehavior: AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior

The switching behavior for the primary constituent device.

var primaryConstituentDeviceRestrictedSwitchingBehaviorConditions: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions

The conditions that restrict the primary constituent device’s switching behavior.

var activePrimaryConstituentDeviceSwitchingBehavior: AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior

The switching behavior of the active constituent device.

var activePrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions

The conditions that restrict camera switching behavior for the active primary constituent device.

var activePrimaryConstituent: AVCaptureDevice?

A virtual device’s active primary constituent device.

enum PrimaryConstituentDeviceSwitchingBehavior

Constants that control when to allow a virtual device to switch its active primary constituent device.

var supportedFallbackPrimaryConstituentDevices: [AVCaptureDevice]

The constituent devices available to select as a fallback for a longer focal length primary constituent device.

var fallbackPrimaryConstituentDevices: [AVCaptureDevice]

The fallback devices to use when a constituent device with a longer focal length becomes limited by its light sensitivity or minimum focus distance.

