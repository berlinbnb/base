// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract BasicMath {
    // Function: adder
    function adder(uint _a, uint _b) public pure returns (uint sum, bool error) {
        unchecked {
            sum = _a + _b;
            // Check for overflow
            if (sum < _a) {
                return (0, true);
            }
        }
        return (sum, false);
    }

    // Function: subtractor
    function subtractor(uint _a, uint _b) public pure returns (uint difference, bool error) {
        if (_b > _a) {
            return (0, true); // Underflow
        }
        difference = _a - _b;
        return (difference, false);
    }
}
