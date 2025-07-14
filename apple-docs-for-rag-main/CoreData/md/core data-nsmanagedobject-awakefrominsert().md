

- Core Data
- NSManagedObject
-  awakeFromInsert() 

Instance Method

# awakeFromInsert()

Provides an opportunity to add code into the life cycle of the managed object when initially creating it.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func awakeFromInsert()
```

## Discussion

You typically use this method to initialize special default property values. This method is invoked only once in the object’s lifetime.

If you want to set attribute values in an implementation of this method, you should typically use primitive accessor methods (either setPrimitiveValue(_:forKey:) or—better—the appropriate custom primitive accessors). This ensures that the new values are treated as baseline values rather than being recorded as undoable changes for the properties in question.

Important

Subclasses must invoke super’s implementation before performing their own initialization.

### Special Considerations

If you create a managed object then perform undo operations to bring the managed object context to a state prior to the object’s creation, then perform redo operations to bring the managed object context back to a state after the object’s creation, awakeFromInsert() is *not* invoked a second time.

You are typically discouraged from performing fetches within an implementation of awakeFromInsert(). Although it is allowed, execution of the fetch request can trigger the sending of internal Core Data notifications which may have unwanted side-effects. For example, in macOS, an instance of NSArrayController may end up inserting a new object into its content array twice.

## See Also

### Managing Change Events

class var contextShouldIgnoreUnmodeledPropertyChanges: Bool

A Boolean value that indicates whether to mark instances of the class as having changes when an unmodeled property changes.

func awakeFromFetch()

Provides an opportunity to add code into the life cycle of the managed object when fufilling it from a fault.

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

class func fetchRequest() -> NSFetchRequest&lt;any NSFetchRequestResult>

Returns an initialized fetch request with the entity this subclass represents.

