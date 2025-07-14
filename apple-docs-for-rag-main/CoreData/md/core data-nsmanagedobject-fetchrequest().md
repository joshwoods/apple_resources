

- Core Data
- NSManagedObject
-  fetchRequest() 

Type Method

# fetchRequest()

Returns an initialized fetch request with the entity this subclass represents.

iOS 10.0+iPadOS 10.0+Mac CatalystmacOS 10.12+tvOS 10.0+visionOSwatchOS 3.0+

``` source
@objc
dynamic class func fetchRequest() -> NSFetchRequest
```

## Discussion

This method is only legal to call on subclasses of `NSManagedObject` that represent a single entity in the model.

## See Also

### Managing Change Events

class var contextShouldIgnoreUnmodeledPropertyChanges: Bool

A Boolean value that indicates whether to mark instances of the class as having changes when an unmodeled property changes.

func awakeFromFetch()

Provides an opportunity to add code into the life cycle of the managed object when fufilling it from a fault.

func awakeFromInsert()

Provides an opportunity to add code into the life cycle of the managed object when initially creating it.

func awake(fromSnapshotEvents: NSSnapshotEventType)

Provides an opportunity to add code into the life cycle of the managed object when fulfilling it from a snapshot.

func changedValues() -> [String : Any]

Returns a dictionary containing the keys and new values of persistent properties with changes since the last fetching or saving of the managed object.

func changedValuesForCurrentEvent() -> [String : Any]

Returns a dictionary containing the keys and new values of persistent properties with changes since the last fetching or saving of the managed object.

func committedValues(forKeys: [String]?) -> [String : Any]

Returns a dictionary of the most recent fetched or saved values of the managed object for the properties of the specified keys.

func prepareForDeletion()

Provides an opportunity to add code into the life cycle of the managed object before deleting it.

func willSave()

Provides an opportunity to add code into the life cycle of the managed object before saving it.

func didSave()

Provides an opportunity to add code into the life cycle of the managed object after the managed object’s context completes a save operation.

func willTurnIntoFault()

Provides an opportunity to add code into the life cycle of the managed object before converting it to a fault.

func didTurnIntoFault()

Provides an opportunity to add code into the life cycle of the managed object after converting it to a fault.

