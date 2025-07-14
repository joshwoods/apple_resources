

- FSKit
- FSTaskOptions
-  taskOptions 

Instance Property

# taskOptions

An array of strings that represent command-line options for the task.

macOS 15.4+

``` source
var taskOptions: [String] { get }
```

## Discussion

This property is equivalent to the `argv` array of C strings passed to a command-line tool.

