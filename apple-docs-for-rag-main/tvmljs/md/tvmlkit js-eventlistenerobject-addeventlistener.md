

- TVMLKit JS
- EventListenerObject
-  addEventListener 

Instance Method

# addEventListener

Creates an event listener.

tvOS 9.0+

``` source
void addEventListener(
    in String type, 
    in Object listener, 
    in optional Object extraInfo
);
```

## Parameters 

`type`  

The developer-defined name of the event type to add.

`listener`  

The listener object to be added. This object is typically a function.

`extraInfo`  

Optional parameter that is used to handle specific types of events. Different events have different formats.

## Discussion

Use the `extraInfo` parameter to handle information for different types of events; for example, specifying the type of metadata a metadata listener is listening for.

## See Also

### Adding and Removing Event Listeners

removeEventListener

Removes the designated event listener.

