

- Objective-C Runtime
- NSObject
-  NSKeyValueObserving 

API Collection

# NSKeyValueObserving

An informal protocol that objects adopt to be notified of changes to the specified properties of other objects.

## Overview

You can observe any object properties including simple attributes, to-one relationships, and to-many relationships. Observers of to-many relationships are informed of the type of change made — as well as which objects are involved in the change.

NSObject provides an implementation of the NSKeyValueObserving protocol that provides an automatic observing capability for all objects. You can further refine notifications by disabling automatic observer notifications and implementing manual notifications using the methods in this protocol.

## Topics

### Change Notification

func observeValue(forKeyPath: String?, of: Any?, change: [NSKeyValueChangeKey : Any]?, context: UnsafeMutableRawPointer?)

Informs the observing object when the value at the specified key path relative to the observed object has changed.

### Registering for Observation

func addObserver(NSObject, forKeyPath: String, options: NSKeyValueObservingOptions, context: UnsafeMutableRawPointer?)

Registers the observer object to receive KVO notifications for the key path relative to the object receiving this message.

func removeObserver(NSObject, forKeyPath: String)

Stops the observer object from receiving change notifications for the property specified by the key path relative to the object receiving this message.

func removeObserver(NSObject, forKeyPath: String, context: UnsafeMutableRawPointer?)

Stops the observer object from receiving change notifications for the property specified by the key path relative to the object receiving this message, given the context.

### Notifying Observers of Changes

func willChangeValue(forKey: String)

Informs the observed object that the value of a given property is about to change.

func didChangeValue(forKey: String)

Informs the observed object that the value of a given property has changed.

func willChange(NSKeyValueChange, valuesAt: IndexSet, forKey: String)

Informs the observed object that the specified change is about to be executed at given indexes for a specified ordered to-many relationship.

func didChange(NSKeyValueChange, valuesAt: IndexSet, forKey: String)

Informs the observed object that the specified change has occurred on the indexes for a specified ordered to-many relationship.

func willChangeValue(forKey: String, withSetMutation: NSKeyValueSetMutationKind, using: Set&lt;AnyHashable>)

Informs the observed object that the specified change is about to be made to a specified unordered to-many relationship.

func didChangeValue(forKey: String, withSetMutation: NSKeyValueSetMutationKind, using: Set&lt;AnyHashable>)

Informs the observed object that the specified change was made to a specified unordered to-many relationship.

### Observing Customization

class func automaticallyNotifiesObservers(forKey: String) -> Bool

Returns a Boolean value that indicates whether the observed object supports automatic key-value observation for the given key.

class func keyPathsForValuesAffectingValue(forKey: String) -> Set&lt;String>

Returns a set of key paths for properties whose values affect the value of the specified key.

var observationInfo: UnsafeMutableRawPointer?

Returns a pointer that identifies information about all of the observers that are registered with the observed object.

### Constants

class NSKeyValueObservation

struct NSKeyValueObservedChange

enum NSKeyValueChange

The kinds of changes that can be observed.

struct NSKeyValueObservingOptions

The values that can be returned in a change dictionary.

struct NSKeyValueChangeKey

The keys that can appear in the change dictionary.

enum NSKeyValueSetMutationKind

The kinds of mutation that you can make to an unordered collection.

## See Also

### Related Documentation

Key-Value Observing Programming Guide

