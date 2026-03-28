# SendEther.sol
Remix - Deploy Contract On Base Network SendEther.sol
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract SendEther {
    function send(address payable _to) public payable {
        _to.transfer(msg.value);
    }
}
