// SPDX-License-Identifier: MIT
pragma solidity ^0.8.9;

contract ownerAccess{
    address public owner;
    constructor(){
        owner=msg.sender;
    }
    modifier onlyOwner(){
        require (owner==msg.sender,"only owner can access");
        _;
    }
    function addition(uint256 u, uint256 v)public view onlyOwner returns(uint256){
        return u+v;
    }
    function subtraction(uint256 w,uint x) public view onlyOwner returns(uint256){
        return w-x;
    }
}
