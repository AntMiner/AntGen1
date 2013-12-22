
This is cgminer application for AntMiner USB miner.


AntMiner USB miner options:

--bmsc-options <115200:timeout> Set antminer U1 configurations

--bmsc-freq <arg> Set ASIC clock frequency


  argment --bmsc-options <baud:to>

  baud value should be 115200

  to sets the timeout value: to*100ms. timeout value should be less than: (2^32)/(freq*8)


  argment --bmsc-freq <freq>

  0581 : 150M
  0681 : 175M
  4F02 : 193M
  0781 : 200M
  0881 : 225M
  0981 : 250M
  0A81 : 275M
  0B81 : 300M
  0C81 : 325M
  0D81 : 350M
  0E81 : 375M
  0F81 : 400M
  5081 : 425M
  5181 : 450M
  5281 : 475M
  5381 : 500M


Example:

run at default clock frequency(4F02, 193.75), timeout is 2s

cgminer.exe --bmsc-options 115200:20 -o pool_url -u user -p password


run at default 200M clock frequency, timeout is 2s

cgminer.exe --bmsc-options 115200:20 -o pool_url -u user -p password --bmsc-freq 0781

