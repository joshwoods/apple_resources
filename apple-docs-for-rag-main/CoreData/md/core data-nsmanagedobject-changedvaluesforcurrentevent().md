

- Core Data
- NSManagedObject
-  changedValuesForCurrentEvent() 

Instance Method

# changedValuesForCurrentEvent()

Returns a dictionary containing the keys and new values of persistent properties with changes since the last fetching or saving of the managed object.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func changedValuesForCurrentEvent() -> [String : Any]
```

## Return Value

A dictionary with keys that are the names of persistent properties with changes since the last posting of NSManagedObjectContextObjectsDidChange, and with the new values for those properties.

## Discussion

This method only reports changes to properties that are persistent properties of the receiver, not changes to transient properties or custom instance variables.

Note

In Objective-C, this method returns the keys and values of persistent properties with changes since the last posting of NSManagedObjectContextObjectsDidChangeNotification.

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

class func fetchRequest() -> NSFetchRequest&lt;any NSFetchRequestResult>

Returns an initialized fetch request with the entity this subclass represents.

