

- Foundation
- AttributedString
-  AttributedString.SingleAttributeTransformer 

Structure

# AttributedString.SingleAttributeTransformer

A type that transforms an attribute by altering its range or value, or by replacing it entirely.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@preconcurrency
struct SingleAttributeTransformer where T : AttributedStringKey, T.Value : Sendable
```

## Overview

For simple transformations, the closure you provide to the `transformingAttributes(…)` methods of AttributedString can use this instance to change the attribute’s value. You can also use this instance to change the range of the string that the attribute applies to. To completely replace the attribute with an attribute of a different type, use replace(with:value:).

## Topics

### Accessing the Attribute’s Range

var range: Range&lt;AttributedString.Index>

The range of the attribute in the attributed string.

### Accessing the Attribute’s Value

var value: T.Value?

The value of the attribute.

### Replacing Attributes

func replace&lt;U>(with: U.Type, value: U.Value)

Replaces an attribute with a different attribute.

func replace&lt;U>(with: KeyPath&lt;AttributeDynamicLookup, U>, value: U.Value)

Replaces an attribute with a different attribute that a key path identifies.

## Relationships

### Conforms To

- Sendable

## See Also

### Transforming Attributes

func transformingAttributes&lt;K>(K.Type, (inout AttributedString.SingleAttributeTransformer&lt;K>) -> Void) -> AttributedString

Returns an attributed string by calling a closure that transforms one attribute of a source attributed string.

func transformingAttributes&lt;K>(KeyPath&lt;AttributeDynamicLookup, K>, (inout AttributedString.SingleAttributeTransformer&lt;K>) -> Void) -> AttributedString

Returns an attributed string by calling a closure that transforms one attribute, which a key path identifies, of a source attributed string.

func transformingAttributes&lt;K1, K2>(K1.Type, K2.Type, (inout AttributedString.SingleAttributeTransformer&lt;K1>, inout AttributedString.SingleAttributeTransformer&lt;K2>) -> Void) -> AttributedString

Returns an attributed string by calling a closure that transforms two attributes of a source attributed string.

func transformingAttributes&lt;K1, K2>(KeyPath&lt;AttributeDynamicLookup, K1>, KeyPath&lt;AttributeDynamicLookup, K2>, (inout AttributedString.SingleAttributeTransformer&lt;K1>, inout AttributedString.SingleAttributeTransformer&lt;K2>) -> Void) -> AttributedString

Returns an attributed string created by calling a closure that transforms two attributes, which key paths identify, of a source attributed string.

func transformingAttributes&lt;K1, K2, K3>(K1.Type, K2.Type, K3.Type, (inout AttributedString.SingleAttributeTransformer&lt;K1>, inout AttributedString.SingleAttributeTransformer&lt;K2>, inout AttributedString.SingleAttributeTransformer&lt;K3>) -> Void) -> AttributedString

Returns an attributed string by calling a closure that transforms three attributes of a source attributed string.

func transformingAttributes&lt;K1, K2, K3>(KeyPath&lt;AttributeDynamicLookup, K1>, KeyPath&lt;AttributeDynamicLookup, K2>, KeyPath&lt;AttributeDynamicLookup, K3>, (inout AttributedString.SingleAttributeTransformer&lt;K1>, inout AttributedString.SingleAttributeTransformer&lt;K2>, inout AttributedString.SingleAttributeTransformer&lt;K3>) -> Void) -> AttributedString

Returns an attributed string by calling a closure that transforms three attributes, which key paths identify, of a source attributed string.

func transformingAttributes&lt;K1, K2, K3, K4>(K1.Type, K2.Type, K3.Type, K4.Type, (inout AttributedString.SingleAttributeTransformer&lt;K1>, inout AttributedString.SingleAttributeTransformer&lt;K2>, inout AttributedString.SingleAttributeTransformer&lt;K3>, inout AttributedString.SingleAttributeTransformer&lt;K4>) -> Void) -> AttributedString

Returns an attributed string by calling a closure that transforms four attributes of a source attributed string.

func transformingAttributes&lt;K1, K2, K3, K4>(KeyPath&lt;AttributeDynamicLookup, K1>, KeyPath&lt;AttributeDynamicLookup, K2>, KeyPath&lt;AttributeDynamicLookup, K3>, KeyPath&lt;AttributeDynamicLookup, K4>, (inout AttributedString.SingleAttributeTransformer&lt;K1>, inout AttributedString.SingleAttributeTransformer&lt;K2>, inout AttributedString.SingleAttributeTransformer&lt;K3>, inout AttributedString.SingleAttributeTransformer&lt;K4>) -> Void) -> AttributedString

Returns an attributed string created by calling a closure that transforms four attributes, which key paths identify, of a source attributed string.

func transformingAttributes&lt;K1, K2, K3, K4, K5>(K1.Type, K2.Type, K3.Type, K4.Type, K5.Type, (inout AttributedString.SingleAttributeTransformer&lt;K1>, inout AttributedString.SingleAttributeTransformer&lt;K2>, inout AttributedString.SingleAttributeTransformer&lt;K3>, inout AttributedString.SingleAttributeTransformer&lt;K4>, inout AttributedString.SingleAttributeTransformer&lt;K5>) -> Void) -> AttributedString

Returns an attributed string created by calling a closure that transforms five attributes of a source attributed string.

func transformingAttributes&lt;K1, K2, K3, K4, K5>(KeyPath&lt;AttributeDynamicLookup, K1>, KeyPath&lt;AttributeDynamicLookup, K2>, KeyPath&lt;AttributeDynamicLookup, K3>, KeyPath&lt;AttributeDynamicLookup, K4>, KeyPath&lt;AttributeDynamicLookup, K5>, (inout AttributedString.SingleAttributeTransformer&lt;K1>, inout AttributedString.SingleAttributeTransformer&lt;K2>, inout AttributedString.SingleAttributeTransformer&lt;K3>, inout AttributedString.SingleAttributeTransformer&lt;K4>, inout AttributedString.SingleAttributeTransformer&lt;K5>) -> Void) -> AttributedString

Returns an attributed string created by calling a closure that transforms five attributes, which key paths identify, of a source attributed string.

