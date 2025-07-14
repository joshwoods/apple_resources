

- Bundle Resources
- Information Property List
-  Data and storage 

API Collection

# Data and storage

Regulate documents, URLs, and other kinds of data movement and storage.

## Overview

The system needs to know what kinds of data your app stores, provides, or consumes. Add keys to your app’s Information Property List that declare your app’s data management capabilities.

## Topics

### Documents

CFBundleDocumentTypes

The document types supported by the bundle.

**Name:** Document types

UISupportsDocumentBrowser

A Boolean value indicating whether the app is a document-based app.

**Name:** Supports Document Browser

LSSupportsOpeningDocumentsInPlace

A Boolean value indicating whether the app may open the original document from a file provider, rather than a copy of the document.

**Name:** Supports opening documents in place

NSDownloadsUbiquitousContents

A Boolean value that indicates whether the system should download documents before handing them over to the app.

### URL schemes

CFBundleURLTypes

A list of URL schemes (http, ftp, and so on) supported by the app.

**Name:** URL types

### Universal type identifiers

UTExportedTypeDeclarations

The uniform type identifiers owned and exported by the app.

**Name:** Exported Type UTIs

UTImportedTypeDeclarations

The uniform type identifiers inherently supported, but not owned, by the app.

**Name:** Imported Type UTIs

### Network

NSAdvertisingAttributionReportEndpoint

The URL where Private Click Measurement and SKAdNetwork send attribution information.

NSAppTransportSecurity

A description of changes made to the default security for HTTP connections.

**Name:** App Transport Security Settings

NSBonjourServices

Bonjour service types browsed by the app.

**Name:** Bonjour services

CKSharingSupported

A Boolean value that indicates your app supports CloudKit Sharing.

### Background downloads

BAInitialDownloadRestrictions

The restrictions that apply to the set of assets that download immediately after app installation.

BAMaxInstallSize

The combined, maximum size, in bytes, of the non-essential assets that download immediately after app installation.

BAManifestURL

The location URL of the app’s manifest file that contains the names and sizes of assets.

BAEssentialMaxInstallSize

The combined, maximum size of the essential assets that the system downloads before it launches your app in bytes.

### Storage

APFiles

Describes the files or directories the app installs on the system.

**Name:** Installation files

APInstallerURL

The base path to the files or folders that the app installs.

**Name:** Installation directory base file URL

NSSupportsPurgeableLocalStorage

A Boolean value indicating whether the app continues working if the system purges the local storage.

LSFileQuarantineEnabled

A Boolean value indicating whether the files this app creates are quarantined by default.

**Name:** File quarantine enabled

UIFileSharingEnabled

A Boolean value indicating whether the app shares files.

**Name:** Application supports iTunes file sharing

CSResourcesFileMapped

A Boolean value indicating whether the app’s resources files should be mapped into memory.

**Name:** Resources should be file-mapped

NSDownloadsUbiquitousContents

A Boolean value that indicates whether the system should download documents before handing them over to the app.

### CoreML models

LSBundleContainsCoreMLmlmodelc

A Boolean value indicating whether the app contains a Core ML model to optimize loading the model.

**Name:** Bundle contains CoreML models

### Java

NSJavaRoot

The root directory for the app’s Java class files.

**Name:** Java root directory

## See Also

### Services

Protected resources

Control an app’s access to protected system services and user data.

App services

Configure services provided by the app, like support for giving directions or using game controllers.

Kernel and drivers

Configure device drivers provided by the app.

