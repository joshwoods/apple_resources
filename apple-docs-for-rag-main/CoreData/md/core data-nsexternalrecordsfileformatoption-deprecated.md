

- Core Data
-  NSExternalRecordsFileFormatOption Deprecated

Global Variable

# NSExternalRecordsFileFormatOption

Option to specify the file format of a Spotlight external records.

macOS 10.6–10.13Deprecated

``` source
let NSExternalRecordsFileFormatOption: String
```

Deprecated

Spotlight integration is deprecated. Use CoreSpotlight integration instead.

## Discussion

For possible values, see `Format Options for Spotlight External Record Files`.

## See Also

### Deprecated

let NSExternalRecordsDirectoryOption: String

Option indicating the directory where Spotlight external record files should be written to.

Deprecated

let NSExternalRecordExtensionOption: String

Option indicating the file extension to use for Spotlight external record files.

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

let NSPersistentStoreRemoveUbiquitousMetadataOption: String

The corresponding value is an `NSNumber` object representing a boolean that indicates whether the receiver should remove all associated ubiquity metadata from a persistent store. You typically use this option during migration or copying to disassociate a persistent store file from an iCloud account.

Deprecated

let NSPersistentStoreUbiquitousContainerIdentifierKey: String

The a string specifying the iCloud container identifier.

Deprecated

let NSPersistentStoreRebuildFromUbiquitousContentOption: String

The corresponding value is an `NSNumber` object representing a boolean that indicates whether the receiver should erase the local store file and rebuild it from the iCloud data in Mobile Documents.

Deprecated

