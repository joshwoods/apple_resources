

- HealthKit
-  HKGlassesPrescription 

Class

# HKGlassesPrescription

A sample that stores a prescription for glasses.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
class HKGlassesPrescription
```

## Overview

To create a sample that stores a glasses prescription, start by defining a specification for each eye. Each lens specification object requires a `sphere` parameter. This measures the lens’s strength for correcting either nearsightedness or farsightedness (measured in diopter() units).

```
// The correction for farsightedness.
let sphere = HKQuantity(unit: .diopter(), doubleValue: -0.75)
```

Next, create values for any of the prescription’s optional parameters. For example, if the prescription corrects for astigmatism, create the `cylinder` and `axis` values. The `cylinder` value uses diopter() units, while the `axis` uses degreeAngle().

```
// The corrections for astigmatism.
let cylinder = HKQuantity(unit: .diopter(), doubleValue: -0.5)
let axis = HKQuantity(unit: .degreeAngle(), doubleValue: 155.0)
```

To add a multifocal correction for reading, create an `addPower` value using diopter() units.

```
// Multifocal correction for reading.
let addPower = HKQuantity(unit: .diopter(), doubleValue: +2.00)
```

To add a correction for eye alignment, create an HKVisionPrism object.

```
// The correction for eye alignment.
let prismQuantity = HKQuantity(unit: .prismDiopter(), doubleValue: +0.25)
let angle = HKQuantity(unit: .degreeAngle(), doubleValue: 15.0)
let prism = HKVisionPrism(amount: prismQuantity,
                          angle: angle,
                          eye: .right)
```

To add information about the distance between the eye and the back of the lens, or the pupil and the center of the nose, create `vertexDistance`, `nearDistance`, and `farDistance` values. All of these use millimeters.

```
// Distance between the back of the lens and the eye.
let vertexDistance = HKQuantity(unit: HKUnit.meterUnit(with: .milli), doubleValue: 14.0)

// Set the distance between the pupil and the center of the nose when looking at a nearby object.
let nearDistance = HKQuantity(unit: HKUnit.meterUnit(with: .milli), doubleValue: 25.0)

// Set the distance between the pupil and the center of the nose when looking far away.
let farDistance = HKQuantity(unit: HKUnit.meterUnit(with: .milli), doubleValue: 27.0)
```

Then you can create the HKGlassesLensSpecification lens specification.

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

After you create your lens specifications, you can create an HKGlassesPrescription sample.

```
// The date the doctor issued the prescription.
let dateIssued = Date()

// The date when the prescription expires.
let expirationDate = dateIssued.addingTimeInterval(60 * 24 * 365)

// The glasses prescription.
let prescription = HKGlassesPrescription(rightEyeSpecification: glassesRightEye,
                                         leftEyeSpecification: glassesLeftEye,
                                         dateIssued: dateIssued,
                                         expirationDate: expirationDate,
                                         device: HKDevice.local(),
                                         metadata: nil)
```

Then save the sample to the HealthKit store.

```
// Save the sample to the HealthKit store.
do {
    try await store.save(prescription)
} catch {
    // Handle the error here.
    fatalError("*** An error occurred while saving the prescription sample to the HealthKit store \(error.localizedDescription) ***")
}
```

Finally, add an image or PDF of the prescription to the sample as an attachment.

```
// Get the attachment store.
let attachmentStore = HKAttachmentStore(healthStore: store)

// Attach the image to the sample.
do {
    _ = try await attachmentStore.addAttachment(to: prescription,
                                                name: "Glasses Prescription",
                                                contentType: type,
                                                url: url)
} catch {
    // Handle the error.
    fatalError("*** An error occurred while attaching the image: \(error.localizedDescription) ***")
}
```

Important

Some regions may require an image of the original prescription to validate the prescription record. You can add an image or PDF of the prescription as an attachment. For more information about how to add an attachment, see HKAttachmentStore.

## Topics

### Creating glasses prescription samples

convenience init(rightEyeSpecification: HKGlassesLensSpecification?, leftEyeSpecification: HKGlassesLensSpecification?, dateIssued: Date, expirationDate: Date?, device: HKDevice?, metadata: [String : Any]?)

Creates a new glasses prescription sample.

### Accessing the glasses prescription data

var leftEye: HKGlassesLensSpecification?

The lens specification for the left eye.

var rightEye: HKGlassesLensSpecification?

The lens specification for the right eye.

### Adding metadata

let HKMetadataKeyGlassesPrescriptionDescription: String

A description of the glasses prescription.

## Relationships

### Inherits From

- HKVisionPrescription

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

class HKContactsPrescription

A sample that store a prescription for contacts.

class HKGlassesLensSpecification

An object that contains the glasses prescription data for one eye.

class HKContactsLensSpecification

An object that contains the contacts prescription data for one eye.

class HKLensSpecification

An abstract superclass for lens specifications.

class HKVisionPrism

Prescription data for eye alignment.

class HKPrescriptionType

A type that identifies samples that store a prescription.

