

- ARKit
-  ar_session_set_authorization_update_handler_f 

Function

# ar_session_set_authorization_update_handler_f

Sets the handler for receiving updates in authorization status for a specific authorization type.

visionOS 1.0+

``` source
extern void ar_session_set_authorization_update_handler_f(ar_session_t session, dispatch_queue_t authorization_update_queue, void * context, ar_authorization_update_handler_function_t authorization_update_handler_function);
```

## See Also

### Sessions

ar_session_t

The main entry point for receiving data from ARKit.

ar_session_create

Creates a new session.

ar_session_query_authorization_results

Checks whether the current session is authorized for particular authorization types without requesting authorization.

ar_session_query_authorization_results_f

Checks whether the current session is authorized for particular authorization types without requesting authorization.

ar_session_request_authorization

Requests authorization from the user to use the specified kinds of ARKit data.

ar_session_request_authorization_f

Requests authorization from the user to use the specified kinds of ARKit data.

ar_session_run

Runs a session with the data providers you supply.

ar_session_set_authorization_update_handler

Sets the handler for receiving updates in authorization status for a specific authorization type.

ar_session_set_data_provider_state_change_handler

Sets the handler for responding to a change in the state of one or more data providers.

ar_session_set_data_provider_state_change_handler_f

Sets the handler for responding to a change in the state of one or more data providers.

ar_session_data_provider_state_change_handler_t

A handler for receiving updates to data provider states.

ar_session_stop

Stops a session.

