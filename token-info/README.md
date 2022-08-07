# Pull Request Standards

Please follow the guidelines below to submit your pull request and list your token:

**1. Create a Folder**

The first thing you need to do is to create a folder named after your token's
smart contract address.

**2. Create The Files**

Inside your folder, you will need to create 3 files:

```shell
|- logo.json    -   Your logo information.
|- logo.png     -   Your logo file. Needs to be square.
|- token.json   -   Your token information.
```

**3. Format Your Files**

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

**4. Submit Your PR**

With all finished, you can submit your pull request and wait for merging. We may
also request changes before we merge, so please follow up on your PR to make sure
you process any changes required on a timely manner.
