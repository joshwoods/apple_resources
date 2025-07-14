

- SwiftData
-  Index(\_:) 

Macro

# Index(\_:)

Specifies the key-paths that SwiftData uses to create one or more binary indices for the associated model.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+Swift 5.9+

``` source
@freestanding(declaration)
macro Index(_ indices: [PartialKeyPath]...) where T : PersistentModel
```

## See Also

### Model definition

macro Model()

Converts a Swift class into a stored model that’s managed by SwiftData.

macro Attribute(Schema.Attribute.Option..., originalName: String?, hashModifier: String?)

Specifies the custom behavior that SwiftData applies to the annotated property when managing the owning class.

macro Unique&lt;T>([PartialKeyPath&lt;T>]...)

Specifies the key-paths that SwiftData uses to enforce the uniqueness of model instances.

macro Index&lt;T>(Schema.Index&lt;T>.Types&lt;T>...)

Specifies the key-paths that SwiftData uses to create one or more indicies for the associated model, where each index is either binary or R-tree.

Defining data relationships with enumerations and model classes

Create relationships for static and dynamic data stored in your app.

macro Relationship(Schema.Relationship.Option..., deleteRule: Schema.Relationship.DeleteRule, minimumModelCount: Int?, maximumModelCount: Int?, originalName: String?, inverse: AnyKeyPath?, hashModifier: String?)

Specifies the options that SwiftData needs to manage the annotated property as a relationship between two models.

macro Transient()

Tells SwiftData not to persist the annotated property when managing the owning class.

