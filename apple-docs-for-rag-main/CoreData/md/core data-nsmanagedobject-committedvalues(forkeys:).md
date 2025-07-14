

- Core Data
- NSManagedObject
-  committedValues(forKeys:) 

Instance Method

# committedValues(forKeys:)

Returns a dictionary of the most recent fetched or saved values of the managed object for the properties of the specified keys.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func committedValues(forKeys keys: [String]?) -> [String : Any]
```

## Parameters 

`keys`  

An array containing names of properties of the receiver, or `nil`.

## Return Value

A dictionary containing the last fetched or saved values of the receiver for the properties specified by `keys`.

## Discussion

`nil` values are represented by an instance of NSNull.

This method only reports values of properties that are defined as persistent properties of the receiver, not values of transient properties or of custom instance variables.

You can invoke this method with the `keys` value of `nil` to retrieve committed values for all the receiver’s properties, as illustrated by the following example.

```
NSDictionary *allCommittedValues =
        [aManagedObject committedValuesForKeys:nil];
```

It is more efficient to use `nil` than to pass an array of all the property keys.

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

