# metacrafter
const NFTs = []
//this function will take in some values as parameters,create an
//NFT object using the parameters passed to it for its metadata,
//and store it in the variable above 

function mintNFT (_name, _facecolor, _pantType, _chain) {
const NFT = {
"name":_name,
"faceColor":_facecolor,
"pantType":_pantType,
"chain":_chain
}
NFTs.push(NFT);
console.log("Minted: " + _name);
}
//create a "loop" that will go through an "array" of NFT's
//and print their metadata with console.log()
function listNFTs () {
for(let i = 0; i < NFTs.length; i++) {
console.log("\nID: \t\t " + (i + 1));
console.log("Name: \t\t" + NFTs[i].name);
console.log("Facecolor: \t" + NFTs[i].faceColor);
console.log("PantType: " + NFTs[i].pantType);
console.log("Chain :\t\t" + NFTs[i].chain);

 }
}
//print the total number of NFTs we have minted to the console 
function getTotalSupply() {
console.log("\n" + NFTs.length);
}
//call your functions below this line
mintNFT("rohit" , "White", "Jeans", "Diamond Chain");
mintNFT("surya" , "Black", "Joggers", "Silver Chain");
mintNFT("bumrah" , "Black", "Trousers", "Platinum Chain");
mintNFT("ishan", "White", "Track", "Silver Chain");
listNFTs();
getTotalSupply();
