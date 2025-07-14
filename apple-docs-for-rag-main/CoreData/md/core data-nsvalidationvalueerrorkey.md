

- Core Data
-  NSValidationValueErrorKey 

Global Variable

# NSValidationValueErrorKey

The error key for the value that failed to validate.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
let NSValidationValueErrorKey: String
```

## See Also

### Managing Data Validation

func validateValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>, forKey: String) throws

Validates a property value for a given key.

func validateForDelete() throws

Determines whether the managed object can be deleted in its current state.

func validateForInsert() throws

Determines whether the managed object can be inserted in its current state.

func validateForUpdate() throws

Determines whether the managed object’s current state is valid.

Validation error codes

Error codes relating to the validation of managed objects.

let NSValidationKeyErrorKey: String

The error key for the attribute that failed to validate.

let NSValidationObjectErrorKey: String

The error key for the object that failed to validate.

let NSValidationPredicateErrorKey: String

The error key for the predicate that failed to validate.

