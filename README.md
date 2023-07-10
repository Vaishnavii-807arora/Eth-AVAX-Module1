# Error Handlers Example

This is a simple smart contract written in Solidity that demonstrates the usage of three error handlers: `require`, `revert`, and `assert`. The contract provides basic functionalities for manipulating a counter variable.

## Contract Details

The `ErrorHandlersExample` contract has the following state variable:

- `counter`: An unsigned integer variable that holds the current counter value.

The contract provides the following functions:

### increment

solidity
```function increment(uint _value) public```
This function allows you to increment the counter by a specified value. It uses the require statement to validate that the _value parameter is greater than zero. If the condition fails, the function throws an exception with the error message "Value must be greater than zero".


### decrement
```function decrement(uint _value) public```
This function allows you to decrement the counter by a specified value. It checks if the _value parameter is greater than the current counter value. If it is, the function reverts the transaction and throws an exception with the error message "Value cannot exceed the current counter value".

### resetCounter
```function resetCounter() public```
This function resets the counter to zero. It uses the assert statement to ensure that the counter variable is greater than or equal to zero. If the condition fails, indicating an unexpected state, the transaction will be reverted.

## Getting Started
1. To interact with the smart contract, you'll need an Ethereum development environment such as Remix or the Solidity compiler. Follow these steps to get started:

2. Clone this repository or copy the smart contract code into a new Solidity file.

3. Compile the smart contract using your preferred Solidity compiler.

4. Deploy the contract to an Ethereum network of your choice. Ensure that you have the necessary permissions and funds to deploy the contract.

5. Once the contract is deployed, you can interact with it using the provided functions to increment, decrement, or reset the counter.

## Error Handling
The contract demonstrates the usage of three error handlers:

* require: Used to validate user input or check pre-conditions.

+ revert: Used to explicitly revert state changes and provide an error message.

- assert: Used to check for conditions that should never occur.

* By understanding and utilizing these error handlers, you can handle various scenarios and ensure the contract's intended behavior.

## Authors
Vaishnavi Arora

## License
This contract is licensed under the MIT License. SPDX-License-Identifier: MIT.
loom video link, https://www.loom.com/share/95fcdadff3414d09905e548cc0325628
