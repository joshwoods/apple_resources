

- HealthKit
-  HKVisionPrism 

Class

# HKVisionPrism

Prescription data for eye alignment.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
class HKVisionPrism
```

## Overview

To include prism information in a glasses prescription, start by creating an HKVisionPrism object.

```
// The correction for eye alignment.
let prismQuantity = HKQuantity(unit: .prismDiopter(), doubleValue: +0.25)
let angle = HKQuantity(unit: .degreeAngle(), doubleValue: 15.0)
let prism = HKVisionPrism(amount: prismQuantity,
                          angle: angle,
                          eye: .right)
```

Then, pass this value to the HKGlassesLensSpecification’s initializer.

```
// The prescription for the right eye.
let glassesRightEye = HKGlassesLensSpecification(sphere: sphere,
                                                 cylinder: cylinder,
                                                 axis: axis,
                                                 addPower: addPower,
                                                 vertexDistance: vertexDistance,
                                                 prism: prism,
                                                 farPupillaryDistance: farDistance,
                                                 nearPupillaryDistance: nearDistance)
```

Finally, create the glasses prescription and save it to the HealthKit store.

```
// The glasses prescription.
let prescription = HKGlassesPrescription(rightEyeSpecification: glassesRightEye,
                                               leftEyeSpecification: glassesLeftEye,
                                               dateIssued: dateIssued,
                                               expirationDate: expirationDate,
                                               device: HKDevice.local(),
                                               metadata: nil)
// Save the sample to the HealthKit store.
do {
    try await store.save(prescription)
} catch {
    // Handle the error here.
    fatalError("*** An error occurred while saving the prescription sample to the HealthKit store \(error.localizedDescription) ***")
}
```

## Topics

### Creating vision prism objects

init(amount: HKQuantity, angle: HKQuantity, eye: HKVisionEye)

Creates a new vision prism object, using a single quantity and an alignment angle.

init(verticalAmount: HKQuantity, verticalBase: HKPrismBase, horizontalAmount: HKQuantity, horizontalBase: HKPrismBase, eye: HKVisionEye)

Creates a new vision prism object that separates the correction strength into horizontal and vertical components.

### Accessing lens specification data

var eye: HKVisionEye

A value indicating which eye the correction applies to.

enum HKVisionEye

A value that specifies the eye for a vision prescription.

var amount: HKQuantity

The strength of the correction.

var angle: HKQuantity

The orientation of the adjustment.

var horizontalAmount: HKQuantity

The strength of the horizontal correction.

var horizontalBase: HKPrismBase

The orientation of the horizontal portion of the correction.

var verticalAmount: HKQuantity

The strength of the vertical correction.

var verticalBase: HKPrismBase

The orientation of the vertical portion of the correction.

enum HKPrismBase

The orientation of the prism correction, represented by the location of the prism’s base (the thickest part of the prism).

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Vision prescriptions

class HKVisionPrescription

A sample that stores a vision prescription.

class HKGlassesPrescription

A sample that stores a prescription for glasses.

class HKContactsPrescription

A sample that store a prescription for contacts.

class HKGlassesLensSpecification

An object that contains the glasses prescription data for one eye.

class HKContactsLensSpecification

An object that contains the contacts prescription data for one eye.

class HKLensSpecification

An abstract superclass for lens specifications.

class HKPrescriptionType

A type that identifies samples that store a prescription.

