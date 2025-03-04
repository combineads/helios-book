# `PubKeyHash`

This is a type-safe wrapper around [`ByteArray`](./bytearray.md) that represents the hash of a public key. 

The first part of a regular payment address (i.e. not witnessed by a script) is a `PubKeyHash`.

Example instantiation:

```helios
pkh: PubKeyHash = PubKeyHash::new(#...); ...
```

## Associated Functions

### `new`

```helios
PubKeyHash::new(bytes: ByteArray) -> PubKeyHash
```

### `from_data`

```helios
PubKeyHash::from_data(data: Data) -> PubKeyHash
```

## Operators

### `==`

```helios
PubKeyHash == PubKeyHash -> Bool
```

### `!=`

```helios
PubKeyHash != PubKeyHash -> Bool
```

### `>=`

```helios
PubKeyHash >= PubKeyHash -> Bool
```

### `>`

```helios
PubKeyHash > PubKeyHash -> Bool
```

### `<=`

```helios
PubKeyHash <= PubKeyHash -> Bool
```

### `<`

```helios
PubKeyHash < PubKeyHash -> Bool
```

## Methods

### `serialize`

```helios
pkh.serialize() -> ByteArray
```

### `show`

Hexadecimal representation of a `PubKeyHash`.

```helios
pkh.show() -> String
```
