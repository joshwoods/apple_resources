

- SwiftUI
-  Persistent storage 

API Collection

# Persistent storage

Store data for use across sessions of your app.

## Overview

The operating system provides ways to store data when your app closes, so that when people open your app again later, they can continue working without interruption. The mechanism that you use depends on factors like what and how much you need to store, whether you need serialized or random access to the data, and so on.

You use the same kinds of storage in a SwiftUI app that you use in any other app. For example, you can access files on disk using the FileManager interface. However, SwiftUI also provides conveniences that make it easier to use certain kinds of persistent storage in a declarative environment. For example, you can use FetchRequest and FetchedResults to interact with a Core Data model.

## Topics

### Saving state across app launches

Restoring Your App’s State with SwiftUI

Provide app continuity for users by preserving their current activities.

func defaultAppStorage(UserDefaults) -> some View

The default store used by `AppStorage` contained within the view.

struct AppStorage

A property wrapper type that reflects a value from `UserDefaults` and invalidates a view on a change in value in that user default.

struct SceneStorage

A property wrapper type that reads and writes to persisted, per-scene storage.

### Accessing Core Data

Loading and Displaying a Large Data Feed

Consume data in the background, and lower memory use by batching imports and preventing duplicate records.

var managedObjectContext: NSManagedObjectContext

struct FetchRequest

A property wrapper type that retrieves entities from a Core Data persistent store.

struct FetchedResults

A collection of results retrieved from a Core Data store.

struct SectionedFetchRequest

A property wrapper type that retrieves entities, grouped into sections, from a Core Data persistent store.

struct SectionedFetchResults

A collection of results retrieved from a Core Data persistent store, grouped into sections.

## See Also

### Data and storage

Model data

Manage the data that your app uses to drive its interface.

Environment values

Share data throughout a view hierarchy using the environment.

Preferences

Indicate configuration preferences from views to their container views.

