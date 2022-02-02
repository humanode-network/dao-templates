- Import private key to humanode network to `~/.aragon/humanode_key.json`

```
{
  "rpc": "http://127.0.0.1:9933",
  "keys": ["0x99b3c12287537e38c90a9219d4cb074a89a16e9cdb20bf85728ebd97c343e342"]
}
```

- If you have problems with node version on installing dependencies, add `--ignore-engines` to the command.

- Go to `/shared` directory and run `yarn` and then `yarn link`

- Go to `/templates/company`

- `yarn link @aragon/templates-shared`

- Install deps

`yarn`

- Compile contracts

`yarn compile`

- A test humanode account with funds is used.

`OWNER="0x6Be02d1d3665660d22FF9624b7BE0551ee1Ac91b`

- Deploy Company Template

`npx truffle exec --network humanode scripts/deploy.js --ens <ENS Registry address> --dao-factory <DAO Factory address>`
