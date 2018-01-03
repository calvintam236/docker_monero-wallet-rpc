# What is Monero-Wallet-RPC?

Monero-Wallet-RPC is the RPC interface for Monero wallet provided by [monero-project](https://github.com/monero-project/monero).

# How to use this image [X86_64 version]

Create shared volume:

```console
$ docker volume create --name monero-wallet-rpc
```

Run in background:

```console
$ docker run -v monero-wallet-rpc:/monero-wallet-rpc -d --name YOUR_CONTAINER_NAME -p YOUR_PORT:YOUR_PORT calvintam236/monero-wallet-rpc:x86_64 --daemon-address YOUR_DAEMON_HOST:YOUR_DAEMON_PORT --daemon-login YOUR_DAEMON_USERNAME:YOUR_DAEMON_PASSWORD --rpc-bind-port YOUR_PORT --rpc-bind-ip 0.0.0.0 --rpc-login YOUR_WALLET_USERNAME:YOUR_WALLET_PASSWORD --confirm-external-bind
```

Get `monero-wallet-rpc` options with:

```console
$ docker run --rm calvintam236/monero-wallet-rpc:x86_64
```

Fetch logs of a container:

```console
$ docker logs YOUR_CONTAINER_NAME
```
