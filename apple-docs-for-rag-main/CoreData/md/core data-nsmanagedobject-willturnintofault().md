

- Core Data
- NSManagedObject
-  willTurnIntoFault() 

Instance Method

# willTurnIntoFault()

Provides an opportunity to add code into the life cycle of the managed object before converting it to a fault.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func willTurnIntoFault()
```

## Discussion

This method is the companion of the didTurnIntoFault() method. You can use it to (re)set state which requires access to property values (for example, observers across key paths). The default implementation does nothing.

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

func didTurnIntoFault()

Provides an opportunity to add code into the life cycle of the managed object after converting it to a fault.

class func fetchRequest() -> NSFetchRequest&lt;any NSFetchRequestResult>

Returns an initialized fetch request with the entity this subclass represents.

