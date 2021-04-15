# APY

**Steps to set the interest rate according to the APY changes in smart contracts\(Only Owner\).**

1. Smart contract function ‘setRate’ needs to be invoked in order to set the interest rate and this can be done only by the contract owner. - “_**function setRate\(uint256 rate\_\) public onlyOwner{}**_”

2. setRate function takes one uint64 variable input and this is the new interest rate to be used multiplied by 100.

Interest rate calculator:

Case 1: New APY: 8%

For 1 month lock period: \(8/12\) = 0.67 \* 100 = 67

‘67’ needs to be passed as input to the ‘setRate’ function for the contract with a 1 month lock period.

Case 2: New APY: 12%

For 3-month lock period: \(12/12\) \* 3 = 3 \*100 = 300

‘300’ needs to be passed as input to the ‘setRate’ function for the contract with a 3-month lock period.

a. Once the interest rate of the pool changes, the new interest rate can be viewed using the ‘index’ and the ‘rates’ function.

b. ‘Index’ – the current change in the effective interest rate of the pool.

c. ‘rates’ – the read function that returns the effective interest rate and the timestamp it was added to the pool\(takes index as input\).

d. When user stakes in the current pool, the current index of the pool will be linked with the staking. This will be used for the reward calculation.

