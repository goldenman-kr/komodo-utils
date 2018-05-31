# komodo-notarynode-mined-counter

## instruction

0. Precondition : komodo installed and you are KMD miner

1. please install jsoncpp library to parse response of komodod
```
sudo apt-get install libjsoncpp-dev
```

2. how to compile : 
```
$ g++ -o exefileName sourceFile.cpp -ljsoncpp
ex) $ g++ -o nodeMined nn.cpp -ljsoncpp
```

3. how to run
```
$ ./nodeMined (if no params, default 25, default 814000)

$ ./nodeMined 100  (display last 100 blocks mined since Block 814000)

$ ./nodeMined 100 850000 (display last 10 blocks mined since Block 850000)

$ ./nodeMined 0 850000 (display last 25(default) blocks mined since Block 850000)
```

------------------------

## Example
```
$ ./nodeMined 15 850000
Loading blockchain info...please wait...(numOfList:15)
--------------------------------------------------------
num     Amount          Height          Time Interval(M)
--------------------------------------------------------
1       3.00000000      850091 (0)
96      3.00001000      856947 (+66)    58
97      3.00067400      857024 (+77)    117
98      3.00062400      857095 (+71)    67
99      3.00031200      857195 (+100)   89
100     3.00093600      857261 (+66)    63
101     3.00113400      857328 (+67)    65
102     3.00354695      857394 (+66)    65
103     3.00081200      857460 (+66)    64
104     3.00799398      857526 (+66)    84
105     3.00060000      857592 (+66)    68
106     3.00247200      857696 (+104)   84
107     3.00031200      857765 (+69)    72
108     3.41157273      857835 (+70)    69
109     3.00062400      857901 (+66)    63
110     3.00094600      857967 (+66)    64
--------------------------------------------------------
Largest: 3.41157273 KMD
Average: 3.00729866 KMD
Total  : 330.80285222 KMD (avrg interval : 71)
--------------------------------------------------------
Last my reward : 857967 (37 ago)
Cur last block : 858004
Est next block : 858038 (34 left)
--------------------------------------------------------
Last mined : 2018-05-31 06:33 (-86 mins)
Curr Time  : 2018-05-31 08:00
--------------------------------------------------------
Mined per Hour  : 2.49756778 KMD
Mined per Day   : 59.94162668 KMD
Mined per Month : 1823.22447807 KMD
--------------------------------------------------------

```
