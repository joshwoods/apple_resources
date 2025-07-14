

- Create ML
- MLDataTable
- MLDataTable.Row
-  subscript(\_:\_:) 

Instance Subscript

# subscript(\_:\_:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
subscript(name: MLDataTable.Row.Key, type: T.Type) -> T? where T : MLDataValueConvertible { get }
```

## See Also

### Accessing rows

subscript(MLDataTable.Row.Key) -> MLDataTable.Row.Value?

