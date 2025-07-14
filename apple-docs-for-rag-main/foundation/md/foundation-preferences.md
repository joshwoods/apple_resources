

- Foundation
-  Preferences 

API Collection

# Preferences

Persistently store domain-scoped pieces of information for configuring your app.

## Topics

### App-Specific Data

class UserDefaults

An interface to the user’s defaults database, where you store key-value pairs persistently across launches of your app.

### Shared Data

class NSUbiquitousKeyValueStore

An iCloud-based container of key-value pairs you use to share data among instances of your app running on a user’s connected devices.

## See Also

### Files and Data Persistence

File System

Create, read, write, and examine files and folders in the file system.

Archives and Serialization

Convert objects and values to and from property list, JSON, and other flat binary representations.

Spotlight

Search for files and other items on the local device, and index your app’s content for searching.

iCloud

Manage files and key-value data that automatically synchronize among a user’s iCloud devices.

Optimizing Your App’s Data for iCloud Backup

Minimize the space and time that backups take to create by excluding purgeable and nonpurgeable data from backups.

