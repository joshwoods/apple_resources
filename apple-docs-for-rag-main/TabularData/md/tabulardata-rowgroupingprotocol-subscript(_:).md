

- TabularData
- RowGroupingProtocol
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Retrieves a group slice by key.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(keys: Any?...) -> DataFrame.Slice? { get }
```

**Required**

## Parameters 

`keys`  

A comma-separated, or variadic, list of key optionals.

