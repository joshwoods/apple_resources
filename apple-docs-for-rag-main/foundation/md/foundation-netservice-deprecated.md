

- Foundation
-  NetService Deprecated

Class

# NetService

A network service that broadcasts its availability using multicast DNS.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.2–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
class NetService
```

Deprecated

Use nw_connection_t or nw_listener_t in Network framework instead

## Overview

The NetService class represents a network service, either one your application publishes or is a client of. This class and the NetServiceBrowser class use multicast DNS to convey information about network services to and from your application. The API of NetService provides a convenient way to publish the services offered by your application and to resolve the socket address for a service.

The types of services you access using NetService are the same types that you access directly using BSD sockets. HTTP and FTP are two services commonly provided by systems. (For a list of common services and the ports used by those services, see the file `/etc/services`.) Applications can also define their own custom services to provide specific data to clients.

You can use the NetService class as either a publisher of a service or a client of a service. If your application publishes a service, your code must acquire a port and prepare a socket to communicate with clients. Once your socket is ready, you use the NetService class to notify clients that your service is ready. If your application is the client of a network service, you can either create an NetService object directly (if you know the exact host and port information) or use an NetServiceBrowser object to browse for services.

To publish a service, initialize your NetService object with the service name, domain, type, and port information. All of this information must be valid for the socket created by your application. Once initialized, call the publish() method to broadcast your service information to the network.

When connecting to a service, use the NetServiceBrowser class to locate the service on the network and obtain the corresponding NetService object. Once you have the object, call the resolve(withTimeout:) method to verify that the service is available and ready for your application. If it is, the addresses property provides the socket information you can use to connect to the service.

The methods of NetService operate asynchronously so your application is not impacted by the speed of the network. All information about a service is returned to your application through the NetService object’s delegate. You must provide a delegate object to respond to messages and to handle errors appropriately.

## Topics

### Creating Network Services

convenience init(domain: String, type: String, name: String)

Returns the receiver, initialized as a network service of a given type and sets the initial host information.

init(domain: String, type: String, name: String, port: Int32)

Initializes the receiver for publishing a network service of type `type` at the socket location specified by `domain`, `name`, and `port`.

### Configuring Network Services

class func data(fromTXTRecord: [String : Data]) -> Data

Returns an `NSData` object representing a TXT record formed from a given dictionary.

class func dictionary(fromTXTRecord: Data) -> [String : Data]

Returns a dictionary representing a TXT record given as an `NSData` object.

var addresses: [Data]?

A read-only array containing `NSData` objects, each of which contains a socket address for the service.

var domain: String

A string containing the domain for this service.

var includesPeerToPeer: Bool

Specifies whether to also publish, resolve, or monitor this service over peer-to-peer Bluetooth and Wi-Fi, if available. false by default.

func getInputStream(UnsafeMutablePointer&lt;InputStream?>?, outputStream: UnsafeMutablePointer&lt;OutputStream?>?) -> Bool

Creates a pair of input and output streams for the receiver and returns a Boolean value that indicates whether they were retrieved successfully.

var name: String

A string containing the name of this service.

var type: String

The type of the published service.

func txtRecordData() -> Data?

Returns the TXT record for the receiver.

func setTXTRecord(Data?) -> Bool

Sets the TXT record for the receiver, and returns a Boolean value that indicates whether the operation was successful.

var delegate: (any NetServiceDelegate)?

The delegate for the receiver.

### Managing Run Loops

func schedule(in: RunLoop, forMode: RunLoop.Mode)

Adds the service to the specified run loop.

func remove(from: RunLoop, forMode: RunLoop.Mode)

Removes the service from the given run loop for a given mode.

### Using Network Services

func publish()

Attempts to advertise the receiver’s on the network.

func publish(options: NetService.Options)

Attempts to advertise the receiver on the network, with the given options.

func resolve()

Starts a resolve process for the service.

func resolve(withTimeout: TimeInterval)

Starts a resolve process of a finite duration for the service.

var port: Int

The port on which the service is listening for connections.

func startMonitoring()

Starts the monitoring of TXT-record updates for the receiver.

func stop()

Halts a currently running attempt to publish or resolve a service.

func stopMonitoring()

Stops the monitoring of TXT-record updates for the receiver.

### Obtaining the DNS Hostname

var hostName: String?

A string containing the DNS hostname for this service.

### Constants

NSNetServices Errors

If an error occurs, the delegate error-handling methods return a dictionary with the following keys.

enum ErrorCode

These constants identify errors that can occur when accessing net services.

struct Options

These constants specify options for a network service.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Local Network Services

protocol NetServiceDelegate

The interface a net service uses to inform its delegate about the state of the service it offers.

NSBonjourServices

Bonjour service types browsed by the app.

NSLocalNetworkUsageDescription

A message that tells the user why the app is requesting access to the local network.

