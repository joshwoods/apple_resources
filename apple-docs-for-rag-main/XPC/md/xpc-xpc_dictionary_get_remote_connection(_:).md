

- XPC
-  xpc_dictionary_get_remote_connection(\_:) 

Function

# xpc_dictionary_get_remote_connection(\_:)

Returns the connection that receives the dictionary.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_dictionary_get_remote_connection(_ xdict: xpc_object_t) -> xpc_connection_t?
```

## Parameters 

`xdict`  

The dictionary object which is to be examined.

## Return Value

If the dictionary was received by a connection event handler or a dictionary created through xpc_dictionary_create_reply(_:), a connection object over which a reply message can be sent is returned. For any other dictionary, NULL is returned.

## See Also

### Dictionary objects

struct XPCDictionary

A type that contains key-value pairs, notably used as the container of messages between a client and listener.

func xpc_dictionary_create(UnsafePointer&lt;UnsafePointer&lt;CChar>>?, UnsafePointer&lt;xpc_object_t?>?, Int) -> xpc_object_t

Creates an XPC object that represents a dictionary of XPC objects keyed to C-strings.

func xpc_dictionary_create_empty() -> xpc_object_t

Creates an XPC object that represents a dictionary of XPC objects keyed to C-strings.

func xpc_dictionary_create_connection(xpc_object_t, UnsafePointer&lt;CChar>) -> xpc_connection_t?

Creates a connection from a dictionary directly.

func xpc_dictionary_create_reply(xpc_object_t) -> xpc_object_t?

Creates a dictionary that is in reply to the specified dictionary.

func xpc_dictionary_set_value(xpc_object_t, UnsafePointer&lt;CChar>, xpc_object_t?)

Sets the value for the specified key to the specified object.

func xpc_dictionary_get_count(xpc_object_t) -> Int

Returns the number of values in the dictionary.

func xpc_dictionary_get_value(xpc_object_t, UnsafePointer&lt;CChar>) -> xpc_object_t?

Returns the value for the specified key.

func xpc_dictionary_apply(xpc_object_t, (UnsafePointer&lt;CChar>, xpc_object_t) -> Bool) -> Bool

Invokes the specified block for every key-value pair in the dictionary.

func xpc_dictionary_dup_fd(xpc_object_t, UnsafePointer&lt;CChar>) -> Int32

Creates a file descriptor from a dictionary directly.

func xpc_dictionary_get_array(xpc_object_t, UnsafePointer&lt;CChar>) -> xpc_object_t?

Returns the array value for the specified key.

func xpc_dictionary_get_bool(xpc_object_t, UnsafePointer&lt;CChar>) -> Bool

Gets a Boolean primitive value from a dictionary directly.

func xpc_dictionary_get_data(xpc_object_t, UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;Int>?) -> UnsafeRawPointer?

Gets a raw data value from a dictionary directly.

func xpc_dictionary_get_date(xpc_object_t, UnsafePointer&lt;CChar>) -> Int64

Gets a date value from a dictionary directly.

func xpc_dictionary_get_dictionary(xpc_object_t, UnsafePointer&lt;CChar>) -> xpc_object_t?

Returns the dictionary value for the specified key.

