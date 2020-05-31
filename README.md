# solidity2
// Use of arrays and giving values to variables

pragma solidity ^0.6.1;

contract token{
   
   string public name;
  
   uint256[] public digits;
   address owner;
   
   
   function setname(string memory _name) public {
       name = _name;
   }
   
   function getname() public view returns(string memory){
       return(name);
   }
    
   function adddigits(uint256 _digits) public {
       digits.push(_digits);
   } 
   
   function seedigits() public view returns(uint256){
       return(digits.length);
   }
}

