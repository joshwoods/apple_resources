

- Foundation
-  ObjectiveCConvertibleAttributedStringKey 

Protocol

# ObjectiveCConvertibleAttributedStringKey

A protocol that defines Objective-C interoperability with an attribute key’s value type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
protocol ObjectiveCConvertibleAttributedStringKey : AttributedStringKey
```

## Overview

Conform to this protocol to allow your attributed string key to customize its Objective-C conversion behavior. This allows you to define an Objective-C value type and provide methods to convert to and from this type.

Attributed string keys that don’t conform to this protocol cast the value to AnyObject before converting to Objective-C. When converting from Objective-C, the value casts to the key’s Value type. In cases where Swift types bridge automatically to Objective-C types, like String to NSString, this default behavior is adequate. But for unbridged value types, you need to conform to this protocol and provide the conversion methods.

## Topics

### Accessing the Objective-C Type

associatedtype ObjectiveCValue : NSObject

The Objective-C type that corresponds to this key’s value type.

**Required**

### Converting between Swift and Objective-C Types

static func objectiveCValue(for: Self.Value) throws -> Self.ObjectiveCValue

Returns an Objective-C typed value for a given value of this key’s type.

**Required** Default implementations provided.

static func value(for: Self.ObjectiveCValue) throws -> Self.Value

Returns a value of this key’s type for a given Objective-C value.

**Required** Default implementations provided.

## Relationships

### Inherits From

- AttributedStringKey

### Conforming Types

- AttributeScopes.AccessibilityAttributes.AdjustedPitchAttribute
- AttributeScopes.AccessibilityAttributes.AnnouncementPriorityAttribute
- AttributeScopes.AccessibilityAttributes.HeadingLevelAttribute
- AttributeScopes.AccessibilityAttributes.TextualContextAttribute
- AttributeScopes.AppKitAttributes.AdaptiveImageGlyphAttribute
- AttributeScopes.AppKitAttributes.StrikethroughStyleAttribute
- AttributeScopes.AppKitAttributes.UnderlineStyleAttribute
- AttributeScopes.FoundationAttributes.InflectionAlternativeAttribute
- AttributeScopes.FoundationAttributes.InlinePresentationIntentAttribute
- AttributeScopes.FoundationAttributes.LinkAttribute
- AttributeScopes.FoundationAttributes.PersonNameComponentAttribute
- AttributeScopes.UIKitAttributes.AdaptiveImageGlyphAttribute
- AttributeScopes.UIKitAttributes.StrikethroughStyleAttribute
- AttributeScopes.UIKitAttributes.UnderlineStyleAttribute

