# Sender

```shell

cargo run -- --listen-address /ip4/127.0.0.1/tcp/40837 \
          --secret-key-seed 1 \
          provide \
          --path /home/remon/Pictures/octocat.png \
          --name octocat.png

```

## Receiver

```shell
cargo run -- --peer /ip4/127.0.0.1/tcp/40837/p2p/12D3KooWPjceQrSwdWXPyLLeABRXmuqt69Rg3sBYbU1Nft9HyQ6X \
          get \
          --name octocat.png
```

## Sender. Large File

```shell

cargo run -- --listen-address /ip4/127.0.0.1/tcp/40837 \
          --secret-key-seed 1 \
          provide \
          --path /home/remon/Downloads/material-theme.zip \
          --name material-theme.zip

```

## Receiver. Large File

```shell
cargo run -- --peer /ip4/127.0.0.1/tcp/40837/p2p/12D3KooWPjceQrSwdWXPyLLeABRXmuqt69Rg3sBYbU1Nft9HyQ6X \
          get \
          --name material-theme.zip
```
