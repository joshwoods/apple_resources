

- ARKit
-  ar_authorization_update_handler_t 

Type Alias

# ar_authorization_update_handler_t

A handler for receiving updates in authorization status for a specific authorization type.

visionOS 1.0+

``` source
typedef void (^)(NSObject *) ar_authorization_update_handler_t;
```

## See Also

### Authorization

ar_authorization_status_t

The authorization states for a type of ARKit data.

ar_authorization_type_t

The authorization types you can request from ARKit.

ar_authorization_result_get_authorization_type

Gets the authorization type associated with an authorization result.

ar_authorization_result_get_status

Gets the authorization status associated with an authorization result.

ar_authorization_results_enumerate_results

Enumerates a collection of authorization results.

ar_authorization_results_enumerate_results_f

Enumerates a collection of authorization results.

ar_authorization_results_get_count

Gets the number of authorization results in a collection.

ar_authorization_status_allowed

Your app has permission to use the associated kind of ARKit data.

ar_authorization_status_denied

Your app doesn’t have permission to use the associated kind of ARKit data.

ar_authorization_status_not_determined

Permission for your app to use the associated kind of ARKit data is undetermined.

ar_authorization_result_t

An authorization result.

ar_authorization_results_enumerator_t

A handler for enumerating a collection of authorization results.

ar_authorization_results_handler_t

A handler to call upon completion of an authorization request.

ar_authorization_results_t

A collection of authorization results.

ar_authorization_results_handler_function_t

