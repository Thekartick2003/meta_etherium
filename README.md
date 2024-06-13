This is my metacrafter project of etherum beginner course in which they asked me to make some a contract which have some public variables that store the details about your coin (Token Name, Token Abbrv., Total Supply)
Do a mapping of addresses to balances (address => uint) and as we know that every address is associated with uint when you  given address it would return token amount.
Here is the function mint which having two parameters names as address and value. This mint function will increase the totalsupply as the amount of the value is specified and similarly the balance of the address is increases as the value is specified in the mint function for the sender transcation.
Moreover, here the burn function which will meant to deduct the token from the  sender or user.
In this burn function token get deducted value from the total supply and from the balance of the “sender”.
The Burn function also check that the sufficent balance before burning the token.
