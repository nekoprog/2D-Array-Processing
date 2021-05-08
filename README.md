# 2D-Array-Processing
Python example code for 2D Array Processing

Sample data from CAN bus stream in HEX, converted into binary form and saved into 8x8 array
```
[0x4,0x86,0x27,0x0,0x0,0x0,0x0,0x0]
```

Below is the output of the array:
```
[['0', '0', '0', '0', '0', '1', '0', '0'],
 ['1', '0', '0', '0', '0', '1', '1', '0'],
 ['0', '0', '1', '0', '0', '1', '1', '1'],
 ['0', '0', '0', '0', '0', '0', '0', '0'],
 ['0', '0', '0', '0', '0', '0', '0', '0'],
 ['0', '0', '0', '0', '0', '0', '0', '0'],
 ['0', '0', '0', '0', '0', '0', '0', '0'],
 ['0', '0', '0', '0', '0', '0', '0', '0']]
```

Array(s) can be called by row, column or row and column and converted depending on your needs
Below is the results where user needs current output speed state and output speed data

Output speed state in Array row 0, column 5, binary 0 or 1 translates to OFF and ON
```
Array[0][5]
'0' = OFF
'1' = ON
```

Output speed data in Array row 2 all column, combined to form 1 byte binary data, when converted to decimal it translates to speed in kilometer per hour (km/h)
```
Array[2]
00100111 = 39km/h
```
