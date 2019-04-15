The function without a name, `function() payable public`, is called a fallback function.
This function sets the message sender as the owner; we just need to make sure the required
conditions are fullfilled.

First, contribute for a very small amount of ether:
`contract.contribute(0.0002)`

Then, activate the fallback function by just sending ether to the contract:
`contract.send({ value: 1 })`

Now you are contract owner ,just withdraw all the contract's funds by using:
`contract.withdraw()`
