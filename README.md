# Event-Example-8
Event Example.sol
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract EventExample {
    event MessageChanged(string newMessage);

    string public message;

    function setMessage(string memory _msg) public {
        message = _msg;
        emit MessageChanged(_msg);
    }
}
