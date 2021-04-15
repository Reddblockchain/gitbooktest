# Staking

**Staking method:**

Prerequisite: Make sure you have added an allowance of the staking amount to the staking pool from the token contract.

Any user can stake in the Rookie, Professional/Liquidity staking pools with no restriction on the amount, however the user has to deposit a certain amount to become eligible for the Professional Tier.

Only Professional Tier users have access to the Legendary staking pool.

Once the allowance is added to the staking pool, users can call the ‘_stake’_ function and pass the amount to be staked\(uint256\) in the pool.

After the staking is successful, users can view their staking details using ‘_userDeposits’_ function with their wallet address. This function returns the user staked amount, user staked time and the status of withdrawal.

Any user can stake only once with one wallet address, and after successful withdrawal of the current staking, user will now be able to stake again in the current pool.

\*\*\*\*

