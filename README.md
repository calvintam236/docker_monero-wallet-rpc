## Monero-Wallet-RPC

### What is it?

Monero-Wallet-RPC is the RPC interface for Monero wallet provided by [monero-project](https://github.com/monero-project/monero).

### Example usages

Replace `ARCH` for your system architecture. Available option(s): `x86_64`

- To run the container in background:

```console
$ docker run -v monero-wallet-rpc:/monero-wallet-rpc -d --name YOUR_CONTAINER_NAME -p YOUR_PORT:YOUR_PORT calvintam236/monero-wallet-rpc:ARCH --daemon-address YOUR_DAEMON_HOST:YOUR_DAEMON_PORT --daemon-login YOUR_DAEMON_USERNAME:YOUR_DAEMON_PASSWORD --rpc-bind-port YOUR_PORT --rpc-bind-ip 0.0.0.0 --rpc-login YOUR_WALLET_USERNAME:YOUR_WALLET_PASSWORD --confirm-external-bind
```

- Get `monero-wallet-rpc` options:

```console
$ docker run --rm calvintam236/monero-wallet-rpc:ARCH
```

- To fetch logs of a container:

```console
$ docker logs YOUR_CONTAINER_NAME
```

### Donations

If you like to buy me a cup of coffee for this Dockerfile/ docker image, you can donate to here:

- BTC: `1MTkPFtp3qxE4Y98pTHP3z767RGKmrT92a`
- ETH: `0x5896a85E8c175c563DC00087535582394d394838`
- XMR: `4ASikgNhKqmY5EjnaoDws1jjyhQy9ZrcDcCwfYVt5Rtxb6B1FqsehpLY8ZxxZD5B6r8QZKb4y1FKW1eqiS5Lph77Ca9qprU`
- ETC: `0xFaBA3be3b3De5469C3F6C6185150928F3773C7b4`
- ZEC: `t1Z5Kc75JQ17txyaDUfwwyabTgsJMfuuSp4`
