# hs-ledger-address

This tool will allow you to use a **Ledger device** and the Ledger Bitcoin app
to generate a [Handshake][handshake] address. In the future you should be able
to use the upcoming, Ledger Handshake app to sign & send transactions on the
Handshake network.

>NOTE: This tool will not allow you to sign & send transactions on the
Handshake network.

## Usage
```
hs-ledger-address:
  Usage:
    $ hs-ledger-address address [account no.] - Get first receive address for the specified account
    $ hs-ledger-address xpub [account no.] - Get xpub for the specified account
    $ hs-ledger-address devices - List all connected Ledger devices
    $ hs-ledger-address help - Show this message

  Options:
    -n, --network <network> (default "main")
    -h, -?, --help - Shows this message
    -t, --timeout (default 5000) - Ledger timeout

  NOTE: Handshake uses the same type of ECC private keys as Bitcoin (secp256k1),
  so private key generation can happen within the Ledger Bitcoin app. Because
  Ledger devices are BIP44 compliant, this tool is able to specify a path in
  the HD tree that is specific to Handshake addresses. It is recommended to use
  the first Handshake account by specifying `0` as your account no.
```

## License

- Copyright (c) 2018, Nodari Chkuaselidze (MIT License).


[handshake]: https://handshake.org
