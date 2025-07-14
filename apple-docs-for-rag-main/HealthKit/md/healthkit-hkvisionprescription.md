

- HealthKit
-  HKVisionPrescription 

Class

# HKVisionPrescription

A sample that stores a vision prescription.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
class HKVisionPrescription
```

## Overview

Use this class to create an image-only prescription. Here, you attach the prescription as an image or PDF to a simple sample. The sample contains only basic information about the prescription, such as the issue and expiration dates. To see the prescription data, people must view the attached image or PDF.

Important

Some regions may require an image of the original prescription to validate the prescription record.

To create an image-only prescription, start by creating an HKVisionPrescription sample object.

```
// Create a minimal prescription sample that just holds an image attachment.
let prescription = HKVisionPrescription(type: .glasses,
                                        dateIssued: Date(),
                                        expirationDate: nil,
                                        device: HKDevice.local(),
                                        metadata: nil)
```

Next, save the sample to the HealthKit store.

```
// Save the sample to the HealthKit store.
do {
    try await store.save(prescription)
} catch {
    // Handle the error here.
    fatalError("*** An error occurred while saving the prescription sample to the HealthKit store \(error.localizedDescription) ***")
}
```

Then, you can attach the image or PDF to the sample.

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

For more information about adding images or pdfs as attachments, see HKAttachmentStore. To create a vision prescription sample that contains the full data for the prescription, use HKGlassesPrescription or HKContactsPrescription instead.

## Topics

### Creating vision prescription samples

convenience init(type: HKVisionPrescriptionType, dateIssued: Date, expirationDate: Date?, device: HKDevice?, metadata: [String : Any]?)

Creates a new vision prescription sample.

### Accessing the prescription data

var prescriptionType: HKVisionPrescriptionType

The type of vision prescription.

enum HKVisionPrescriptionType

The type of vision prescription, for example a prescription for glasses or for contacts.

var dateIssued: Date

The date when the doctor issued the prescription.

var expirationDate: Date?

The date when the prescription expires.

## Relationships

### Inherits From

- HKSample

### Inherited By

- HKContactsPrescription
- HKGlassesPrescription

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

class HKVisionPrism

Prescription data for eye alignment.

class HKPrescriptionType

A type that identifies samples that store a prescription.

