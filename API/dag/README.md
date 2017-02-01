dag API
=======

> The dag API comes to replace the `object API`, it support the creation and manipulation of dag-pb object, as well as other IPLD formats (i.e dag-cbor, ethereum-block, git, etc)

#### `dag.put`

> Store an IPLD format node

##### `Go` **WIP**

##### `JavaScript` - ipfs.dag.put(dagNode, formatMulticodec, hashAlg, callback)

- `dagNode` - a DAG node that follows one of the supported IPLD formats.
- `formatMulticodec` - The IPLD format multicodec.
- `hashAlg` - The hash algorithm to be used over the serialized dagNode.
- `callback` must follow `function (err) {}` signature, where `err` is an error if the operation was not successful.

If no `callback` is passed, a [promise][] is returned.

#### `dag.get`

> Retrieve an IPLD format node

##### `Go` **WIP**

##### `JavaScript` - ipfs.dag.get(cid, callback)

- `cid` is a [CID][https://github.com/ipfs/js-cid] instance.

`callback` must follow `function (err, dagNode) {}` signature, where `err` is an error if the operation was not successful and `dagNode` is the IPLD format DAG node retrieved.

If no `callback` is passed, a [promise][] is returned.