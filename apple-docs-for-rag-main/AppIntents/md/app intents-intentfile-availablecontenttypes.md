

- App Intents
- IntentFile
-  availableContentTypes 

Instance Property

# availableContentTypes

Valid content types the `IntentFile` can possibly be converted to.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var availableContentTypes: [UTType] { get }
```

## Discussion

Use these content types to request an `IntentFile` representation as either a file url or data.

