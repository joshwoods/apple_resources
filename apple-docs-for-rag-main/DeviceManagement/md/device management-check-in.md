

- Device Management
-  Check-in 

API Collection

# Check-in

Authenticate devices and maintain push tokens with these commands.

## Overview

The MDM check-in protocol validates a deviceʼs eligibility for MDM enrollment and informs the server that a deviceʼs push token has been updated.

When the MDM payload is installed, the device initiates communication with the check-in server. The device validates the TLS certificate of the server, then uses the identity specified in its MDM payload as the client authentication certificate for the connection.

If a check-in server URL is provided in the MDM payload, the check-in protocol communicates with that check-in server. If no check-in server URL is provided, the main MDM server URL is used instead.

## Topics

### Commands

Authenticate

Authenticates a user during MDM payload installation.

UserAuthenticate

Authenticates a user with a two-step authentication protocol.

Check Out

Responds to the removal of the MDM enrollment profile from a device.

Get Token

Check-in protocol get-token data.

Token Update

Updates the token for a device on the server.

Get Bootstrap Token

Gets the bootstrap token.

Set Bootstrap Token

Sets the bootstrap token.

### Declarative Management

Declarative Management Checkin

The checkin protocol for declarative management.

Get Server Supported Declarations

Get a list of the declarations available on the server.

Get the Device Status

The request for getting the status of a device.

Get the Device Token

The request for sending the device token details.

## See Also

### MDM Protocol

Implementing Device Management

Set up an MDM server and send commands to managed devices.

Commands and Queries

Manage the configuration and behavior of your devices.

User Enrollment

Authenticate devices using an user identity focused workflow.

