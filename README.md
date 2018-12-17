
# appStoreDAO.Concept
This spawned out of conversations with a few other app (ala Android, iOS, etc) devs who have had issues with distribution while trying to include blockchain tech in their offerings.
This is an idea to bring the community at large together to create a 'decentralized' app store of sorts, making it easier to distribute compiled apps to end users without dealing with walled gardens.

The BULVRD Team does not currently have the bandwidth to tackle this as a whole but if there becomes enough interest across the community, we'd like to be involved in getting this going.

Feel free to open an issue or put in a pull request on this to open up some discussion!

## High Level:

App developers are still heavily dependent on platform focused app store for distribution. While still taking heavy profit cuts from devs, they also act as gate keepers and often keep great products out. Some of the bigger app stores are currently working out details on how to allow blockchain / crypto projects. For example both Apple and Google are known to push projects to make changes to get listed, sometimes having to leave core vision out to get published. Amazon's app store currently does not allow any blockchain or crypto apps to be listed, yet AWS has direct support for Ethereum node deployment. 

While a main focus here is on blockchain / crypto projects, there are countless other industries that lack the ability to reach end users.

The core of this idea is to create a truly decentralized app store. Meaning no gate keepers, no cuts taken from devs, and global accessibility. 

### How?

We can leverage a lot of existing Ethereum blockchain based tech to make this happen. A DAO can be setup that a developer can buy into. All entry funds are of course then managed by the DAO and used as seen fit. 

NFTs seem like a great use here as well. A spec'd standard could be leveraged to make searching and indexing streamlined. This would also provide a solution for transferring ownership.

For example, you could even look at the ERC-721 spec. A lot of the spec'd metadata would carry over the what someone distributing an app would want. Taking same principles, a dev can link externally to images, download links, etc. IPFS could be leveraged here, or a dev could host themselves which would make version updating a bit easier without having to update the contract and redeploy. But maybe that would actually be more ideal?

Maybe a json blob looks something like:

    {
    "name" : "BULVRD",
    "snippet" : "BULVRD is the global community mapping and route reporting ecosystem that allows you to earn cryptocurrency tokens while you drive",
    "logoUrl" : "https://bulvrdapp.com/logo.jpg",
    "bannerUrl" : "https://bulvrdapp.com/banner.jpg",
    "description": "Drive and explore the world via 3D maps, Augmented Reality, and in-car with Apple CarPlay.",
    "screenshots" : ["","","",],
    "platform" : "Android",
    "downloadUrl" : "https://bulvrdapp.com/app/android.apk",
    "website" : "https://bulvrdapp.com"
    }

The DAO could manage creating and releasing the base 'app stores' that index these.  Be it web viewers, mobile apps, etc.

This can also open up some new interesting ways for a developer to monetize an app without having to work within the confines of given app stores.

#### Some Examples:

- NFT creates a copy and deposits to users wallet. NFT must be in user wallet to open app?
    - Can enable instant secondary market?
- User must hold app token to use
- Dev gets 100% of in-app purchases made

#### Some Problems:
- While you'd want to make it as open as possible, at some level there needs to be validation of ownership. This could be managed via the DAO, or some community based initiative. 
- Would you want to filter out unverified apps? For example, lets say someone uploaded a Coinbase apk that had some data mining changes, assumingely you'd want a way to protect end users from this?
