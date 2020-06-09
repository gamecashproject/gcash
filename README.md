# Gamecash

Gamecash is a PoW + PoS-based + Masternode cryptocurrency

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




