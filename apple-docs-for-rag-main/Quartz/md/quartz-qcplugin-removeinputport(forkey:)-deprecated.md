

- Quartz
- QCPlugIn
-  removeInputPort(forKey:) Deprecated

Instance Method

# removeInputPort(forKey:)

Removes the input port for a given key.

macOS 10.4–10.15Deprecated

``` source
func removeInputPort(forKey key: String!)
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`key`  

The key associated with the port that you want to remove.

## Discussion

This method throws an exception if from within the execute(_:atTime:withArguments:) method, if there is not an input port with that key, or if the port is created from a property.

## See Also

### Adding Ports Dynamically

func addInputPort(withType: String!, forKey: String!, withAttributes: [AnyHashable : Any]!)

Adds an input port of the specified type and associates a key and attributes with the port.

Deprecated

func addOutputPort(withType: String!, forKey: String!, withAttributes: [AnyHashable : Any]!)

Adds an output port of the specified type and associates a key and attributes with the port.

Deprecated

func removeOutputPort(forKey: String!)

Removes the output port for a given key.

Deprecated

