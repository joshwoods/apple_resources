

- Network
-  Privacy Management 

API Collection

# Privacy Management

Configure parameters related to user privacy.

## Topics

### Traffic Attribution

Inspecting app activity data

Verify that your app accesses only the user data and network resources that you expect it to access.

Indicating the source of network activity

Control whether the App Privacy Report attributes network traffic to the app or to the user.

func nw_parameters_set_attribution(nw_parameters_t, nw_parameters_attribution_t)

Sets a flag that indicates whether the network request originates from the developer or the user.

func nw_parameters_get_attribution(nw_parameters_t) -> nw_parameters_attribution_t

Gets a flag that indicates whether the network request originates from the developer or the user.

enum nw_parameters_attribution_t

The entities that can make a network request.

## See Also

### Network Security and Privacy

Security Options

Configure security options for TLS handshakes.

Creating an Identity for Local Network TLS

Learn how to create and use a digital identity in your application for local network TLS.

