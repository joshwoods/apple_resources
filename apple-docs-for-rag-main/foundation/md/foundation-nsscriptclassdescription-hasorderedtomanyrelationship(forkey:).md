

- Foundation
- NSScriptClassDescription
-  hasOrderedToManyRelationship(forKey:) 

Instance Method

# hasOrderedToManyRelationship(forKey:)

Returns a Boolean value indicating whether the described class has an ordered to-many relationship identified by the specified key.

macOS 10.5+

``` source
func hasOrderedToManyRelationship(forKey key: String) -> Bool
```

## Parameters 

`key`  

The identifying key for a property of the receiver.

## Return Value

true if the described class has an ordered to-many relationship identified by the specified key; otherwise, false.

## See Also

### Getting attribute and relationship information

func hasProperty(forKey: String) -> Bool

Returns a Boolean value indicating whether the described class has a property identified by the specified key.

func hasReadableProperty(forKey: String) -> Bool

Returns a Boolean value indicating whether the described class has a readable property identified by the specified key.

func hasWritableProperty(forKey: String) -> Bool

Returns a Boolean value indicating whether the described class has a writable property identified by the specified key.

func key(withAppleEventCode: FourCharCode) -> String?

Given an Apple event code that identifies a property or element class, returns the key for the corresponding attribute, one-to-one relationship, or one-to-many relationship.

func type(forKey: String) -> String?

Returns the name of the declared type of the attribute or relationship identified by the passed key.

