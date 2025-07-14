

- Foundation
-  CocoaError 

Structure

# CocoaError

Describes errors within the Cocoa error domain.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct CocoaError
```

## Topics

### Structures

struct Code

The error code itself.

### Instance Properties

var affectedObjects: [AnyObject]?

var affectedStores: [AnyObject]?

var filePath: String?

The file path associated with the error, if any.

var isCoderError: Bool

var isExecutableError: Bool

var isFileError: Bool

var isFontError: Bool

var isFormattingError: Bool

var isPropertyListError: Bool

var isServiceError: Bool

var isSharingServiceError: Bool

var isTextReadWriteError: Bool

var isUbiquitousFileError: Bool

var isUserActivityError: Bool

var isValidationError: Bool

var isXPCConnectionError: Bool

var persistentStoreSaveConflicts: [NSMergeConflict]?

var stringEncoding: String.Encoding?

The string encoding associated with this error, if any.

var underlying: (any Error)?

The underlying error behind this error, if any.

var underlyingErrors: [any Error]

var url: URL?

The URL associated with this error, if any.

var validationKey: String?

var validationObject: Any?

var validationPredicate: NSPredicate?

var validationValue: Any?

### Type Properties

static var ServiceApplicationLaunchFailedError: CocoaError.CodeDeprecated

static var ServiceApplicationNotFoundError: CocoaError.CodeDeprecated

static var ServiceInvalidPasteboardDataError: CocoaError.CodeDeprecated

static var ServiceMalformedServiceDictionaryError: CocoaError.CodeDeprecated

static var ServiceMiscellaneousError: CocoaError.CodeDeprecated

static var ServiceRequestTimedOutError: CocoaError.CodeDeprecated

static var SharingServiceNotConfiguredError: CocoaError.CodeDeprecated

static var TextReadInapplicableDocumentTypeError: CocoaError.CodeDeprecated

static var TextWriteInapplicableDocumentTypeError: CocoaError.CodeDeprecated

static var coderInvalidValue: CocoaError.Code

static var coderReadCorrupt: CocoaError.Code

static var coderReadCorruptError: CocoaError.CodeDeprecated

static var coderValueNotFound: CocoaError.Code

static var coderValueNotFoundError: CocoaError.CodeDeprecated

static var coreData: CocoaError.Code

static var coreDataError: CocoaError.CodeDeprecated

static var entityMigrationPolicy: CocoaError.Code

static var entityMigrationPolicyError: CocoaError.CodeDeprecated

static var executableArchitectureMismatch: CocoaError.Code

static var executableArchitectureMismatchError: CocoaError.CodeDeprecated

static var executableLink: CocoaError.Code

static var executableLinkError: CocoaError.CodeDeprecated

static var executableLoad: CocoaError.Code

static var executableLoadError: CocoaError.CodeDeprecated

static var executableNotLoadable: CocoaError.Code

static var executableNotLoadableError: CocoaError.CodeDeprecated

static var executableRuntimeMismatch: CocoaError.Code

static var executableRuntimeMismatchError: CocoaError.CodeDeprecated

static var externalRecordImport: CocoaError.Code

static var externalRecordImportError: CocoaError.CodeDeprecated

static var featureUnsupported: CocoaError.Code

static var featureUnsupportedError: CocoaError.CodeDeprecated

static var fileLocking: CocoaError.Code

static var fileLockingError: CocoaError.CodeDeprecated

static var fileManagerUnmountBusy: CocoaError.Code

static var fileManagerUnmountBusyError: CocoaError.CodeDeprecated

static var fileManagerUnmountUnknown: CocoaError.Code

static var fileManagerUnmountUnknownError: CocoaError.CodeDeprecated

static var fileNoSuchFile: CocoaError.Code

static var fileNoSuchFileError: CocoaError.CodeDeprecated

static var fileReadCorruptFile: CocoaError.Code

static var fileReadCorruptFileError: CocoaError.CodeDeprecated

static var fileReadInapplicableStringEncoding: CocoaError.Code

static var fileReadInapplicableStringEncodingError: CocoaError.CodeDeprecated

static var fileReadInvalidFileName: CocoaError.Code

static var fileReadInvalidFileNameError: CocoaError.CodeDeprecated

static var fileReadNoPermission: CocoaError.Code

static var fileReadNoPermissionError: CocoaError.CodeDeprecated

static var fileReadNoSuchFile: CocoaError.Code

static var fileReadNoSuchFileError: CocoaError.CodeDeprecated

static var fileReadTooLarge: CocoaError.Code

static var fileReadTooLargeError: CocoaError.CodeDeprecated

static var fileReadUnknown: CocoaError.Code

static var fileReadUnknownError: CocoaError.CodeDeprecated

static var fileReadUnknownStringEncoding: CocoaError.Code

static var fileReadUnknownStringEncodingError: CocoaError.CodeDeprecated

static var fileReadUnsupportedScheme: CocoaError.Code

static var fileReadUnsupportedSchemeError: CocoaError.CodeDeprecated

static var fileWriteFileExists: CocoaError.Code

static var fileWriteFileExistsError: CocoaError.CodeDeprecated

static var fileWriteInapplicableStringEncoding: CocoaError.Code

static var fileWriteInapplicableStringEncodingError: CocoaError.CodeDeprecated

static var fileWriteInvalidFileName: CocoaError.Code

static var fileWriteInvalidFileNameError: CocoaError.CodeDeprecated

static var fileWriteNoPermission: CocoaError.Code

static var fileWriteNoPermissionError: CocoaError.CodeDeprecated

static var fileWriteOutOfSpace: CocoaError.Code

static var fileWriteOutOfSpaceError: CocoaError.CodeDeprecated

static var fileWriteUnknown: CocoaError.Code

static var fileWriteUnknownError: CocoaError.CodeDeprecated

static var fileWriteUnsupportedScheme: CocoaError.Code

static var fileWriteUnsupportedSchemeError: CocoaError.CodeDeprecated

static var fileWriteVolumeReadOnly: CocoaError.Code

static var fileWriteVolumeReadOnlyError: CocoaError.CodeDeprecated

static var fontAssetDownloadError: CocoaError.Code

static var formatting: CocoaError.Code

static var formattingError: CocoaError.CodeDeprecated

static var inferredMappingModel: CocoaError.Code

static var inferredMappingModelError: CocoaError.CodeDeprecated

static var keyValueValidation: CocoaError.Code

static var keyValueValidationError: CocoaError.CodeDeprecated

static var managedObjectConstraintMerge: CocoaError.Code

static var managedObjectConstraintMergeError: CocoaError.CodeDeprecated

static var managedObjectContextLocking: CocoaError.Code

static var managedObjectContextLockingError: CocoaError.CodeDeprecated

static var managedObjectExternalRelationship: CocoaError.Code

static var managedObjectExternalRelationshipError: CocoaError.CodeDeprecated

static var managedObjectMerge: CocoaError.Code

static var managedObjectMergeError: CocoaError.CodeDeprecated

static var managedObjectReferentialIntegrity: CocoaError.Code

static var managedObjectReferentialIntegrityError: CocoaError.CodeDeprecated

static var managedObjectValidation: CocoaError.Code

static var managedObjectValidationError: CocoaError.CodeDeprecated

static var migration: CocoaError.Code

static var migrationCancelled: CocoaError.Code

static var migrationCancelledError: CocoaError.CodeDeprecated

static var migrationError: CocoaError.CodeDeprecated

static var migrationManagerDestinationStore: CocoaError.Code

static var migrationManagerDestinationStoreError: CocoaError.CodeDeprecated

static var migrationManagerSourceStore: CocoaError.Code

static var migrationManagerSourceStoreError: CocoaError.CodeDeprecated

static var migrationMissingMappingModel: CocoaError.Code

static var migrationMissingMappingModelError: CocoaError.CodeDeprecated

static var migrationMissingSourceModel: CocoaError.Code

static var migrationMissingSourceModelError: CocoaError.CodeDeprecated

static var persistentStoreCoordinatorLocking: CocoaError.Code

static var persistentStoreCoordinatorLockingError: CocoaError.CodeDeprecated

static var persistentStoreIncompatibleSchema: CocoaError.Code

static var persistentStoreIncompatibleSchemaError: CocoaError.CodeDeprecated

static var persistentStoreIncompatibleVersionHash: CocoaError.Code

static var persistentStoreIncompatibleVersionHashError: CocoaError.CodeDeprecated

static var persistentStoreIncompleteSave: CocoaError.Code

static var persistentStoreIncompleteSaveError: CocoaError.CodeDeprecated

static var persistentStoreInvalidType: CocoaError.Code

static var persistentStoreInvalidTypeError: CocoaError.CodeDeprecated

static var persistentStoreOpen: CocoaError.Code

static var persistentStoreOpenError: CocoaError.CodeDeprecated

static var persistentStoreOperation: CocoaError.Code

static var persistentStoreOperationError: CocoaError.CodeDeprecated

static var persistentStoreSave: CocoaError.Code

static var persistentStoreSaveConflicts: CocoaError.Code

static var persistentStoreSaveConflictsError: CocoaError.CodeDeprecated

static var persistentStoreSaveError: CocoaError.CodeDeprecated

static var persistentStoreTimeout: CocoaError.Code

static var persistentStoreTimeoutError: CocoaError.CodeDeprecated

static var persistentStoreTypeMismatch: CocoaError.Code

static var persistentStoreTypeMismatchError: CocoaError.CodeDeprecated

static var persistentStoreUnsupportedRequestType: CocoaError.Code

static var persistentStoreUnsupportedRequestTypeError: CocoaError.CodeDeprecated

static var propertyListReadCorrupt: CocoaError.Code

static var propertyListReadCorruptError: CocoaError.CodeDeprecated

static var propertyListReadStream: CocoaError.Code

static var propertyListReadStreamError: CocoaError.CodeDeprecated

static var propertyListReadUnknownVersion: CocoaError.Code

static var propertyListReadUnknownVersionError: CocoaError.CodeDeprecated

static var propertyListWriteInvalid: CocoaError.Code

static var propertyListWriteInvalidError: CocoaError.CodeDeprecated

static var propertyListWriteStream: CocoaError.Code

static var propertyListWriteStreamError: CocoaError.CodeDeprecated

static var serviceApplicationLaunchFailed: CocoaError.Code

static var serviceApplicationLaunchFailedError: CocoaError.CodeDeprecated

static var serviceApplicationNotFound: CocoaError.Code

static var serviceApplicationNotFoundError: CocoaError.CodeDeprecated

static var serviceInvalidPasteboardData: CocoaError.Code

static var serviceInvalidPasteboardDataError: CocoaError.CodeDeprecated

static var serviceMalformedServiceDictionary: CocoaError.Code

static var serviceMalformedServiceDictionaryError: CocoaError.CodeDeprecated

static var serviceMiscellaneous: CocoaError.Code

static var serviceMiscellaneousError: CocoaError.CodeDeprecated

static var serviceRequestTimedOut: CocoaError.Code

static var serviceRequestTimedOutError: CocoaError.CodeDeprecated

static var sharingServiceNotConfigured: CocoaError.Code

static var sharingServiceNotConfiguredError: CocoaError.CodeDeprecated

static var sqlite: CocoaError.Code

static var sqliteError: CocoaError.CodeDeprecated

static var textReadInapplicableDocumentType: CocoaError.Code

static var textReadInapplicableDocumentTypeError: CocoaError.CodeDeprecated

static var textWriteInapplicableDocumentType: CocoaError.Code

static var textWriteInapplicableDocumentTypeError: CocoaError.CodeDeprecated

static var ubiquitousFileNotUploadedDueToQuota: CocoaError.Code

static var ubiquitousFileNotUploadedDueToQuotaError: CocoaError.CodeDeprecated

static var ubiquitousFileUbiquityServerNotAvailable: CocoaError.Code

static var ubiquitousFileUnavailable: CocoaError.Code

static var ubiquitousFileUnavailableError: CocoaError.CodeDeprecated

static var userActivityConnectionUnavailable: CocoaError.Code

static var userActivityConnectionUnavailableError: CocoaError.CodeDeprecated

static var userActivityHandoffFailed: CocoaError.Code

static var userActivityHandoffFailedError: CocoaError.CodeDeprecated

static var userActivityHandoffUserInfoTooLarge: CocoaError.Code

static var userActivityHandoffUserInfoTooLargeError: CocoaError.CodeDeprecated

static var userActivityRemoteApplicationTimedOut: CocoaError.Code

static var userActivityRemoteApplicationTimedOutError: CocoaError.CodeDeprecated

static var userCancelled: CocoaError.Code

static var userCancelledError: CocoaError.CodeDeprecated

static var validationDateTooLate: CocoaError.Code

static var validationDateTooLateError: CocoaError.CodeDeprecated

static var validationDateTooSoon: CocoaError.Code

static var validationDateTooSoonError: CocoaError.CodeDeprecated

static var validationInvalidDate: CocoaError.Code

static var validationInvalidDateError: CocoaError.CodeDeprecated

static var validationMissingMandatoryProperty: CocoaError.Code

static var validationMissingMandatoryPropertyError: CocoaError.CodeDeprecated

static var validationMultipleErrors: CocoaError.Code

static var validationMultipleErrorsError: CocoaError.CodeDeprecated

static var validationNumberTooLarge: CocoaError.Code

static var validationNumberTooLargeError: CocoaError.CodeDeprecated

static var validationNumberTooSmall: CocoaError.Code

static var validationNumberTooSmallError: CocoaError.CodeDeprecated

static var validationRelationshipDeniedDelete: CocoaError.Code

static var validationRelationshipDeniedDeleteError: CocoaError.CodeDeprecated

static var validationRelationshipExceedsMaximumCount: CocoaError.Code

static var validationRelationshipExceedsMaximumCountError: CocoaError.CodeDeprecated

static var validationRelationshipLacksMinimumCount: CocoaError.Code

static var validationRelationshipLacksMinimumCountError: CocoaError.CodeDeprecated

static var validationStringPatternMatching: CocoaError.Code

static var validationStringPatternMatchingError: CocoaError.CodeDeprecated

static var validationStringTooLong: CocoaError.Code

static var validationStringTooLongError: CocoaError.CodeDeprecated

static var validationStringTooShort: CocoaError.Code

static var validationStringTooShortError: CocoaError.CodeDeprecated

static var xpcConnectionInterrupted: CocoaError.Code

static var xpcConnectionInvalid: CocoaError.Code

static var xpcConnectionReplyInvalid: CocoaError.Code

### Type Methods

static func error(CocoaError.Code, userInfo: [AnyHashable : Any]?, url: URL?) -> any Error

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Error Codes

struct MachError

Describes an error in the Mach error domain.

struct POSIXError

Describes an error in the POSIX error domain.

NSError Codes

Error codes in the Cocoa error domain.

