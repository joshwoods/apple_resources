

- HealthKit
- HKContactsPrescription
-  init(rightEyeSpecification:leftEyeSpecification:brand:dateIssued:expirationDate:device:metadata:) 

Initializer

# init(rightEyeSpecification:leftEyeSpecification:brand:dateIssued:expirationDate:device:metadata:)

Creates a new glasses prescription sample.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
convenience init(
    rightEyeSpecification: HKContactsLensSpecification?,
    leftEyeSpecification: HKContactsLensSpecification?,
    brand: String,
    dateIssued: Date,
    expirationDate: Date?,
    device: HKDevice?,
    metadata: [String : Any]?
)
```

## Parameters 

`rightEyeSpecification`  

The lens specification for the right eye.

`leftEyeSpecification`  

The lens specification for the left eye.

`brand`  

The name of the prescribed brand, based on the contact lens fitting.

`dateIssued`  

The date when the doctor issued the prescription.

`expirationDate`  

The date when the prescription expires.

`device`  

The device that generated the sample.

`metadata`  

Additional metadata about the sample.

