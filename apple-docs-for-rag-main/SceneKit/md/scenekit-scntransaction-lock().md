

- SceneKit
- SCNTransaction
-  lock() 

Type Method

# lock()

Attempts to acquire a recursive spinlock to ensure the validity of values you retrieve during the transaction.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func lock()
```

## Discussion

SceneKit’s data model is thread-safe in that it ensures that internal data structures will not be corrupted by concurrent attempts to modify their contents from multiple threads. However, this model does not guarantee the validity of values you read from scene graph objects after returning them.

For example, consider the following operation:

```
_node.position = SCNVector3Make(_node.position.x, _node.position.y + 10, _node.position.z);
```

The intent of this line is to move a node by ten units. But if another thread modifies the node’s position property concurrently, the new position value could be unexpected. If your app modifies the scene graph from multiple threads, use a transaction lock to ensure that your modifications take effect as intended.

```
[SCNTransaction lock];
_node.position = SCNVector3Make(_node.position.x, _node.position.y + 10, _node.position.z);
[SCNTransaction unlock];
```

If another thread currently holds a lock on the transaction, calling lock() has no effect.

## See Also

### Managing Concurrency

class func unlock()

Relinquishes a previously acquired transaction lock.

