# Rewards

**Rewards:**

Rewards need to be manually added to the smart contracts using the “_addReward_” function.

Prerequisite: Make sure you have added an allowance of the reward amount to the staking pool.

Once the allowance is added to the Staking pool from the token contract, pass the reward amount as parameter\(uint256\) to the ‘addReward’ function. All staking pools have ‘totalReward’ and ‘rewardBalance’ read functions which return the total Rewards added to the smart contract till date and the current balance of rewards the smart contract holds.

Also users can check the ‘stakedTotal’ and ‘stakedBalance’ read functions which return the total tokens staked in the pool till date and the current staked balance in the smart contract to determine the rewards to be added to the pool.

Anyone can add rewards to the staking pools.

**Reward Calculation:**

Rewards will be calculated at the time of user withdrawal. This calculation will take care of all the effective interest rate changes during the user active lock period and will calculate the reward accordingly. The calculation will discard any changes in the effective interest rate during the passive lock period \(User lock duration expired but haven’t unstaked\).



