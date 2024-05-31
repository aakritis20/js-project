Hello, My name is Aakriti Singh and here i am going to give the brief explanation of the given assessment/project.
So firstly, what i did is I created an array named as NFTs using a keyword var.
Then i created a function and named it mintNFT passed the parameters and then in that function i created another variable which is NFT and in that i created the objects of those parameters and then pushed the NFT into NFTs
In next step created another function listnfts to print the entries of all the objects using for loop
Then created another function gettotalsupply where the total number of entries are printed
And in last step i called all the function.
#Written below is the code

var NFTs=[]
function mintNFT (name,gender,languages) {
    var NFT={
        "name": name,
        "gender": gender,
        "languages": languages
    }
    NFTs.push(NFT);
    console.log("detail of user: "+name);
 }
function listNFTs () {
    for(var i=0;i<NFTs.length;i++){
        console.log("\nID: "+(i+1));
        console.log("name: "+NFTs[i].name);
        console.log("gender: "+NFTs[i].gender);
        console.log("languages: "+NFTs[i].languages);
    }
}

function getTotalSupply() {
    console.log(NFTs.length);

}
mintNFT("joey","male","german");
mintNFT("monica","female","english");
mintNFT("Ross","Male","English")
mintNFT("Rachel","female","Spanish");
listNFTs();
getTotalSupply();
