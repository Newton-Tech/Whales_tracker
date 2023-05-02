# Whales_tracker

This is a Node.js script that interacts with the Ethereum network using the ethers.js library to monitor transfers of the USDT token. The script listens for events emitted by the USDT contract for Transfer events and checks if the transfer amount is greater than or equal to a specified threshold amount. If the transfer amount is greater than or equal to the threshold, the script plays a sound and logs a message to the console with a link to the Etherscan transaction page for the transfer.

The script uses the Ethereum JSON-RPC URL provided by Cloudflare to connect to the Ethereum network. It then instantiates a contract object for the USDT token using its contract address and ABI (Application Binary Interface), which is an interface that defines the contract's functions and events.

The script then listens for the Transfer event emitted by the contract using the on method of the contract object. When a Transfer event is emitted, the script checks if the transfer amount is greater than or equal to the specified threshold using a conditional statement. If the condition is true, the script plays a sound using the node-aplay library and logs a message to the console with a link to the Etherscan transaction page for the transfer.

Finally, the script calls the main function to execute the monitoring logic.
