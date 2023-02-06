# Solana RPC

Install the following packages.

- [Solanapy](https://github.com/michaelhly/solana-py)

`pip install solana`

- [Solders](https://github.com/kevinheavey/solders)

`pip intsall solders`

# Local validator rpc example
 
For local developement run `solana-test-validator`

```python
from solana.rpc.api import Client
from solders.pubkey import Pubkey

client = Client("http://localhost:8899")
publickey = client.get_account_info(Pubkey([0] * 31 + [1]))

Pubkey.from_string('4vJ9JU1bJJE96FWSJKvHsmmFADCg4gpZQff4P3bkLKi')
```
