

- Swift
- SIMDStorage
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses the element at the specified index.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
subscript(index: Int) -> Self.Scalar { get set }
```

**Required** Default implementations provided.

## Parameters 

`index`  

The index of the element to access. `index` must be in the range `0..

## Default Implementations

### SIMDStorage Implementations

subscript&lt;Index>(SIMD8&lt;Index>) -> SIMD8&lt;Self.Scalar>

Extracts the scalars at specified indices to form a SIMD8.

subscript&lt;Index>(SIMD3&lt;Index>) -> SIMD3&lt;Self.Scalar>

Extracts the scalars at specified indices to form a SIMD3.

subscript&lt;Index>(SIMD16&lt;Index>) -> SIMD16&lt;Self.Scalar>

Extracts the scalars at specified indices to form a SIMD16.

subscript&lt;Index>(SIMD32&lt;Index>) -> SIMD32&lt;Self.Scalar>

Extracts the scalars at specified indices to form a SIMD32.

subscript&lt;Index>(SIMD64&lt;Index>) -> SIMD64&lt;Self.Scalar>

Extracts the scalars at specified indices to form a SIMD64.

subscript&lt;Index>(SIMD2&lt;Index>) -> SIMD2&lt;Self.Scalar>

Extracts the scalars at specified indices to form a SIMD2.

subscript&lt;Index>(SIMD4&lt;Index>) -> SIMD4&lt;Self.Scalar>

Extracts the scalars at specified indices to form a SIMD4.

