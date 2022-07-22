# Metamask connect - HTML, JavaScript, Ethers:

A sample HTML file to show how to connect with Metamask from the front-end. This is a minimalistic example that you can find in the [Metamask docs](https://docs.metamask.io/guide/create-dapp.html#basic-action-part-1).

# Requirements

- [Metamask](https://metamask.io/)
  - This is a browser extension that lets you interact with the blockchain.

# Quickstart

1. Clone the repo, install dependencies, and create the build.

2. Serve the file

```
yarn http-server
```

And you'll see an output like:

```
Available on:
  http://127.0.0.1:8080
  http://x.x.x.x:8080
Hit CTRL + C to stop the server
```

Copy and paste the first link into your browser, and you should see a small button that says "Connect".

Hit it, and you should see that Metamask pop up.

# Execute a transaction

If you want to execute a transaction, follow this:

Make sure you have the following installed: Clone the hardhat-simple-storage in my repositories, then cd into it.

1. You'll need to open up a second terminal and run:

```
yarn hardhat node
```

This will deploy a sample contract and start a local hardhat blockchain.

2. Update your `index.js` with the new contract address.

In your `index.js` file, update the variable `contractAddress` with the address of the deployed contract. You'll see it near the top of the hardhat output.

3. Rebuild

```
yarn build
```

4. Connect your [metamask](https://metamask.io/) to your local hardhat blockchain.

> **PLEASE USE A METAMASK ACCOUNT THAT IS NOT ASSOCIATED WITH ANY REAL MONEY.**
>
> I usually use a few different browser profiles to separate my Metamasks easily.

In the output of the above command, take one of the private key accounts and [import it into your metamask.](https://metamask.zendesk.com/hc/en-us/articles/360015489331-How-to-import-an-Account)

Additionally, add your localhost (with chainId 31337) to your Metamask.

5. Reserve the front-end with `yarn http-server`, and then hit the `Execute` button after connecting

# Thank you!
