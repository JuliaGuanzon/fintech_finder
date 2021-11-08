<h1 align="center">Fintech Finder</h1> 

At Fintech Finder, we have created a user friendly application that will help customers find fintech professionals and enable the usage of cryptocurrency as a form of payment. Fintech Finder is bringing the future of paying instantaneously with cryptocurrency, as to lessen the time between the sending and receiving of payment as with other traditional forms of payment.

---
## Technologies

In order for this program to run, this application must be used in either Git Bash or VS Code, as it uses the Python language. To run the program, it is essential to have Anaconda/Python installed. To ensure the code works, please open the file in a dev environment using python.

The operating systems and program versions are mentioned below and are highly recommended when running the program.

**Systems**

[conda 4.10.3](https://docs.anaconda.com/anaconda/install/index.html) - Package manager, Environment Manager

python 3.7 - included in Anaconda

[Pandas](https://pandas.pydata.org/) - Open source data analysis and manipulation tool

**Other Installations**

[Streamlit](https://github.com/streamlit/streamlit) - Open source app framework

---

## Installation Guide


As mentioned above, to ensure that there are no errors when running this application, the user must use Git Bash or Visual Studio Code to access the application file. 

For this application, the user may need to downgrade their previous program installations. Please be sure to use the versions below:

```
pip uninstall pandas -y
pip install pandas==1.2.5

pip uninstall streamlit -y
pip install streamlit==0.84.2

```

WARNING: Pandas 1.3.0 or greater is not compatible with Streamlit.

---

## Usage

From the GitBash terminal, the user can open the application by entering the following code:

![image](https://user-images.githubusercontent.com/84649228/140665907-a9d943d9-f68d-4ce4-9cbd-ed81e893d581.png)

As the user can see, there are four choices of candidates to choose from:

![image](https://user-images.githubusercontent.com/84649228/140619760-783f779f-78f6-4f8f-9b25-9b28a4c4b5aa.png)
![image](https://user-images.githubusercontent.com/84649228/140619797-eba69f80-4dcb-4578-91e2-3260885e758b.png)

From here, the user can decide which candidate they would like to hire based on their hourly rate and their rating as a worker. When the user is ready, they can select the candidate they would like via the sidebar, as well as how long the user would like them to work for. Once they have made their choice, they can "Send Transaction." Once the transaction is complete, there will be a "Validated Transaction Hash" where the transaction hash will populate, thus confirming the transaction.

![image](https://user-images.githubusercontent.com/84649228/140619834-4dbeeea1-1612-450a-b255-10f785d17ed9.png)
![image](https://user-images.githubusercontent.com/84649228/140619875-ca63c534-498c-4b4d-a068-2243e1968b68.png)

---
## Inspecting Transactions via Kovan Etherscan

To ensure that transactions are working and going through, we can verify the details of the transaction by running our address in [Kovan Etherscan](https://kovan.etherscan.io/).

Once we conduct our transaction and a "Validation Transaction Hash," we are able to research the transaction.

![image](https://user-images.githubusercontent.com/84649228/140665509-a943542b-ba4e-4249-a20a-dd03937183e3.png)
<p align="center" width="50%">
    <img width="40%" src="https://user-images.githubusercontent.com/84649228/140665540-4cf3a5c5-41e0-4737-bf9d-1b8b980beba4.png"> 
</p> 

Enter the "Client Account Address" into the search bar, and you should see the image below.
It should show the user's transactions. As you can see in the image, there are transactions in and out, from funding the account to sending money to candidates.
![image](https://user-images.githubusercontent.com/84649228/140665734-507e7971-4ecf-47f6-b59b-18261ad79886.png)

The transaction between the user and candidate Kendall was for 0.00032 Ether. The transaction is the first item seen on the list. We can look into the detail by clicking the item under the "Txn Hash" as seen in the image below.
![image](https://user-images.githubusercontent.com/84649228/140665752-656366ec-76f4-47bd-bbeb-750e69dcecaf.png)

If you go back to the user's transaction page, you can click on the "To" address to see the receiver's transactions. Below are the candidate's transactions of getting paid.
![image](https://user-images.githubusercontent.com/84649228/140665774-884c698b-87e5-4b31-9a43-3f145a60321d.png)


### Note: Edit to Code

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

