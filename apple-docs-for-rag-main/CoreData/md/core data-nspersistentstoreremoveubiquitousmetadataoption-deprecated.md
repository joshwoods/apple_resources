

- Core Data
-  NSPersistentStoreRemoveUbiquitousMetadataOption Deprecated

Global Variable

# NSPersistentStoreRemoveUbiquitousMetadataOption

The corresponding value is an `NSNumber` object representing a boolean that indicates whether the receiver should remove all associated ubiquity metadata from a persistent store. You typically use this option during migration or copying to disassociate a persistent store file from an iCloud account.

iOS 7.0–10.0DeprecatediPadOS 7.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.12DeprecatedvisionOS 1.0–1.0Deprecated

``` source
let NSPersistentStoreRemoveUbiquitousMetadataOption: String
```

Deprecated

Please see the release notes and Core Data documentation.

## See Also

### Deprecated

let NSExternalRecordsDirectoryOption: String

Option indicating the directory where Spotlight external record files should be written to.

Deprecated

let NSExternalRecordExtensionOption: String

Option indicating the file extension to use for Spotlight external record files.

Deprecated

let NSExternalRecordsFileFormatOption: String

Option to specify the file format of a Spotlight external records.

Deprecated

let NSPersistentStoreUbiquitousContentNameKey: String

Option to specify that a persistent store has a given name in ubiquity.

Deprecated

let NSPersistentStoreUbiquitousContentURLKey: String

Option to specify the log path to use for ubiquitous content logs.

Deprecated

let NSPersistentStoreUbiquitousPeerTokenOption: String

The corresponding value is an optionally specified string which will be mixed in to Core Data’s identifier for each iCloud peer. The value must be an alphanumeric string without any special characters, whitespace or punctuation. The primary use for this option is to allow multiple applications on the same peer (device) to share a Core Data store integrated with iCloud. Each application will require its own store file.

Deprecated

let NSPersistentStoreUbiquitousContainerIdentifierKey: String

The a string specifying the iCloud container identifier.

Deprecated

let NSPersistentStoreRebuildFromUbiquitousContentOption: String

The corresponding value is an `NSNumber` object representing a boolean that indicates whether the receiver should erase the local store file and rebuild it from the iCloud data in Mobile Documents.

Deprecated

