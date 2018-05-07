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
$ ./nodeMined 100  (display last 100 blocks mined)

$ ./nodeMined (if no number, default 25)
```

------------------------

## Example
```
$ ~/nodeMined 10
Loading blockchain info...please wait...10
--------------------------------------------------------
num     Amount          Height          Time Interval(M)
--------------------------------------------------------
1       3.00081282      814258  -----
137     3.00013118      823992 (+111)   115
138     3.00074400      824075 (+83)    138
139     3.00041200      824155 (+80)    60
140     3.00103600      824224 (+69)    71
141     3.00031200      824299 (+75)    85
142     3.00063400      824374 (+75)    69
143     3.00000000      824440 (+66)    63
144     3.00032200      824509 (+69)    78
145     3.00124616      824578 (+69)    64
146     3.00033200      824644 (+66)    66
--------------------------------------------------------
Total : 439.63570998 KMD (avrg interval : 71)
--------------------------------------------------------
Cur last block : 824709
Est next block : 824715 (6 left)
--------------------------------------------------------
Last mined : 2018-05-07 15:35 (-66 mins)
Curr Time  : 2018-05-07 16:42
--------------------------------------------------------
Mined per Hour : 2.44491080 KMD
Mined per Day  : 58.67785915 KMD
Mined per Month : 1784.78488248 KMD
--------------------------------------------------------

```
