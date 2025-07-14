

- Core Services
- Apple Events
-  AEEventSource 

Type Alias

# AEEventSource

A data type for values that specify how an Apple event was delivered.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias AEEventSource = Int8
```

## Discussion

Event Source Constants lists the valid constant values for a variable or parameter of type `AEEventSource`.

You might use a variable of this type, for example, to get the source type of an Apple event by calling the function AEGetAttributePtr(_:_:_:_:_:_:_:). You pass the `keyEventSourceAttr` constant as the value for the `theAEKeyWord` parameter and you pass a pointer to a variable of type `AEEventSource` for the `dataPtr` parameter.On return, the variable will contain one of the event source constant values described in Event Source Constants. The complete call looks like the following:

AppleEvent       theAppleEvent; // previously obtained Apple event
DescType        returnedType;
AEEventSource   sourceOfAE;
Size            actualSize;
OSErr           myErr;
myErr = AEGetAttributePtr(theAppleEvent,
                            keyEventSourceAttr,
                            typeShortInteger,
                            &amp;returnedType,
                            (void *) &amp;sourceOfAE,
                            sizeof (sourceOfAE),
                            &amp;actualSize);

