

- Endpoint Security
-  es_event_xpc_connect_t 

Structure

# es_event_xpc_connect_t

Mac CatalystmacOS

``` source
struct es_event_xpc_connect_t
```

## Topics

### Initializers

init()

init(service_name: es_string_token_t, service_domain_type: es_xpc_domain_type_t)

### Instance Properties

var service_domain_type: es_xpc_domain_type_t

var service_name: es_string_token_t

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Structures

struct es_authorization_result_t

struct es_btm_launch_item_t

struct es_event_authentication_auto_unlock_t

struct es_event_authentication_od_t

struct es_event_authentication_t

struct es_event_authentication_token_t

struct es_event_authentication_touchid_t

struct es_event_authorization_judgement_t

struct es_event_authorization_petition_t

struct es_event_btm_launch_item_add_t

struct es_event_btm_launch_item_remove_t

struct es_event_gatekeeper_user_override_t

struct es_event_login_login_t

struct es_event_login_logout_t

struct es_event_lw_session_lock_t

