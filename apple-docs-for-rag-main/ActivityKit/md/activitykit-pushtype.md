

- ActivityKit
-  PushType 

Structure

# PushType

The structure that offers constants you use to configure a Live Activity to receive updates through ActivityKit push notifications.

iOS 16.1+iPadOS 16.1+

``` source
struct PushType
```

## Overview

Pass the token constant to the request(attributes:contentState:pushType:) function to start a Live Activity that receives content updates with ActivityKit push notifications. Pass channel(_:) to request(attributes:contentState:pushType:) function to specify that you want to use a broadcast channel instead of a token. You can only specify one PushType.

To learn more about using ActivityKit push notifications to update your Live Activity, see Starting and updating Live Activities with ActivityKit push notifications.

## Topics

### Supporting ActivityKit push notifications

static var token: PushType

A constant you use to configure a Live Activity that updates its dynamic content by receiving ActivityKit push notifications.

static func channel(String) -> PushType

A constant to configure a Live Activity that updates its dynamic content for broadcast channels.

### Operators

static func == (PushType, PushType) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

## See Also

### Starting a Live Activity

static func request(attributes: Attributes, content: ActivityContent&lt;Activity&lt;Attributes>.ContentState>, pushType: PushType?) throws -> Activity&lt;Attributes>

Requests and starts a Live Activity.

let attributes: Attributes

A set of attributes that describe a Live Activity and its content.

protocol ActivityAttributes

The protocol you implement to describe the content of a Live Activity.

enum ActivityStyle

var content: ActivityContent&lt;Activity&lt;Attributes>.ContentState>

The dynamic content of a Live Activity.

struct ActivityContent

A structure that describes the state and configuration of a Live Activity.

typealias ContentState

The type alias for the structure that describes the dynamic content of a Live Activity.

enum ActivityAuthorizationError

An error that indicates why the request to start a Live Activity failed.

static func request(attributes: Attributes, content: ActivityContent&lt;Activity&lt;Attributes>.ContentState>, pushType: PushType?, style: ActivityStyle) throws -> Activity&lt;Attributes>

