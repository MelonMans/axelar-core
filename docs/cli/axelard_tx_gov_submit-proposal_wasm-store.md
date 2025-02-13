## axelard tx gov submit-proposal wasm-store

Submit a wasm binary proposal

```
axelard tx gov submit-proposal wasm-store [wasm file] --title [text] --description [text] --run-as [address] --unpin-code [unpin_code] --source [source] --builder [builder] --code-hash [code_hash] [flags]
```

### Options

```
  -a, --account-number uint                   The account number of the signing account (offline mode only)
  -b, --broadcast-mode string                 Transaction broadcasting mode (sync|async|block) (default "block")
      --builder string                        Builder is a valid docker image name with tag, such as "cosmwasm/workspace-optimizer:0.12.9"
      --code-hash bytesHex                    CodeHash is the sha256 hash of the wasm code
      --code-source-url string                Code Source URL is a valid absolute HTTPS URI to the contract's source code,
      --deposit string                        Deposit of proposal
      --description string                    Description of proposal
      --dry-run                               ignore the --gas flag and perform a simulation of a transaction, but don't broadcast it (when enabled, the local Keybase is not accessible)
      --fee-account string                    Fee account pays fees for the transaction instead of deducting from the signer
      --fees string                           Fees to pay along with transaction; eg: 10uatom
      --from string                           Name or address of private key with which to sign
      --gas string                            gas limit to set per-transaction; set to "auto" to calculate sufficient gas automatically (default 200000)
      --gas-adjustment float                  adjustment factor to be multiplied against the estimate returned by the tx simulation; if the gas limit is set manually this flag is ignored  (default 1)
      --gas-prices string                     Gas prices in decimal format to determine the transaction fee (e.g. 0.1uatom) (default "0.007uaxl")
      --generate-only                         Build an unsigned transaction and write it to STDOUT (when enabled, the local Keybase is not accessible)
  -h, --help                                  help for wasm-store
      --instantiate-anyof-addresses strings   Any of the addresses can instantiate a contract from the code, optional
      --instantiate-everybody string          Everybody can instantiate a contract from the code, optional
      --instantiate-nobody string             Nobody except the governance process can instantiate a contract from the code, optional
      --instantiate-only-address string       Removed: use instantiate-anyof-addresses instead
      --keyring-backend string                Select keyring's backend (os|file|kwallet|pass|test|memory) (default "file")
      --keyring-dir string                    The client Keyring directory; if omitted, the default 'home' directory will be used
      --ledger                                Use a connected Ledger device
      --node string                           <host>:<port> to tendermint rpc interface for this chain (default "tcp://localhost:26657")
      --note string                           Note to add a description to the transaction (previously --memo)
      --offline                               Offline mode (does not allow any online functionality
  -o, --output string                         Output format (text|json) (default "json")
      --run-as string                         The address that is stored as code creator
  -s, --sequence uint                         The sequence number of the signing account (offline mode only)
      --sign-mode string                      Choose sign mode (direct|amino-json), this is an advanced feature
      --timeout-height uint                   Set a block timeout height to prevent the tx from being committed past a certain height
      --title string                          Title of proposal
      --unpin-code                            Unpin code on upload, optional
  -y, --yes                                   Skip tx broadcasting prompt confirmation (default true)
```

### Options inherited from parent commands

```
      --chain-id string     The network chain ID (default "axelar")
      --home string         directory for config and data (default "$HOME/.axelar")
      --log_format string   The logging format (json|plain) (default "plain")
      --log_level string    The logging level (trace|debug|info|warn|error|fatal|panic) (default "info")
      --trace               print out full stack trace on errors
```

### SEE ALSO

- [axelard tx gov submit-proposal](axelard_tx_gov_submit-proposal.md)	 - Submit a proposal along with an initial deposit
