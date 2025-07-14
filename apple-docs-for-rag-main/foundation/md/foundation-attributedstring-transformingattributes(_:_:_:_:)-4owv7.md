

- Foundation
- AttributedString
-  transformingAttributes(\_:\_:\_:\_:) 

Instance Method

# transformingAttributes(\_:\_:\_:\_:)

Returns an attributed string by calling a closure that transforms three attributes of a source attributed string.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@preconcurrency
func transformingAttributes(
    _ k: K1.Type,
    _ k2: K2.Type,
    _ k3: K3.Type,
    _ c: (inout AttributedString.SingleAttributeTransformer, inout AttributedString.SingleAttributeTransformer, inout AttributedString.SingleAttributeTransformer) -> Void
) -> AttributedString where K1 : AttributedStringKey, K2 : AttributedStringKey, K3 : AttributedStringKey, K1.Value : Sendable, K2.Value : Sendable, K3.Value : Sendable
```

## Parameters 

`k`  

The AttributedStringKey that identifies an attribute to transform.

`k2`  

The AttributedStringKey that identifies a second attribute to transform.

`k3`  

The AttributedStringKey that identifies a third attribute to transform.

`c`  

A closure that receives three AttributedString.SingleAttributeTransformer instances that you use to access and alter the attributes’ ranges and values.

## Return Value

An attributed string with the applied transformations to the specified attributes.

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

struct SingleAttributeTransformer

A type that transforms an attribute by altering its range or value, or by replacing it entirely.

