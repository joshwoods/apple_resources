

- HealthKit
-  HKContactsLensSpecification 

Class

# HKContactsLensSpecification

An object that contains the contacts prescription data for one eye.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
class HKContactsLensSpecification
```

## Overview

To create a sample that stores a contacts prescription, start by defining a specification for each eye. Each lens specification object requires a `sphere` parameter. This measures the lens’s strength for correcting either nearsightedness or farsightedness (measured in diopter() units).

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

To add fitting information for the contact lens, create `baseCurve` and `diameter` values. Both of these values use millimeters.

```
// The fitting information.
let baseCurve = HKQuantity(unit: HKUnit.meterUnit(with: .milli),
                           doubleValue: 9.0)

let diameter = HKQuantity(unit: HKUnit.meterUnit(with: .milli),
                          doubleValue: 12.0)
```

Then you can create the HKContactsLensSpecification lens specification.

```
// The prescription for the right eye.
let contactsRightEye = HKContactsLensSpecification(sphere: sphere,
                                                   cylinder: cylinder,
                                                   axis: axis,
                                                   addPower: addPower,
                                                   baseCurve: baseCurve,
                                                   diameter: diameter)
```

After you create your lens specifications, you can create an HKContactsPrescription sample.

```
// The date the doctor issued the prescription.
let dateIssued = Date()

// The date when the prescription expires.
let expirationDate = dateIssued.addingTimeInterval(60 * 24 * 365)

// The contacts prescription.
let prescription = HKContactsPrescription(rightEyeSpecification: contactsRightEye,
                                          leftEyeSpecification: contactsLeftEye,
                                          brand: "MyBrand Name",
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

Many regions require an image of the prescription to manufacture glasses or contacts. Add an image or pdf of the prescription as an attachment. For more information, see HKAttachmentStore.

## Topics

### Creating contacts lens specifications

init(sphere: HKQuantity, cylinder: HKQuantity?, axis: HKQuantity?, addPower: HKQuantity?, baseCurve: HKQuantity?, diameter: HKQuantity?)

Creates a new contact lens specification, containing the prescription data for one eye.

### Accessing the specification’s data

var baseCurve: HKQuantity?

Part of the contact’s fit, it measures the curve of the back side of the contact, measured in mm.

var diameter: HKQuantity?

Part of the contact’s fit, it measures the diameter of the lens, measured in mm.

## Relationships

### Inherits From

- HKLensSpecification

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

class HKLensSpecification

An abstract superclass for lens specifications.

class HKVisionPrism

Prescription data for eye alignment.

class HKPrescriptionType

A type that identifies samples that store a prescription.

