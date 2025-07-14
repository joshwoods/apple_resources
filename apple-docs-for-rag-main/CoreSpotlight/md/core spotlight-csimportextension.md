

- Core Spotlight
-  CSImportExtension 

Class

# CSImportExtension

An object that provides searchable attributes for file types that the app supports.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
class CSImportExtension
```

## Overview

To create a Spotlight File Importer extension, add a target to your app using the Spotlight File Importer template in Xcode. The template project contains a subclass of `CSImportExtension`. To index content on a user’s device, Core Spotlight loads your extension and invokes the update(_:forFileAt:) method. Core Spotlight passes a CSSearchableItemAttributeSet and URL of a file to the extension, and you set properties that are relevant for the file.

Typically, your extension loads details about the file and uses that information to set properties of the attribute set. For example, if your app contains files that are notes the user creates, it does the following:

```
class NoteImporter: CSImportExtension {
    override func update(_ attributes: CSSearchableItemAttributeSet, forFileAt contentURL: URL) throws {
        // NoteDetails is an app-defined object that encapsulates a note.
        guard let note = NoteDetails.noteDetails(for: contentURL) else {
            throw NoteError.noteNotFound
        }
        attributes.title = note.title
        attributes.contentCreationDate = note.creationDate
        attributes.userCreated = NSNumber(booleanLiteral: true)
    }
}
```

Important

Core Spotlight indexes files in batches and may call update(_:forFileAt:) simultaneously on multiple queues with different values of `contentURL`.

To specify the file types your app supports, set the value of CSSupportedContentTypes in your extension’s `Info.plist` file to an array of file type identifiers. For more information about file type identifiers, see Uniform Type Identifiers. The app in the previous example configures the extension’s `Info.plist` as follows:

```
NSExtension

    NSExtensionPointIdentifier
    com.apple.spotlight.import
    NSExtensionPrincipalClass
    FileImporter
    NSExtensionAttributes

        CSSupportedContentTypes

            com.example.mynoteapp.note

```

## Topics

### Providing searchable attributes

func update(CSSearchableItemAttributeSet, forFileAt: URL) throws

Provides searchable attributes for a file at the specified URL.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSExtensionRequestHandling
- NSObjectProtocol

## See Also

### Spotlight app extensions

Regenerating your app’s indexes on demand

Create an app extension to maintain your app’s indexes and regenerate them as needed.

class CSIndexExtensionRequestHandler

An interface that implements an index-maintenance app extension.

