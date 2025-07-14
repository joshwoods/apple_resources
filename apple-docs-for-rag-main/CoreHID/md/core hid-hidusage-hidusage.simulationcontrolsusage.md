

- Core HID
- HIDUsage
-  HIDUsage.SimulationControlsUsage 

Enumeration

# HIDUsage.SimulationControlsUsage

macOS 15.0+

``` source
enum SimulationControlsUsage
```

## Topics

### Enumeration Cases

case accelerator

case aileron

case aileronTrim

case airplaneSimulationDevice

case antiTorqueControl

case automobileSimulationDevice

case autopilotEnable

case ballast

case barrelElevation

case bicycleCrank

case bicycleSimulationDevice

case brake

case chaffRelease

case clutch

case collectiveControl

case cyclicControl

case cyclicTrim

case diveBrake

case divePlane

case electronicCountermeasures

case elevator

case elevatorTrim

case flareRelease

case flightCommunications

case flightControlStick

case flightSimulationDevice

case flightStick

case flightYoke

case frontBrake

case handleBars

case helicopterSimulationDevice

case landingGear

case magicCarpetSimulationDevice

case motorcycleSimulationDevice

case rearBrake

case rudder

case sailingSimulationDevice

case shifter

case spaceshipSimulationDevice

case sportsSimulationDevice

case steering

case submarineSimulationDevice

case tankSimulationDevice

case throttle

case toeBrake

case trackControl

case trigger

case turretDirection

case weaponsArm

case weaponsSelect

case wingFlaps

### Initializers

init?(rawValue: UInt16)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: UInt16

The corresponding value of the raw type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let page: UInt16

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

