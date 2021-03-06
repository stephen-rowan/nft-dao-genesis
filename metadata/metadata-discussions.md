# Metadata Discussions

## Alessandro Konrad's Proposal

{% embed url="https://forum.cardano.org/t/cip-nft-metadata-standard/45687" %}

## Native Tokens Q&A with Polina Vinogradova, lead engineer

{% embed url="https://www.youtube.com/watch?v=ZSvfITJp7R0&start=22" %}

### Notes

### Token features :

Each Token has a :

Policy id

Asset name \(the unique index\)

A policy script dictates how the token is minted. A policy can include/combine time intervals and signatures.

Metadata is stored in a transaction's history not on the ledger

### Metadata server

Metadata will be stored in JSON schema on a server.

Basic JSON schema will include :

Policy ID, Asset Name, Description, Logo, URL, Signatures required by policyID and Corresponding Keys

A token name can be registered more than once but not an asset name \(the unique index\)

Anyone will able to run their own metadata server with their own rules and standards. 

### Fees / Minimum Executable Value

The minimum executable value prevents overflow abuse of the blockchain. The cost is proportional to the amount of memory a UTXO entry takes up. By default the person sending the token pays the ADA fee.

Fees are scaled to the number of Tokens and Asset IDs in each transaction

Minimum Transaction fee : 1 ADA

Minimum Token fee : 1.4 ADA : 1 token with 1 asset ID and 1 NAME

Anyone will able to run their own metadata server instance.

The value for ADA is stored as a protocol parameter.

### Metadata Registry

Currently the registry will be maintained / audited manually \(via GitHub ?\). 

Only holders of Policy ID / Keys will be able to post entries in the metadata registry.

It is hoped that anyone running their own metadata server maintains these minimum security standards. 

### Metadata Standards

The Cardano Foundation JSON schema specfied \(above\) is the extant metadata standard.

### ERC-20

ERC-20 interface transactions will have to checked off the Cardano chain \( to check ETH is burnt\). Refer ERC-20 questions to upcoming Q and A from that team.

### References

{% embed url="https://github.com/cardano-foundation/cardano-token-registry" %}

{% embed url="https://github.com/input-output-hk/cardano-metadata-submitter" %}

{% embed url="https://docs.cardano.org/projects/cardano-node/en/latest/reference/simple-scripts.html" %}

Discord context

{% embed url="https://discordapp.com/channels/804069702572965888/812452503966056488/826827405624344668" %}







