

- App Intents
- AssistantSchemas
- AssistantSchemas.EnumSchema
-  assetType 

Instance Property

# assetType

The type of asset.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var assetType: some AssistantSchemas.Enum { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app enum implementation.

For more information about the `.photos` app intent domain, see Making photo and video actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app enum that conforms to the `.photos.assetType` schema:

```
@AssistantEnum(schema: .photos.assetType)
enum PhotoAssetType: AppEnum {
    case photo
    case video

    static var caseDisplayRepresentations: [PhotoAssetType: AppIntents.DisplayRepresentation] = [
        .photo: "Photo",
        .video: "Video",
    ]
}
```

