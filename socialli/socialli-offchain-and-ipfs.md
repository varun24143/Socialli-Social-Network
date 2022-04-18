# Socialli Offchain and IPFS

Off-chain is a storage where data is built on the basis of blockchain events. This allows the dapps to conveniently perform work that the blockchain itself does not allow. It will save text data, posts, comments, videos, images to IPFS, build user feeds and notifications in Postgresql, and support full text search by indexing the data into an ElasticSearch database.&#x20;

Socialli builds an integration directly to IPFS, where the contents and metadata of blocks will be stored for scaling purposes and the CIDs that are generated will be stored in the substrate node’s storage's corresponding to the various structs that will be constructed.
