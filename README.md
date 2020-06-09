# Gamecash

Gamecash is an innovative PoW + PoS-based + Masternode cryptocurrency

Pos/Masternode global interest first year: 60%
Masternode Reward: 54%
Pos reward: 6%

Pos/Masternode global interest second year: 30%
Masternode Reward: 27%
Pos reward: 3%

Pos/Masternode global interest Third/Fifth year: 15%
Masternode Reward: 13,5%
Pos reward: 1,5%

Masternode Collateral: 100,000

Pow: 
First year: 1
Second year: 250
Third/Fifth year: 100

Supply: 300M (genesis time)

Gamecash  has  a  very  special  masternode  reward,  the  reward  is calculated based on PoS (Proof-Of-Stake) instead of PoW (Proof-Of-Work).  
Each  PoS  block  generates  different  amount  of  GameCash based on the coins staked.
There is only one masternode winner for each PoS block, the winner is  designated  by  hash  calculation  similar  to  PoW, and it is fully random.
Therefore,  a masternode could earn rewards in three continuous PoS blocks, and a masternode could also earn nothing in thousand PoS blocks. 
GameCash  has  60%  PoS  block  reward  in  the  first  year,  54%  is allocated  to  masternode  and  6%  for  coin  staker, by result of this formula: nSubsidy = nCoinAge * COIN_YEAR_REWARD * 33 / (365 * 33 + 8); 



Gamecash uses libsecp256k1,
			  libgmp,
			  Boost1.55,
			  OR Boost1.57,  
			  Openssl1.01m,
			  Berkeley DB 4.8,
			  QT5 to compile


Block Spacing: 60 Seconds
Stake Minimum Age: 8 Hours

Port: 58754
RPC Port: 58854


BUILD LINUX (see the [Wiki](https://github.com/sagacrypto/Gamecash/wiki/Unix-Build) for dependencies)
-----------
1) git clone source

2) cd Gamecash/src

3) mkdir obj/crypto

4) chmod +x leveldb/build_detect_platform

5) cd leveldb && make libleveldb.a libmemenv.a

6) cd ..

7) sudo make -f makefile.unix USE_UPNP=    # Headless Gamecash

8) strip gamecashd

9) sudo cp gamecashd /usr/local/bin




