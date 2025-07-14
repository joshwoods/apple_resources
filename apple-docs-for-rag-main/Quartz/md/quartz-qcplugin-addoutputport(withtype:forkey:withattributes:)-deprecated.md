

- Quartz
- QCPlugIn
-  addOutputPort(withType:forKey:withAttributes:) Deprecated

Instance Method

# addOutputPort(withType:forKey:withAttributes:)

Adds an output port of the specified type and associates a key and attributes with the port.

macOS 10.4–10.15Deprecated

``` source
func addOutputPort(
    withType type: String!,
    forKey key: String!,
    withAttributes attributes: [AnyHashable : Any]! = [:]
)
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`type`  

The port type. See Port Input and Output Types.

`key`  

The key to associate with the port.

`attributes`  

A dictionary of attributes for the port. See Input and Output Port Attributes. Although the dictionary is optional, it’s recommended that provide attributes to enhance the experience of those who use your custom patch. The attributes appear in a help tag when the user hovers a pointer over the property port on your custom patch. (See attributesForPropertyPort(withKey:).) Pass `nil` if you do not want to provide attributes.

## Discussion

This method throws an exception if called from within the execute(_:atTime:withArguments:) method or if there is already an output port with that key.

## See Also

### Adding Ports Dynamically

func addInputPort(withType: String!, forKey: String!, withAttributes: [AnyHashable : Any]!)

Adds an input port of the specified type and associates a key and attributes with the port.

Deprecated

func removeInputPort(forKey: String!)

Removes the input port for a given key.

Deprecated

func removeOutputPort(forKey: String!)

Removes the output port for a given key.

Deprecated

