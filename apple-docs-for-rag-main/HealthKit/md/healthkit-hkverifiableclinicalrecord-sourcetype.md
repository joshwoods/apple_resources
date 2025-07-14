

- HealthKit
- HKVerifiableClinicalRecord
-  sourceType 

Instance Property

# sourceType

The source for the verifiable clinical record

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOS 1.0+

``` source
var sourceType: HKVerifiableClinicalRecordSourceType? { get }
```

## Discussion

For a list of valid sources, see HKVerifiableClinicalRecordSourceType.

## See Also

### Reading Metadata

var issuedDate: Date

The date when the issuer created the card.

var relevantDate: Date

A date relevant to this record, such as when the issuer administered a vaccine or performed a test.

var expirationDate: Date?

The date when the card expires.

var recordTypes: [String]

An array of strings representing the types of records contained in the card.

struct HKVerifiableClinicalRecordSourceType

The source type for the verifiable clinical record.

var itemNames: [String]

A human-readable description of the card’s contents.

