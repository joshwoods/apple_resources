

- Security
-  SecTransformMetaAttributeType Deprecated

Enumeration

# SecTransformMetaAttributeType

The keys that describe the metadata attributes of transform attributes.

macOS 10.7–13.0Deprecated

``` source
enum SecTransformMetaAttributeType
```

Deprecated

SecTransform is no longer supported

## Overview

Use one of these values as the `type` parameter in a call to the SecTransformCustomSetAttribute(_:_:_:_:) or SecTransformCustomGetAttribute(_:_:_:) function. These values allow you to access not only the value of an attribute, as you would do directly with calls the SecTransformSetAttribute(_:_:_:_:) or SecTransformGetAttribute(_:_:) function, but also the metadata associated with that attribute, such as the name of an attribute, or whether it is required to have a value.

## Topics

### Constants

case canCycle

The transform allows cyclic behavior.

case deferred

The attribute defers notifications.

case externalize

The attribute is exportable.

case hasInboundConnection

The attribute has an inbound connection.

case hasOutboundConnections

The attribute has an outbound connection.

case name

The name of the attribute.

case ref

A direct reference to an attribute’s value.

case required

Indicates whether the attribute value is optional.

case requiresOutboundConnection

The attribute requires an outbound connection.

case stream

The attribute expects stream operation.

case value

The actual value of the attribute.

### Initializers

init?(rawValue: CFIndex)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

