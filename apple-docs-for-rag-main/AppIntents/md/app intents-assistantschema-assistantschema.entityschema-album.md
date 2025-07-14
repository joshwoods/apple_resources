

- App Intents
- AssistantSchema
- AssistantSchema.EntitySchema
-  album 

Instance Property

# album

The app entity describes an album.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var album: some AssistantSchemas.Entity { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app entity implementation.

For more information about the `.photos` app intent domain, see Making photo and video actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app entity that conforms to the `.photos.album` schema:

```
@AssistantEntity(schema: .photos.album)
struct PhotoAlbumEntity: AppEntity {
    struct Query: EntityStringQuery {
        func entities(for identifiers: [PhotoAlbumEntity.ID]) async throws -> [PhotoAlbumEntity] { [] }
        func entities(matching string: String) async throws -> [PhotoAlbumEntity] { [] }
    }

    static var defaultQuery = Query()
    var displayRepresentation: DisplayRepresentation { "Photo Album" }

    let id = UUID()

    @Property
    var name: String

    @Property
    var creationDate: Date?

    @Property
    var albumType: PhotoAlbumType
}
```

