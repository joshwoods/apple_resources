

- Network
-  nw_endpoint_t 

Type Alias

# nw_endpoint_t

A local or remote endpoint in a network connection.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 6.0+

``` source
typealias nw_endpoint_t = any OS_nw_endpoint
```

## Topics

### Endpoint Types

struct nw_endpoint_type_t

The type of a network endpoint, such as a host or a service.

func nw_endpoint_get_type(nw_endpoint_t) -> nw_endpoint_type_t

Accesses the type of a endpoint.

### Host Endpoints

func nw_endpoint_create_host(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>) -> nw_endpoint_t

Creates a network endpoint with a hostname and port, where the hostname may be interpreted as an IP address.

func nw_endpoint_get_hostname(nw_endpoint_t) -> UnsafePointer&lt;CChar>

Accesses the hostname stored in an endpoint.

func nw_endpoint_get_port(nw_endpoint_t) -> UInt16

Accesses the port stored in an endpoint, in host-byte order.

func nw_endpoint_copy_port_string(nw_endpoint_t) -> UnsafeMutablePointer&lt;CChar>

Copies the port of an endpoint as a string.

### Address Endpoints

func nw_endpoint_create_address(UnsafePointer&lt;sockaddr>) -> nw_endpoint_t

Creates a network endpoint with an address structure.

func nw_endpoint_get_address(nw_endpoint_t) -> UnsafePointer&lt;sockaddr>

Accesses the address structure stored in an address endpoint.

func nw_endpoint_copy_address_string(nw_endpoint_t) -> UnsafeMutablePointer&lt;CChar>

Copies the address of an endpoint as a string.

func nw_endpoint_copy_port_string(nw_endpoint_t) -> UnsafeMutablePointer&lt;CChar>

Copies the port of an endpoint as a string.

### Bonjour Service Endpoints

func nw_endpoint_create_bonjour_service(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>) -> nw_endpoint_t

Creates a network endpoint with a Bonjour service name, type, and domain.

func nw_endpoint_get_bonjour_service_name(nw_endpoint_t) -> UnsafePointer&lt;CChar>

Accesses the Bonjour service name stored in an endpoint.

func nw_endpoint_get_bonjour_service_type(nw_endpoint_t) -> UnsafePointer&lt;CChar>

Accesses the Bonjour service type stored in an endpoint.

func nw_endpoint_get_bonjour_service_domain(nw_endpoint_t) -> UnsafePointer&lt;CChar>

Accesses the Bonjour service domain stored in an endpoint.

### URL Endpoints

func nw_endpoint_create_url(UnsafePointer&lt;CChar>) -> nw_endpoint_t

Creates a network endpoint with a URL string.

func nw_endpoint_get_url(nw_endpoint_t) -> UnsafePointer&lt;CChar>

Accesses the URL string stored in an endpoint.

