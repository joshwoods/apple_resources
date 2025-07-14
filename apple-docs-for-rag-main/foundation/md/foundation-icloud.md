

- Foundation
-  iCloud 

API Collection

# iCloud

Manage files and key-value data that automatically synchronize among a user’s iCloud devices.

## Topics

### iCloud Storage

class FileManager

A convenient interface to the contents of the file system, and the primary means of interacting with it.

protocol FileManagerDelegate

The interface a file manager’s delegate uses to intervene during operations or if an error occurs.

### App Preferences

class NSUbiquitousKeyValueStore

An iCloud-based container of key-value pairs you use to share data among instances of your app running on a user’s connected devices.

### File Search

class NSMetadataQuery

A query that you perform against Spotlight metadata.

protocol NSMetadataQueryDelegate

An interface that enables the delegate of a metadata query to provide substitute results or attributes.

class NSMetadataItem

The metadata associated with a file.

### Entitlements

com.apple.developer.icloud-container-development-container-identifiers

The container identifiers for the iCloud development environment.

com.apple.developer.icloud-container-environment

The development or production environment to use for the iCloud containers.

iCloud Container Identifiers Entitlement

The container identifiers for the iCloud production environment.

iCloud Services Entitlement

The iCloud services used by the app.

iCloud Key-Value Store Entitlement

The container identifier to use for iCloud key-value storage.

### Errors

iCloud Error Codes

Error codes to expect when an iCloud-related error occurs.

## See Also

### Files and Data Persistence

File System

Create, read, write, and examine files and folders in the file system.

Archives and Serialization

Convert objects and values to and from property list, JSON, and other flat binary representations.

Preferences

Persistently store domain-scoped pieces of information for configuring your app.

Spotlight

Search for files and other items on the local device, and index your app’s content for searching.

Optimizing Your App’s Data for iCloud Backup

Minimize the space and time that backups take to create by excluding purgeable and nonpurgeable data from backups.

