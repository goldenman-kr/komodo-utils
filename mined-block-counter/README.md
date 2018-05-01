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
$ ./nodeMined
```

------------------------

## Example
```
$ ./nodeMined
Loading blockchain info...please wait...
---------------------------------------------
num     Height  Amount
---------------------------------------------
1       814258  3.00081282
2       814325  3.00016875
3       814392  3.00001000
4       814458  3.00000000
5       814524  3.00000000
6       814590  3.00000000
7       814664  3.00000000
8       814730  3.00000000
9       814800  3.00001000
10      814867  3.00064090
11      814938  3.00042600
12      815005  3.00066000
13      815072  3.00002000
14      815139  3.00001000
15      815205  3.00000000
16      815272  3.00121513
17      815339  3.00002000
18      815405  3.00001000
19      815471  3.00030000
20      815539  3.00000000
21      815605  3.00000000
22      815672  3.00032200
23      815738  3.00000000
---------------------------------------------
Total : 69.00462560
---------------------------------------------
```
