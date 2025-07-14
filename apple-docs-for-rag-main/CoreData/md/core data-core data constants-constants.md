

- Core Data
-  Core Data Constants 

API Collection

# Core Data Constants

Keys to use with persistent stores and notifications from Core Data.

## Topics

### Core Data Versions

var NSCoreDataVersionNumber: Double

The version of Core Data available in the current process.

var NSCoreDataVersionNumber10_10: Double

The Core Data version number released with macOS 10.10.

var NSCoreDataVersionNumber10_10_2: Double

The Core Data version number released with macOS 10.10.2.

var NSCoreDataVersionNumber10_10_3: Double

The Core Data version number released with macOS 10.10.3.

var NSCoreDataVersionNumber10_11: Double

The Core Data version number released with macOS 10.11.

var NSCoreDataVersionNumber10_11_3: Double

The Core Data version number released with macOS 10.11.3.

var NSCoreDataVersionNumber10_4: Double

The Core Data version number released with macOS 10.4.

var NSCoreDataVersionNumber10_4_3: Double

The Core Data version number released with macOS 10.4.3.

var NSCoreDataVersionNumber10_5: Double

The Core Data version number released with macOS 10.5.

var NSCoreDataVersionNumber10_5_3: Double

The Core Data version number released with macOS 10.5.3.

var NSCoreDataVersionNumber10_6: Double

The Core Data version number released with macOS 10.6.

var NSCoreDataVersionNumber10_6_2: Double

The Core Data version number released with macOS 10.6.2.

var NSCoreDataVersionNumber10_6_3: Double

The Core Data version number released with macOS 10.6.3.

var NSCoreDataVersionNumber10_7: Double

The Core Data version number released with macOS 10.7.

var NSCoreDataVersionNumber10_7_2: Double

The Core Data version number released with macOS 10.7.2.

var NSCoreDataVersionNumber10_7_3: Double

The Core Data version number released with macOS 10.7.3.

var NSCoreDataVersionNumber10_7_4: Double

The Core Data version number released with macOS 10.7.4.

var NSCoreDataVersionNumber10_8: Double

The Core Data version number released with macOS 10.8.

var NSCoreDataVersionNumber10_8_2: Double

The Core Data version number released with macOS 10.8.2.

var NSCoreDataVersionNumber10_9: Double

The Core Data version number released with macOS 10.9.

var NSCoreDataVersionNumber10_9_2: Double

The Core Data version number released with macOS 10.9.2.

var NSCoreDataVersionNumber10_9_3: Double

The Core Data version number released with macOS 10.9.3.

var NSCoreDataVersionNumber_iPhoneOS_3_0: Double

The Core Data version number released with iOS 3.

var NSCoreDataVersionNumber_iPhoneOS_3_1: Double

The Core Data version number released with iOS 3.1.

var NSCoreDataVersionNumber_iPhoneOS_3_2: Double

The Core Data version number released with iOS 3.2.

var NSCoreDataVersionNumber_iPhoneOS_4_0: Double

The Core Data version number released with iOS 4.

var NSCoreDataVersionNumber_iPhoneOS_4_1: Double

The Core Data version number released with iOS 4.1.

var NSCoreDataVersionNumber_iPhoneOS_4_2: Double

The Core Data version number released with iOS 4.2.

var NSCoreDataVersionNumber_iPhoneOS_4_3: Double

The Core Data version number released with iOS 4.2.

var NSCoreDataVersionNumber_iPhoneOS_5_0: Double

The Core Data version number released with iOS 5.

var NSCoreDataVersionNumber_iPhoneOS_5_1: Double

The Core Data version number released with iOS 5.1.

var NSCoreDataVersionNumber_iPhoneOS_6_0: Double

The Core Data version number released with iOS 6.

var NSCoreDataVersionNumber_iPhoneOS_6_1: Double

The Core Data version number released with iOS 6.1.

var NSCoreDataVersionNumber_iPhoneOS_7_0: Double

The Core Data version number released with iOS 7.0.

var NSCoreDataVersionNumber_iPhoneOS_7_1: Double

The Core Data version number released with iOS 7.1.

var NSCoreDataVersionNumber_iPhoneOS_8_0: Double

The Core Data version number released with iOS 8.0.

var NSCoreDataVersionNumber_iPhoneOS_8_3: Double

The Core Data version number released with iOS 8.3.

var NSCoreDataVersionNumber_iPhoneOS_9_0: Double

The Core Data version number released with iOS 9.0.

var NSCoreDataVersionNumber_iPhoneOS_9_2: Double

The Core Data version number released with iOS 9.2.

var NSCoreDataVersionNumber_iPhoneOS_9_3: Double

The Core Data version number released with iOS 9.3.

### Errors

let NSSQLiteErrorDomain: String

Domain for SQLite errors.

Validation Error Codes

Error codes relating to the validation of managed objects.

### User Info Dictionary Keys

let NSAffectedObjectsErrorKey: String

The key for objects prompting an error.

let NSAffectedStoresErrorKey: String

The key for stores prompting an error.

let NSDetailedErrorsKey: String

If multiple validation errors occur in one operation, they are collected in an array and added with this key to the “top-level error” of the operation.

let NSDeletedObjectIDsKey: String

A user info key to identify deleted object identifiers in notifications after saving a managed object context.

let NSInsertedObjectIDsKey: String

A user info key to identify inserted object identifiers in notifications after saving a managed object context.

let NSInvalidatedObjectIDsKey: String

A user info key to identify invalidated object identifiers in notifications after saving a managed object context.

let NSPersistentHistoryTokenKey: String

A user info key to identify the history token in persistent store remote change notifications.

let NSPersistentStoreURLKey: String

A user info key to identify the store URL in persistent store remote change notifications.

let NSRefreshedObjectIDsKey: String

A user info key to identify refreshed object identifiers in notifications after saving a managed object context.

let NSUpdatedObjectIDsKey: String

A user info key to identify updated object identifiers in notifications after saving a managed object context.

### Persistent Store Metadata Keys

let NSBinaryStoreInsecureDecodingCompatibilityOption: String

A flag that indicates Core Data decodes the binary store insecurely.

let NSBinaryStoreSecureDecodingClasses: String

An additional set of classes to use while decoding a binary store.

let NSPersistentStoreRemoteChangeNotificationPostOptionKey: String

A key that indicates a persistent store posts a remote change notification for every write to the store, including writes by other processes.

let NSPersistentStoreModelVersionChecksumKey: String

