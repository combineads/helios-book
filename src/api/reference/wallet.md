# `Wallet`

An interface type for a wallet that manages a user's UTxOs and addresses. Notably implemented by the [`Cip30Wallet`](./cip30wallet.md) class.

## Getters

### `usedAddresses`

Gets a list of addresses which already contain UTxOs.

```ts
wallet.usedAddresses: Promise<helios.Address[]>
```

### `unusedAddresses`

Gets a list of unique unused addresses which can be used to UTxOs to.

```ts
wallet.unusedAddresses: Promise<helios.Address[]>
```

### `utxos`

Gets the complete list of [`UTxO`s](./utxo.md) sitting at the addresses owned by the wallet.

```ts
wallet.utxos: Promise<helios.UTxO[]>
```

## Methods

### `signTx`

Signs a [transaction](./tx.md), returning a list of signatures needed for submitting a valid transaction.

```ts
wallet.signTx(tx: helios.Tx): Promise<helios.Signature[]>
```

### `submitTx`

Submits a [transaction](./tx.md) to the blockchain. Returns the [`TxId`](./txid.md).

```ts
wallet.submitTx(tx: helios.Tx): Promise<helios.TxId>
```