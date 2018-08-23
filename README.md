# hs-ledger-address

This tool will allow you to use **Ledger device** to generate [Handshake][handshake] addresss.
Even though this won't allow you to sign transactions, this is safe way to generate/backup and get addresses for handshake.

You can use this tool with `ledger bitcoin app`. In the future you should be able to use ledger Handshake ledger app, using same seed.

## Usage
```
hs-ledger-address:
  Usage:
    $ hs-ledger-address address [account=0] - Get address for the account.
    $ hs-ledger-address xpub [account=0] - Get xpub for the account.
    $ hs-ledger-address devices - List all ledger devices
    $ hs-ledger-address help - Shows this message.

  Options:
    -n, --network <network> (default "main")
    -h, -?, --help - Shows this message
    -t, --timeout (default 5000) - Ledger timeout

  NOTE: Handshake uses same type of private keys as Bitcoin, so
  private key generation can happen within Ledger Bitcoin App.
  They will be used to generate addresses for HSK. Please always
  backup your private keys even on ledger.
```

## License

- Copyright (c) 2018, Nodari Chkuaselidze (MIT License).


[handshake]: http://handshake.org/
