# Processing a Transaction and Recording Through Ganache

An integral part of a blockchain is the ability to send transactions and trust that it is confirmed and validated on the blockchain. In this application, we explore hiring hypothetical contractors and sending transactions to the blockchain through Ganache as they are paid in ETH. 

---

## Technologies 

This application was built on Python 3.7. Streamlit library enables the blockchain to have a front end visual for users. 

To run this code, in terminal run: 

`streamlit run fintech_finder.py`

---

## Libraries

Import statements already present in program, refer to them below:

```python
import streamlit as st
from dataclasses import dataclass
from typing import Any, List
from web3 import Web3
import os
import requests
from dotenv import load_dotenv
load_dotenv()
from bip44 import Wallet
from web3 import Account
from web3 import middleware
from web3.gas_strategies.time_based import medium_gas_price_strategy
```

---

## Results

In this example, out of our potential contractors, we hire Lane for 20 hours. At an hourly rate of 0.2 ETH/hr, we are looking at transferring a total of 4 ETH to her wallet. The transaction went through and is validated by the green transaction hash in the bottom left corner:

<img width="1214" alt="Screen Shot 2022-10-17 at 15 50 35" src="https://user-images.githubusercontent.com/107497500/196284311-fc4d4104-a88b-4a45-aeef-96897bdfa469.png">

Further evidence of the transaction going through is found in the Ganache application. Seen below: 

<img width="1197" alt="Screen Shot 2022-10-17 at 15 52 03" src="https://user-images.githubusercontent.com/107497500/196284324-9719213b-53bf-48fb-970a-d16983f7da35.png">

Further details about the transaction can be found in the transaction tab in Ganache. Seen below:

<img width="1194" alt="Screen Shot 2022-10-17 at 15 52 19" src="https://user-images.githubusercontent.com/107497500/196284330-aa04a566-c276-4fc3-903d-e0718dc07f25.png">


---
## Contributors

Thank you for Eric Cardena for teaching Rice's FinTech Boot Camp. He was instrumental in teaching and helping us understand this material. Thank you for Rice for preparing this curriculum and the corresponding data sets that are required to be used. 

**Rishi Prasadha**

**LinkedIn**: https://www.linkedin.com/in/rishi-prasadha-912212133/

**Instagram**: @therishiprasadha

**Twitter**: @RishiPrasadha

---

## Licenses 

MIT
