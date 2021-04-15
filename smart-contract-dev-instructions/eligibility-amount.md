# Eligibility Amount

**Steps to set eligibility amount in Rookie and Professional Staking Pools:**

Eligibility amount will be used to check the user eligibility status for the Professional Tier.

1. Smart contract function ‘setEligibilityAmount’ needs to be invoked to set the new Eligibility amount for the Professional Tier.

**“function setEligibilityAmount\(uint256 amount\_\) public onlyOwner{}”**

2. setEligibilityAmount function takes one uint256 input variable.

Case 1: New Eligibility Amount – 5000 tokens

‘5000000000000000000000’ needs to be passed as input to the function.

a. Once the user has staked an amount greater than the eligibility amount, the eligibility status from this pool will be ‘true’, and after withdrawal the status will change to ‘false’.

