# nebula
Lightning Network style State Channels for Cosmos Hub

With a few modifications to Vesting accounts, I believe Lightning Network style functionality is possible on Cosmos Hub.

## Initial Thoughts:

2 or more participants deposit funds into a Vesting account. They can then pass messages to each other to update latest state and invalidate previous one in exact way Lightning does. If they ever publish a valid signed state to the Vesting Account, a timer starts where the other participants can challenge with the later state. If account passes the vesting period, any participant can trigger the Vesting account to send latest finalized balances to participant account.

It may be possible to do more than Lightning can by updating the total balance of the state channel on-chain, I haven't fully thought about this so its a big maybe.

Specific changes to Vesting Account interface will be documented later. The Nebula Account which will be used to create the behavior described above will implement the Vesting Account interface and will also be documented soon.

## Why Nebula?

Nebula models the Lightning Network. Lightning comes from clouds. Nebulas are space clouds. Nebula is built on Cosmos.
