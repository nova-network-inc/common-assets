# Pull Request Standards

Please follow the guidelines below to submit your pull request and list your token.

## For ERC20 Tokens on EVM Chains

### 1. Create a Folder

The first thing you need to do is to create a folder named after your token's
smart contract address.

### 2. Create The Files

Inside your folder, you will need to create 3 files:

```shell
|- logo.json    -   Your logo information.
|- logo.png     -   Your logo file. Needs to be square.
|- token.json   -   Your token information.
```

### 3. Format Your Files

After you have all your files created, you need to format them so it's readable
and within standard.

For your `logo.json` use the format below:

```shell
{
  "logoSize": 512,
  "transparent": true,
  "format": "png",
  "path": "logo"
}
```

For your `token.json` use the format below:

```shell
{
  "chainId": [250],
  "address": "0x69D17C151EF62421ec338a0c92ca1c1202A427EC",
  "symbol": "SNT",
  "name": "Supernova Token",
  "decimals": 18,
  "tags": ["supernova", "token"]
}
```

### 4. Submit Your PR

With all finished, you can submit your pull request and wait for merging. We may
also request changes before we merge, so please follow up on your PR to make sure
you process any changes required on a timely manner.

## For Native Tokens

You will need to create a folder using your token's symbol inside the `_native`
directory. Inside your folder, you will need to create 2 files:

```shell
|- logo.json    -   Your logo information.
|- logo.png     -   Your logo file. Needs to be square.
```

The `logo.png` needs to be a square image, preferably in `PNG` format. You can use
`logo.json` to declare your logo's information, and you can use the format below:

```shell
{
  "logoSize": 512,
  "transparent": true,
  "format": "png",
  "path": "logo"
}
```
## Other Tokens

We still do not offer support for non-EVM token listings, but we may in the future.
If you want to get your token information submitted from a non-EVM chain, please
get in touch with us directly.
