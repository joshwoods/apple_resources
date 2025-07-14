

- SwiftUI
- View fundamentals
- View
-  State modifiers 

API Collection

# State modifiers

Access storage and provide child views with configuration data.

## Overview

SwiftUI provides tools for managing data in your app. For example, you can store values and objects in an environment that’s shared among the views in a view hierarchy. Any view that shares the environment — typically all the descendant views of the view that stores the item — can then access the stored item.

For more information about the types that SwiftUI provides to help manage data in your app, see Model data.

## Topics

### Identity

func tag&lt;V>(V, includeOptional: Bool) -> some View

Sets the unique tag value of this view.

func id&lt;ID>(ID) -> some View

Binds a view’s identity to the given proxy value.

func equatable() -> EquatableView&lt;Self>

Prevents the view from updating its child view when its new value is the same as its old value.

### Environment values

func environment&lt;T>(T?) -> some View

Places an observable object in the view’s environment.

func environment&lt;V>(WritableKeyPath&lt;EnvironmentValues, V>, V) -> some View

Sets the environment value of the specified key path to the given value.

func environmentObject&lt;T>(T) -> some View

Supplies an observable object to a view’s hierarchy.

func transformEnvironment&lt;V>(WritableKeyPath&lt;EnvironmentValues, V>, transform: (inout V) -> Void) -> some View

Transforms the environment value of the specified key path with the given function.

### Preferences

func preference&lt;K>(key: K.Type, value: K.Value) -> some View

Sets a value for the given preference.

func transformPreference&lt;K>(K.Type, (inout K.Value) -> Void) -> some View

Applies a transformation to a preference value.

func anchorPreference&lt;A, K>(key: K.Type, value: Anchor&lt;A>.Source, transform: (Anchor&lt;A>) -> K.Value) -> some View

Sets a value for the specified preference key, the value is a function of a geometry value tied to the current coordinate space, allowing readers of the value to convert the geometry to their local coordinates.

func transformAnchorPreference&lt;A, K>(key: K.Type, value: Anchor&lt;A>.Source, transform: (inout K.Value, Anchor&lt;A>) -> Void) -> some View

Sets a value for the specified preference key, the value is a function of the key’s current value and a geometry value tied to the current coordinate space, allowing readers of the value to convert the geometry to their local coordinates.

func onPreferenceChange&lt;K>(K.Type, perform: (K.Value) -> Void) -> some View

Adds an action to perform when the specified preference key’s value changes.

func backgroundPreferenceValue&lt;Key, T>(Key.Type, (Key.Value) -> T) -> some View

Reads the specified preference value from the view, using it to produce a second view that is applied as the background of the original view.

func backgroundPreferenceValue&lt;K, V>(K.Type, alignment: Alignment, (K.Value) -> V) -> some View

Reads the specified preference value from the view, using it to produce a second view that is applied as the background of the original view.

func overlayPreferenceValue&lt;Key, T>(Key.Type, (Key.Value) -> T) -> some View

Reads the specified preference value from the view, using it to produce a second view that is applied as an overlay to the original view.

func overlayPreferenceValue&lt;K, V>(K.Type, alignment: Alignment, (K.Value) -> V) -> some View

Reads the specified preference value from the view, using it to produce a second view that is applied as an overlay to the original view.

### Default storage

func defaultAppStorage(UserDefaults) -> some View

The default store used by `AppStorage` contained within the view.

### Configuring a model

func modelContext(ModelContext) -> some View

Sets the model context in this view’s environment.

func modelContainer(ModelContainer) -> some View

Sets the model container and associated model context in this view’s environment.

func modelContainer(for:inMemory:isAutosaveEnabled:isUndoEnabled:onSetup:)

Sets the model container in this view for storing the provided model type, creating a new container if necessary, and also sets a model context for that container in this view’s environment.

## See Also

### Providing interactivity

Input and event modifiers

Supply actions for a view to perform in response to user input and system events.

Search modifiers

Enable people to search for content in your app.

Presentation modifiers

Define additional views for the view to present under specified conditions.

