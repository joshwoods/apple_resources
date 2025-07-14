

- Core Data
- Core Data Constants
-  Validation Error Codes 

API Collection

# Validation Error Codes

Error codes relating to the validation of managed objects.

## Topics

### Error codes

var NSCoreDataError: Int

An error code that indicates a nonspecific Core Data error.

var NSEntityMigrationPolicyError: Int

An error code that indicates a migration failure during processing of an entity migration policy.

var NSExternalRecordImportError: Int

Error code to denote a general error encountered while importing external records.

var NSInferredMappingModelError: Int

Error code to denote a problem with the creation of an inferred mapping model.

var NSManagedObjectConstraintMergeError: Int

Error code to denote a problem with the merging of instances of a managed object.

var NSManagedObjectConstraintValidationError: Int

Error code to denote a problem with the validation of a managed object.

var NSManagedObjectContextLockingError: Int

Error code to denote an inability to acquire a lock in a managed object context.

var NSManagedObjectExternalRelationshipError: Int

Error code to denote that an object being saved has a relationship containing an object from another store.

var NSManagedObjectMergeError: Int

Error code to denote that a merge policy failed—Core Data is unable to complete merging.

var NSManagedObjectModelReferenceNotFoundError: Int

An error code that indicates Core Data isn’t able to find or instantiate the referenced object model.

var NSManagedObjectReferentialIntegrityError: Int

Error code to denote an attempt to fire a fault pointing to an object that does not exist.

var NSManagedObjectValidationError: Int

Error code to denote a generic validation error.

var NSMigrationCancelledError: Int

Error code to denote that migration failed due to manual cancellation.

var NSMigrationConstraintViolationError: Int

Error code to denote a problem with the validation of a managed object during a migration.

var NSMigrationError: Int

Error code to denote a general migration error.

var NSMigrationManagerDestinationStoreError: Int

Error code to denote that migration failed due to a problem with the destination data store.

var NSMigrationManagerSourceStoreError: Int

Error code to denote that migration failed due to a problem with the source data store.

var NSMigrationMissingMappingModelError: Int

Error code to denote that migration failed due to a missing mapping model.

var NSMigrationMissingSourceModelError: Int

Error code to denote that migration failed due to a missing source data model.

var NSPersistentHistoryTokenExpiredError: Int

Error code to denote that the persistent history token has expired.

var NSPersistentStoreCoordinatorLockingError: Int

Error code to denote an inability to acquire a lock in a persistent store.

var NSPersistentStoreIncompatibleSchemaError: Int

Error code to denote that a persistent store returned an error for a save operation.

var NSPersistentStoreIncompatibleVersionHashError: Int

Error code to denote that entity version hashes in the store are incompatible with the current managed object model.

var NSPersistentStoreIncompleteSaveError: Int

Error code to denote that one or more of the stores returned an error during a save operations.

var NSPersistentStoreInvalidTypeError: Int

Error code to denote an unknown persistent store type/format/version.

var NSPersistentStoreOpenError: Int

Error code to denote an error occurred while attempting to open a persistent store.

var NSPersistentStoreOperationError: Int

Error code to denote that a persistent store operation failed.

var NSPersistentStoreSaveConflictsError: Int

Error code to denote that an unresolved merge conflict was encountered during a save. .

var NSPersistentStoreSaveError: Int

Error code to denote that a persistent store returned an error for a save operation.

var NSPersistentStoreTimeoutError: Int

Error code to denote that Core Data failed to connect to a persistent store within the time specified by `NSPersistentStoreTimeoutOption`.

var NSPersistentStoreTypeMismatchError: Int

Error code returned by a persistent store coordinator if a store is accessed that does not match the specified type.

var NSPersistentStoreUnsupportedRequestTypeError: Int

Error code to denote that an `NSPersistentStore` subclass was passed a request (an instance of NSPersistentStoreRequest) that it did not understand.

var NSSQLiteError: Int

Error code to denote a general SQLite error.

var NSStagedMigrationBackwardMigrationError: Int

An error code that indicates a failed migration because of an attempt to migrate backward.

var NSStagedMigrationFrameworkVersionMismatchError: Int

An error code that indicates a failed migration because the persistent store’s metadata doesn’t support staged lightweight migrations.

var NSValidationInvalidURIError: Int

Error code to denote a problem with the validation of a URI property.

var NSValidationMultipleErrorsError: Int

Error code to denote an error containing multiple validation errors.

var NSValidationMissingMandatoryPropertyError: Int

Error code for a non-optional property with a nil value.

var NSValidationRelationshipLacksMinimumCountError: Int

Error code to denote a to-many relationship with too few destination objects.

var NSValidationRelationshipExceedsMaximumCountError: Int

Error code to denote a bounded to-many relationship with too many destination objects.

var NSValidationRelationshipDeniedDeleteError: Int

Error code to denote some relationship with delete rule `NSDeleteRuleDeny` is non-empty.

var NSValidationNumberTooLargeError: Int

Error code to denote some numerical value is too large.

var NSValidationNumberTooSmallError: Int

Error code to denote some numerical value is too small.

var NSValidationDateTooLateError: Int

Error code to denote some date value is too late.

var NSValidationDateTooSoonError: Int

Error code to denote some date value is too soon.

var NSValidationInvalidDateError: Int

Error code to denote some date value fails to match date pattern.

var NSValidationStringTooLongError: Int

Error code to denote some string value is too long.

var NSValidationStringTooShortError: Int

Error code to denote some string value is too short.

var NSValidationStringPatternMatchingError: Int

Error code to denote some string value fails to match some pattern.

## See Also

### Errors

let NSSQLiteErrorDomain: String

Domain for SQLite errors.

