# Project Title
This is the etherium begineer proof course project at metacrafter in which it explains to make own token with help of some prerequsites  

# Detialed Description
This is my metacrafter project of etherum beginner course in which they asked me to make some a contract in which i made three public variables that store the details about your coin (Token Name, Token Abbrv., Total Supply).
```contract MyToken {

    // public variables here
     string public tokenName = "Tesla";
     string public tokenAbbrv = "blue_tesla";
      uint  public totalSupply = 5; }
```
Do a mapping of addresses to balances (address => uint) and as we know that every address is associated with uint when you  given address it would return token amount.
```  
    // mapping variable here
    mapping(address => uint ) public balance ;
```
Here is the function named as "mint" which having two parameters names as address and value. This mint function will increase the totalsupply as the amount of the value is specified and similarly the balance of the address is increases as the value is specified in the mint function for the sender transcation.
```
// mint function  
  function Mint(address _address, uint _value) public{
    totalSupply += _value;
    balance[_address] +=_value;
```
Moreover, here we have the burn function which works opposite the mint function. It is meant to deduct the token from the sender or user. In this burn function token, the value gets deducted from the total supply and the balance of the “sender”. The Burn function also checks the sufficient balance before burning the token.
```
 function Burn(address _address, uint _value) public{
    if(balance[_address]>= _value)
    totalSupply -= _value;
    balance[_address] -= _value;
```
### THANK YOU FOR READING !!!
# Author
@Thekartick2003
KARTICK
