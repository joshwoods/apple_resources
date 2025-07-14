

- App Store Connect API
- App Store
-  App Encryption Declarations 

API Collection

# App Encryption Declarations

View, and assign to builds, the declarations about types of encryption used in your app.

## Overview

To comply with regulatory requirements, you sometimes need to provide information and supporting documentation in the form of declarations about the types of encryption used by your app. The app encryption declarations resource represents this information, and enables you to:

- View information about the declaration, and

- Assign the declaration to a build.

- Create app encryption declarations in App Store Connect.

- Upload app encryption declaration documents.

Note

Builds that have the `usesNonExemptEncryption` flag set to true in the app’s property list must link to an app encryption declaration before the app can be submitted for beta app review.

For more information, see Overview of export compliance.

## Topics

### Getting App Encryption Declarations

List App Encryption Declarations

Find and list all available app encryption declarations.

Read App Encryption Declaration Information

Get information about a specific app encryption declaration.

Read the App Information of an App Encryption Declaration

Get the app information from a specific app encryption declaration.

Deprecated

Read a specific App Encryption Declaration Document

Get detailed information about a specified App Encryption Declaration document.

Read the Declaration Document for an App Encryption Declaration

Read the associate document for a specific App Encryption Declaration.

### Assigning App Encryption Declarations

Create an app encryption declarations

Add an app encryption delcaration for a specific app.

Assign Builds to an App Encryption Declaration

Assign one or more builds to an app encryption declaration.

Deprecated

### Uploading App Encryption Declaration Documents

Upload an App Encryption Declaration Document

Add an App Encryption Declaration Document to an existing App Encryption Declaration.

Modify an App Encryption Declaration Document

Commit an App Encryption Declaration Document after uploading it.

### Objects and Data Types

object AppEncryptionDeclarationCreateRequest

The request body you use to create an app encryption declaration.

object AppEncryptionDeclarationDocument

object AppEncryptionDeclarationDocumentCreateRequest

object AppEncryptionDeclarationDocumentResponse

object AppEncryptionDeclarationDocumentUpdateRequest

object AppEncryptionDeclaration

The data structure that represents an App Encryption Declarations resource.

object AppEncryptionDeclarationBuildsLinkagesRequest

A request body you use to add builds to an app encryption declaration.

Deprecated

object AppEncryptionDeclarationResponse

A response that contains a single App Encryption Declarations resource.

object AppEncryptionDeclarationWithoutIncludesResponse

object AppEncryptionDeclarationsResponse

A response that contains a list of App Encryption Declaration resources.

type AppEncryptionDeclarationState

Strings that represent the review or acceptance status of an app encryption declaration submitted to Apple.

## See Also

### Builds

Builds

Manage builds for testers and submit builds for review.

Build Bundles

Read metadata for app and App Clip binaries included in a build you upload to App Store Connect.

Build Icons

Get icons from your app’s binary that are uploaded to App Store.

