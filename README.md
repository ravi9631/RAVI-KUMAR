// Create a variable to hold your NFTs
const NFTs = [];

// Function to mint a new NFT
function mintNFT(name, eyeColor, shirtType, bling) {
    const nft = {
        name: name,
        eyeColor: eyeColor,
        shirtType: shirtType,
        bling: bling
    };
    NFTs.push(nft);
    console.log("Minted: " + name);
}

// Function to list all NFTs
function listNFTs() {
    NFTs.forEach((nft, index) => {
        console.log(`ID: ${index + 1}`);
        console.log(`Name: ${nft.name}`);
        console.log(`Eye Color: ${nft.eyeColor}`);
        console.log(`Shirt Type: ${nft.shirtType}`);
        console.log(`Bling: ${nft.bling}\n`);
    });
}

// Function to get the total number of NFTs
function getTotalSupply() {
    console.log(`Total NFTs: ${NFTs.length}`);
}

// Call your functions below this line
mintNFT("Ravi", "Red", "T-shirt", "Gold Chain");
listNFTs();
getTotalSupply();
