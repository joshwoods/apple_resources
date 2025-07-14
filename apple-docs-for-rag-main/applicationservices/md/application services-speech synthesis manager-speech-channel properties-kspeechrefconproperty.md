

- Application Services
- Speech Synthesis Manager
- Speech-Channel Properties
-  kSpeechRefConProperty 

Global Variable

# kSpeechRefConProperty

Set a speech channel’s reference constant value.

macOS 10.5+

``` source
let kSpeechRefConProperty: CFString
```

## Discussion

The reference constant value is passed to application-defined callback functions and might contain any value convenient for the application. The value associated with this property is a `CFNumber` object that contains an integer value. For example, an application might set the value of the `CFNumber` object to an address in memory that contains a reference to an object or a pointer to a function.

This property works with the SetSpeechProperty(_:_:_:) function.

