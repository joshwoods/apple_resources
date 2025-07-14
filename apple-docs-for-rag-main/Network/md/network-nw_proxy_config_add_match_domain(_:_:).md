

- Network
-  nw_proxy_config_add_match_domain(\_:\_:) 

Function

# nw_proxy_config_add_match_domain(\_:\_:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func nw_proxy_config_add_match_domain(
    _ config: nw_proxy_config_t,
    _ match_domain: UnsafePointer
)
```

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

