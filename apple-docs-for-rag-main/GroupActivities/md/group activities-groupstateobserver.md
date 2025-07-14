

- Group Activities
-  GroupStateObserver 

Class

# GroupStateObserver

An object that contains information about the system’s ability to start SharePlay experiences.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
final class GroupStateObserver
```

## Mentioned in 

Presenting SharePlay activities from your app’s UI

## Overview

Starting a SharePlay experience with the Group Activities framework requires an active FaceTime call. Use a `GroupStateObserver` object to determine whether it’s possible to start such an experience. When no call is active, you might adjust your app’s user interface. For example, you might hide or remove controls that start a shared activity.

To get the current system state, create a `GroupStateObserver` object and check the value of its isEligibleForGroupSession property. To respond right away when the value of the property changes, configure a subscriber for that property.

## Topics

### Creating a group state observer

convenience init()

Creates a new group state observer object for determining the availability of group sessions.

### Determining the eligibility for shared activities

var isEligibleForGroupSession: Bool

A Boolean value that indicates whether the system can start a group session.

### Instance Properties

var $isEligibleForGroupSession: Published&lt;Bool>.Publisher

### Type Aliases

typealias ObjectWillChangePublisher

The type of publisher that emits before the object has changed.

### Default Implementations

ObservableObject Implementations

## Relationships

### Conforms To

- ObservableObject

