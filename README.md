# crypto-wallet

The purpose of this project is to create a platform called Fintech Finder - an application that allows users to find fintech professionals from among a list of candidates, hite them, and then pay them by hour. The project leverages the Ethereum blockchain network to enable users to instantly pay the professionals with cryptocurrency. The application can be run in the Streamlit web app in conjunction with Ganache.

This is how the Streamlit app looks when the fintech_finder.py file is opened:
![image](https://user-images.githubusercontent.com/89161654/155928424-428fffc5-6487-4b98-91e4-360383a562f2.png)

This is the result of paying Jo for 2 hours at a rate of 0.19 eth = 0.38 eth total:
![image](https://user-images.githubusercontent.com/89161654/155929082-61bf5618-2343-4bb4-a715-544cdb973c9f.png)

The transaction is reflected in Ganache:
![image](https://user-images.githubusercontent.com/89161654/155929139-3eaa1b09-dc2d-46e9-87da-2d91ff8aef3a.png)
![image](https://user-images.githubusercontent.com/89161654/155929167-32ee39ff-a4b8-4467-a392-7fc9c1b9300a.png)

The history of the To address is shown below to reflect the new value:
![image](https://user-images.githubusercontent.com/89161654/155929361-68aca694-745a-4f20-b7c0-f96b60228eed.png)

## Technologies

This project leverages Python 3.7 with streamlit, dataclasses, typing, and web3.

## Installation

Before running this package, ensure that you have streamlit, Ganache, and Web3 libraries installed.

Please install the following libraries using the respective code:

Streamlit
```
pip install streamlit
```

Web3.py
```
pip install web3==5.17
```

eth-tester
```
pip install eth-tester==0.5.0b3
```

mnemonic
```
pip install mnemonic
```

bip44
```
pip install bip44
```

You can download Ganache from the following link: https://www.trufflesuite.com/ganache

## Usage

In order to use this project, clone the repo onto your machine. Open up a Quickstart Ethereum Workspace in Ganache. Ensure that the port number matches that in the fintech_finder.py code. Also ensure that your mnemonic has been set up to match that of the .env file. Once this is properly set up, you can navigate to the repo in your terminal, and run the streamlit webapp via `streamlit run fintech_finder.py`

If the webapp has launched successfully, you can choose the desired fintech professional to hrie and pay on the right, and the number of hours you would like to pay them for. After you hit send transaction, the transaction should be accurately reflected in Ganache.

## Contributors

Austin Do (austindotech@gmail.com)

## License

MIT
