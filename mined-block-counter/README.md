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
$ ./getMined 15
Loading blockchain info...please wait...(numOfList:15)
--------------------------------------------------------
num     Amount          Height          Time Interval(M)
--------------------------------------------------------
1       3.00081282      814258  -----
582     3.00062400      855809 (+66)    65
583     3.00186595      855875 (+66)    81
584     3.00005000      855962 (+87)    75
585     3.00046200      856107 (+145)   145
586     3.00094600      856173 (+66)    71
587     3.00000000      856239 (+66)    71
588     3.00000000      856305 (+66)    57
589     3.00000000      856371 (+66)    92
590     3.00000000      856438 (+67)    44
591     3.00069620      856505 (+67)    60
592     3.00031200      856573 (+68)    75
593     3.00048380      856683 (+110)   116
594     3.00044053      856749 (+66)    84
595     3.00124800      856815 (+66)    55
596     3.00134800      856881 (+66)    60
--------------------------------------------------------
Largest: 9.22554397 KMD
Average: 3.02991846 KMD
Total  : 1805.83140078 KMD (avrg interval : 71)
--------------------------------------------------------
Last my reward : 856881 (53 ago)
Cur last block : 856934
Est next block : 856952 (18 left)
--------------------------------------------------------
Last mined : 2018-05-30 12:15 (-46 mins)
Curr Time  : 2018-05-30 13:02
--------------------------------------------------------
Mined per Hour : 2.49080193 KMD
Mined per Day  : 59.77924637 KMD
Mined per Month : 1818.28541044 KMD
--------------------------------------------------------

```
