# Lottery

To run the lottery, make sure you are on a Unix system with Python 2.7 installed.

First, clone this repository by running:

```
git clone https://github.com/bethereumproject/bounty-lottery
```

The Block number used to generate the lottery seed will be: `6969000`. To make this lottery truly randomized and unpredictable we're using a block number which hasn't been mined yet! You can verify this by checking the timestamp of the edit when the block number was announced.


Navigate into the repository and run the following command with the correct seed generated by our smart contract:

```
python lottery.py <seed> > results.json
```

This will store the lottery outcome to the `results.json` file. You can check that the file is identical to ours by running:

```
cat results.json | | md5sum
```

The output should be: `4b2594d9f4449a1869695dcbf1a7aa63`
