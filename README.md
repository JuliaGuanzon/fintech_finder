<h1 align="center">Fintech Finder</h1> 


### Usage and Examples

As a note, the wages of the workers was decreased as the amount of Ethereum in the account was insufficient for the amount we would need to test.

**Original Code** 

```
candidate_database = {
    "Lane": ["Lane", "0xaC8eB8B2ed5C4a0fC41a84Ee4950F417f67029F0", "4.3", .20, "Images/lane.jpeg"],
    "Ash": ["Ash", "0x2422858F9C4480c2724A309D58Ffd7Ac8bF65396", "5.0", .33, "Images/ash.jpeg"],
    "Jo": ["Jo", "0x8fD00f170FDf3772C5ebdCD90bF257316c69BA45", "4.7", .19, "Images/jo.jpeg"],
    "Kendall": ["Kendall", "0x8fD00f170FDf3772C5ebdCD90bF257316c69BA45", "4.1", .16, "Images/kendall.jpeg"]
}
```
**New Wage**

This is the new wage for workers as they were too expensive for me to use with the small amount of Ethereum I had.
```
candidate_database = {
    "Lane": ["Lane", "0xaC8eB8B2ed5C4a0fC41a84Ee4950F417f67029F0", "4.3", .002, "Images/lane.jpeg"],
    "Ash": ["Ash", "0x2422858F9C4480c2724A309D58Ffd7Ac8bF65396", "5.0", .033, "Images/ash.jpeg"],
    "Jo": ["Jo", "0x8fD00f170FDf3772C5ebdCD90bF257316c69BA45", "4.7", .019, "Images/jo.jpeg"],
    "Kendall": ["Kendall", "0x8fD00f170FDf3772C5ebdCD90bF257316c69BA45", "4.1", .016, "Images/kendall.jpeg"]
}
```

As the user can see, there are four choices of workers to choose from:

![image](https://user-images.githubusercontent.com/84649228/140619760-783f779f-78f6-4f8f-9b25-9b28a4c4b5aa.png)
![image](https://user-images.githubusercontent.com/84649228/140619797-eba69f80-4dcb-4578-91e2-3260885e758b.png)

From here, the user can decide which worker they would like based on their hourly rate and their rating as a worker. When the user is ready, they can select the user they would like via the sidebar, as well as how long the user would like them to work for. Once they have made their choice, they can "Send Transaction." Once the transaction is complete, there will be a "Validated Transaction Hash" where the transaction hash will populate, thus confirming the transaction.

![image](https://user-images.githubusercontent.com/84649228/140619834-4dbeeea1-1612-450a-b255-10f785d17ed9.png)
![image](https://user-images.githubusercontent.com/84649228/140619875-ca63c534-498c-4b4d-a068-2243e1968b68.png)

