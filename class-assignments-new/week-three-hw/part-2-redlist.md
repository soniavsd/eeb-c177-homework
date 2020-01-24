1. Count the number of occurences for each cat
grep -c "species code" European_Red_List.csv
EX: 29
RE: 8
CR: 464
EN: 687
VU: 885
NT: 964
LC: 58
DD: 2409
NA 411
2. Only consider birds
grep AVES European_Red_List.csv | grep -c "species code"
EX: 2
RE: 15
CR: 13
EN: 19
VU: 39
NT: 32
LC: 438
DD: 0
NA 41
3. For each order of birds, compute # of extinct/near extinct (EX, RE, CE)

grep AVES European_Red_List.csv | cut -d "," ..... I couldn't figure out
this one
