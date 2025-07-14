

- Virtualization
- VZVirtioConsolePortConfiguration
-  isConsole 

Instance Property

# isConsole

A Boolean value that indicates whether this port is a console.

macOS 13.0+

``` source
var isConsole: Bool { get set }
```

## Discussion

The framework may mark the console port for use as the system console. The default is `false`.

## See Also

### Configuring the port

var name: String?

The name of the port.

