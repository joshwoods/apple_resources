

- SMS and Call Reporting
-  SMS and MMS Message Filtering 

API Collection

# SMS and MMS Message Filtering

Create an app extension that identifies and filters unwanted SMS and MMS messages while preserving user privacy.

## Overview

When a user receives an SMS or MMS message from an unknown sender, the Messages app can ask your Message Filter app extension to determine whether the message is unsolicited or otherwise unwanted. Your app extension can make this determination by using its own built-in data and logic or by deferring to analysis done by your associated server.

Note

IdentityLookup works only with SMS and MMS messages from unknown senders; it doesn’t work with messages from senders in a user’s Contacts list or with iMessage messages from any source.

To find out if a message from an unknown sender is unwanted, the Messages app launches the currently enabled Message Filter app extension and queries it, as shown in the figure below.

The Messages app uses an ILMessageFilterQueryRequest object to pass information about the message to your Message Filter app extension. If your app extension can determine whether the message is unwanted, it returns its decision to Messages in an ILMessageFilterQueryResponse object.

If your app extension can’t make this determination by itself, it tells Messages to send the information about the message to a server associated with your app. Your server examines the message information and sends a response to Messages, which passes the response to your app extension. The app extension parses the server’s response and returns the final decision to Messages in an ILMessageFilterQueryResponse object, as shown in the figure below.

Note

For privacy reasons, the system handles all communication with your associated server; your Message Filter app extension can’t access the network directly.

Your app extension also can’t write data to containers shared with the containing app.

## Topics

### First Steps

Creating a Message Filter App Extension

Create an app extension that helps identify unwanted messages.

### App Extension

class ILMessageFilterExtensionContext

The extension context for a Message Filter app extension.

class ILMessageFilterExtension

The abstract base class for the principal class of a Message Filter app extension.

### Queries

class ILMessageFilterQueryRequest

A request for a Message Filter app extension to determine the status of a message received from an unknown sender.

protocol ILMessageFilterQueryHandling

A set of methods implemented by a Message Filter app extension to handle query requests.

### Responses

class ILMessageFilterQueryResponse

A response to a message filter query request.

class ILNetworkResponse

A response to an HTTPS network request performed on behalf of a Message Filter app extension.

enum ILMessageFilterAction

Responds to a received message with a filter action.

### Errors

struct ILMessageFilterError

An error type that indicates problems with network requests and responses related to IdentityLookup APIs.

let ILMessageFilterErrorDomain: String

The error domain for errors associated with the IdentityLookup APIs.

