

- Network
-  nw_connection_receive(\_:\_:\_:\_:) 

Function

# nw_connection_receive(\_:\_:\_:\_:)

Schedules a single receive completion handler, with a range indicating how many bytes the handler can receive at one time.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func nw_connection_receive(
    _ connection: nw_connection_t,
    _ minimum_incomplete_length: UInt32,
    _ maximum_length: UInt32,
    _ completion: @escaping nw_connection_receive_completion_t
)
```

## Parameters 

`connection`  

A network connection instance.

`minimum_incomplete_length`  

The minimum length to receive from the connection, until the content is complete.

`maximum_length`  

The maximum length to receive from the connection in a single completion.

`completion`  

A receive completion is invoked exactly once for a call to receive. The completion indicates that the requested content has been received (in which case the content is delivered), or else an error has occurred.

The completion delivers the received content, which may be nil if the message is complete or an error occurred, the message context, a flag indicating if the message is complete, and any associated error.

## See Also

### Functions

func nw_advertise_descriptor_copy_txt_record_object(nw_advertise_descriptor_t) -> nw_txt_record_t?

Accesses the TXT record to advertise with the service.

func nw_advertise_descriptor_create_application_service(UnsafePointer&lt;CChar>) -> nw_advertise_descriptor_t

func nw_advertise_descriptor_create_bonjour_service(UnsafePointer&lt;CChar>?, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>?) -> nw_advertise_descriptor_t?

Initializes a Bonjour service to advertise.

func nw_advertise_descriptor_get_application_service_name(nw_advertise_descriptor_t) -> UnsafePointer&lt;CChar>?

func nw_advertise_descriptor_get_no_auto_rename(nw_advertise_descriptor_t) -> Bool

Checks whether the service prohibits automatic renaming in the event of a name conflict.

func nw_advertise_descriptor_set_no_auto_rename(nw_advertise_descriptor_t, Bool)

Sets a Boolean to indicate whether the service prohibits automatic renaming in the event of a name conflict.

func nw_advertise_descriptor_set_txt_record(nw_advertise_descriptor_t, UnsafeRawPointer?, Int)

Sets the TXT record as a raw buffer to advertise with the service.

func nw_advertise_descriptor_set_txt_record_object(nw_advertise_descriptor_t, nw_txt_record_t?)

Sets the TXT record to advertise with the service.

func nw_browse_descriptor_create_application_service(UnsafePointer&lt;CChar>) -> nw_browse_descriptor_t

func nw_browse_descriptor_create_bonjour_service(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>?) -> nw_browse_descriptor_t

Initializes a service descriptor used to discover a Bonjour service.

func nw_browse_descriptor_get_application_service_name(nw_browse_descriptor_t) -> UnsafePointer&lt;CChar>?

func nw_browse_descriptor_get_bonjour_service_domain(nw_browse_descriptor_t) -> UnsafePointer&lt;CChar>?

Accesses the Bonjour service domain set on a browse descriptor.

func nw_browse_descriptor_get_bonjour_service_type(nw_browse_descriptor_t) -> UnsafePointer&lt;CChar>

Accesses the Bonjour service type set on a browse descriptor.

func nw_browse_descriptor_get_include_txt_record(nw_browse_descriptor_t) -> Bool

Checks if the browse descriptor requires including associated TXT records with all results.

func nw_browse_descriptor_set_include_txt_record(nw_browse_descriptor_t, Bool)

Requires including associated TXT records with all results generated for this service descriptor.

