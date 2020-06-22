# Spicy NetFlow

This repository contains some [Spicy](https://github.com/zeek/spicy) in the
context of NetFlow.

## Usage

Create a self-contained binary:

```sh
spicy-build -o netflow-v5 netflow-v5.spicy
./netflow-v5 < test.data
```

Compile HILTI object code and use Spicy's driver utility:

```sh
spicyz -o neflow-v5.hlto netflow-v5.spicy
spicy-driver neflow-v5.hlto < test.data
```

More soon.
