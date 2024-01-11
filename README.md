# I_Q

**Title: Block Creation and Timestamp Matching**

_Question:_
Imagine a blockchain where blocks are created within a time range of 10-14 seconds. The block numbering starts at 1, and each block is generated at an interval within this timeframe. Your task is to simulate the creation of 100 blocks adhering to this time range.

Following the block creation, the next challenge is to identify the closest block number corresponding to a given timestamp in seconds. How would you approach this task effectively?

The goal is twofold:

1. Generate 100 blocks within the specified time range.
2. Develop a method or algorithm to determine the closest block number concerning any given timestamp within this sequence.

Describe the steps and logic you'd employ to achieve both objectives. This question evaluates your understanding of time intervals, sequencing, and algorithmic thinking in the context of blockchain technology.

#### Random function

```javascript
function getRandomBlockTime() {
  return Math.floor(Math.random() * (14 - 10 + 1)) + 10;
}
```



---

**Title: Optimizing Multiple API Calls for Balances**

_Question:_
You are tasked with fetching balances for n wallet addresses across 5 different APIs, each associated with a specific blockchain. However, these APIs impose varying rate limits per second:

- API 1: 2 calls per second
- API 2: 3 calls per second
- API 3: 4 calls per second
- API 4: 5 calls per second
- API 5: 1 call per second

The challenge is to design an approach that enables fetching the balances of these wallets in the shortest time possible while respecting the rate limits of each API. How would you efficiently coordinate the API calls to achieve this goal without hitting the rate limits excessively?

Considerations:

- There are a total of 75 API calls needed (5 APIs \* 15 wallet addresses).
- Optimize the sequence and parallelism of API calls while adhering to the specific rate limits.
- Implement strategies to handle rate limit constraints, minimize execution time, and manage potential API call failures.

Explain your methodology and the logic behind your approach to manage these API calls effectively.

---
