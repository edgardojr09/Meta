## Type of Functions. 
# Description.
I've been using the Oppenzeplin, I've been importing ONE

Contract 
The NabisToken contract, inheriting from the ERC20 contract, is defined by a state variable storing the contract owner's address and a lockTime mapping indicating token lock time.

Constructor
The constructor initializes the NabisToken contract by calling the ERC20 constructor with the name "Nabis Token" and symbol "NTK", and sets the owner variable to the deployment address.

Modifier Onlyowner
Modifier onlyOwner restricts access to specific functions by checking if the caller is the owner, and reverting with an error message if not.

Function mint
The owner can mint new tokens and assign them to a specific account, restricting access using the onlyOwner modifier and calling the internal mint function from the ERC20 contract. Paste the original address and need input any amount and transact it. You need to paste the Original address and need to input any amount and transact it

THE FUNCTION SETLOCKTIME
address account, uint256 time is public and onlyOwner, allowing only one account to be locked at a time.

Function Burn
The function 'BURN' enables users to burn their tokens, checking if they have sufficient balance to burn the specified amount, using the internal _burn function from the ERC20 contract.
 
Transfer
The function checks if the caller's tokens are locked and calls the parent contract's transfer function if not, and if not, calls the parent contract's transferFrom function.










