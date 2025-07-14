

- Core Data
-  NSManagedObjectModel 

Class

# NSManagedObjectModel

A programmatic representation of the `.xcdatamodeld` file describing your objects.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class NSManagedObjectModel
```

## Mentioned in 

Setting up a Core Data stack manually

Setting up a Core Data stack

## Overview

The model contains one or more `NSEntityDescription` objects representing the entities in the schema. Each `NSEntityDescription` object has property description objects (instances of subclasses of NSPropertyDescription) that represent the properties (or fields) of the entity in the schema. The Core Data framework uses this description in several ways:

- Constraining UI creation in Interface Builder

- Validating attribute and relationship values at runtime

- Mapping between your managed objects and a database or file-based schema for object persistence

A managed object model maintains a mapping between each of its entity objects and a corresponding managed object class for use with the persistent storage mechanisms in the Core Data framework. You can determine the entity for a particular managed object with the `entity` method.

You typically create managed object models using the data modeling tool in Xcode, but it’s possible to build a model programmatically if needed.

### Loading a model file

Managed object model files are typically stored in a project or a framework. To load a model, you provide an URL to the constructor. Note that loading a model doesn’t have the effect of loading all of its entities.

### Storing fetch requests

Frequently, you need a collection of objects that share features in common. Sometimes you can define those features (property values) in advance; sometimes you need to be able to supply values at runtime. For example, suppose you want to retrieve all movies owned by Pixar, or retrieve all movies that earned more than an amount specified by the user at runtime.

Fetch requests are often predefined in a managed object model as templates. They allow you to predefine named queries and their parameters in the model. Typically they contain variables that need to be substituted at runtime. `NSManagedObjectModel` provides an API to retrieve a stored fetch request by name, and to perform variable substitution—see fetchRequestTemplate(forName:) and fetchRequestFromTemplate(withName:substitutionVariables:).

You typically define fetch request templates using the Data Model editor in Xcode. You can also create fetch request templates programmatically, and associate them with a model using setFetchRequestTemplate(_:forName:).

### Supporting multiple configurations for the same model

You may want to specify different sets of entities for the same model to be used in different situations. For example, suppose certain entities should only be available if a user has administrative privileges. To support this requirement, a model may have more than one configuration. Each configuration is named, and has an associated set of entities. The sets may overlap. You establish configurations programmatically using setEntities(_:forConfigurationName:) or using the Xcode design tool, and retrieve the entities for a given configuration name using entities(forConfigurationName:).

### Changing models

Because a model describes the structure of the data in a persistent store, changing any parts of a model that alters the schema renders it incompatible with (and so unable to open) the stores it previously created. If you change your schema, you therefore need to migrate the data in existing stores to new version (see Core Data Model Versioning and Data Migration Programming Guide). For example, if you add a new entity or a new attribute to an existing entity, you *can’t* open old stores; if you add a validation constraint or set a new default value for an attribute, you *can* open old stores.

### Editing models at runtime

Managed object models are editable until they are used by an object graph manager (a managed object context or a persistent store coordinator). This allows you to create or modify them dynamically until their first use. However, once a model is being used, it *must not* be changed. This is enforced at runtime—when the object manager first fetches data using a model, the whole of that model becomes uneditable. Any attempt to mutate a model or any of its sub-objects after that point throws an exception. If you need to modify a model that’s in use, create a copy, modify the copy, and then discard the objects with the old model.

### Enumerating entities with fast enumeration

In macOS 10.5 and later and on iOS, `NSManagedObjectModel` supports the NSFastEnumeration protocol. You can use this to enumerate over a model’s entities, as illustrated in the following example:

```
NSManagedObjectModel *aModel = ...;
for (NSEntityDescription *entity in aModel) {
    // entity is each instance of NSEntityDescription in aModel in turn
}
```

## Topics

### Creating a managed object model

convenience init?(contentsOf: URL)

Initializes the managed object model using the model file at the specified URL.

init()

Initializes an empty managed object model.

class func mergedModel(from: [Bundle]?) -> NSManagedObjectModel?

Returns a model created by merging all the models found in given bundles.

class func mergedModel(from: [Bundle]?, forStoreMetadata: [String : Any]) -> NSManagedObjectModel?

Returns a merged model from a specified array for the version information in provided metadata.

init?(byMerging: [NSManagedObjectModel]?)

Creates a single model from an array of existing models.

init?(byMerging: [NSManagedObjectModel], forStoreMetadata: [String : Any])

Returns, for the version information in given metadata, a model merged from a given array of models.

### Managing entities and configurations

var entities: [NSEntityDescription]

The entities in the model.

var entitiesByName: [String : NSEntityDescription]

The entities of the model, keyed by name.

var configurations: [String]

All the available configuration names of the model.

func entities(forConfigurationName: String?) -> [NSEntityDescription]?

Returns the entities of the model for a specified configuration.

func setEntities([NSEntityDescription], forConfigurationName: String)

Associates the specified entities with the model using the given configuration name.

### Manipulating fetch request templates

var fetchRequestTemplatesByName: [String : NSFetchRequest&lt;any NSFetchRequestResult>]

A dictionary of the receiver’s fetch request templates, keyed by name.

func fetchRequestTemplate(forName: String) -> NSFetchRequest&lt;any NSFetchRequestResult>?

Returns the fetch request with a specified name.

func fetchRequestFromTemplate(withName: String, substitutionVariables: [String : Any]) -> NSFetchRequest&lt;any NSFetchRequestResult>?

Returns a copy of the fetch request template with the variables substituted by values from the substitutions dictionary.

func setFetchRequestTemplate(NSFetchRequest&lt;any NSFetchRequestResult>?, forName: String)

Associates the specified fetch request with the receiver using the given name.

### Handling localization

var localizationDictionary: [String : String]?

The localization dictionary of the model.

### Versioning and migrating entities

var versionChecksum: String

The Base64-encoded 128-bit model version hash.

var versionIdentifiers: Set&lt;AnyHashable>

The set of developer-defined version identifiers for the object model.

var entityVersionHashesByName: [String : Data]

The dictionary of the model’s entity names and their corresponding version hashes.

func isConfiguration(withName: String?, compatibleWithStoreMetadata: [String : Any]) -> Bool

Returns a Boolean value that indicates whether a given configuration in the model is compatible with given metadata from a persistent store.

### Working with indexes

enum NSFetchIndexElementType

Defines the possible types of index elements.

class NSFetchIndexDescription

The description of the index.

class NSFetchIndexElementDescription

Description of an Index Element

### Instance Methods

func makeManagedObjectModel(for: Schema, mergedWith: NSManagedObjectModel?) -> NSManagedObjectModel?

### Type Methods

static func makeManagedObjectModel(for: [any PersistentModel.Type], mergedWith: NSManagedObjectModel?) -> NSManagedObjectModel?

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSFastEnumeration
- NSObjectProtocol

## See Also

### Object Modeling

class NSEntityDescription

A description of a Core Data entity.

class NSPropertyDescription

A description of a single property belonging to an entity.

class NSAttributeDescription

A description of a single attribute belonging to an entity.

class NSDerivedAttributeDescription

A description of an attribute that derives its value by performing a calculation on a related attribute.

class NSRelationshipDescription

A description of a relationship between two entities.

