

- Matter
-  Accessory control 

API Collection

# Accessory control

Communicate with commissioned Matter accessories.

## Overview

Once you’ve commissioned a Matter accessory, use these methods to read and write data, subscribe to data updates, and send commands.

## Topics

### Controlling accessories

class MTRAttributeRequestPath

class MTREventRequestPath

class MTRProductIdentity

class MTRDevice

class MTRBaseDevice

class MTRClusterStateCacheContainer

class MTRWriteParams

class MTRReadParams

class MTRSubscribeParams

class MTRClusterPath

class MTRAttributePath

class MTREventPath

class MTRCommandPath

class MTRAttributeReport

class MTREventReport

protocol MTRDeviceDelegate

protocol MTRDeviceControllerClientProtocol

protocol MTRDeviceControllerServerProtocol

class MTRAsyncCallbackQueueWorkItemDeprecated

class MTRAsyncCallbackWorkQueueDeprecated

class MTRAttributeCacheContainerDeprecated

class MTROTAHeaderParserDeprecated

### Logging information

typealias MTRLogCallback

func MTRSetLogCallback(MTRLogType, MTRLogCallback?)

### Handling errors

typealias MTRDeviceErrorHandler

struct MTRError

enum Code

