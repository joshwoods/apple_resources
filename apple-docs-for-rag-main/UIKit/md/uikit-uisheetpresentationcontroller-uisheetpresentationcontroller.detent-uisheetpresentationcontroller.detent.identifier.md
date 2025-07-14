

- UIKit
- UISheetPresentationController
- UISheetPresentationController.Detent
-  UISheetPresentationController.Detent.Identifier 

Structure

# UISheetPresentationController.Detent.Identifier

Constants that identify system detent sizes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
struct Identifier
```

## Topics

### Identifying detent size

static let large: UISheetPresentationController.Detent.Identifier

The identifier for the system’s large detent.

static let medium: UISheetPresentationController.Detent.Identifier

The identifier for the system’s medium detent.

### Creating a detent identifier

init(String)

Creates a detent identifier.

init(rawValue: String)

Creates a detent identifier with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Identifying a detent

var identifier: UISheetPresentationController.Detent.Identifier

The identifier of the detent.

