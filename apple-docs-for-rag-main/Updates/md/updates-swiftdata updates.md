

- Updates
-  SwiftData updates 

Article

# SwiftData updates

Learn about important changes to SwiftData.

## Overview

Browse notable changes in SwiftData.

## June 2024

### Macros

- Improve performance of sorts and predicate-based fetches by using the Index(_:) macro to define individual and compound indexes.

- Define a unique constraint that includes one or more model attributes using the Unique(_:) macro, enabling SwiftData to regard tuples of attributes as unique.

- Specify `nil` as a relationship’s `inverse` to create a unidirectional relationship.

### Persistent history

- Fetch historical changes for one or more persistent models using the model context’s fetchHistory(_:) method.

- Delete stale model history from a persistent store by calling the context’s deleteHistory(_:) method.

- Provide an alternate change tracking strategy for your custom persistent store by adopting the doc://com.apple.documentation/documentation/swiftdata/history/historyproviding protocol.

### Custom persistent stores

- Adopt the DataStore protocol (and related protocols) to provide custom storage for your app’s persistent models.

## See Also

### Technology updates

Accelerate updates

Learn about important changes to Accelerate.

Accessibility updates

Learn about important changes to Accessibility.

ActivityKit updates

Learn about important changes in ActivityKit.

AdAttributionKit Updates

Learn about important changes to AdAttributionKit.

App Intents updates

Learn about important changes in App Intents.

AppKit updates

Learn about important changes to AppKit.

Apple Intelligence updates

Learn about important changes to Apple Intelligence.

Apple Pencil updates

Learn about important changes to Apple Pencil.

ARKit updates

Learn about important changes to ARKit.

Audio Toolbox updates

Learn about important changes to Audio Toolbox.

AuthenticationServices updates

Learn about important changes to AuthenticationServices.

AVFAudio updates

Learn about important changes to AVFAudio.

AVFoundation updates

Learn about important changes to AVFoundation.

Bundle Resources updates

Learn about important changes to Bundle Resources.

ContactsUI updates

Learn about important changes to ContactsUI.

