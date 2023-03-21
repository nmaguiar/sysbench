./sysbench memory run | sed -n '/---/,$p' | ojob ojob.io/formats/map format=yaml 

./sysbench cpu run | sed -n '/---/,$p' | ojob ojob.io/formats/map format=yaml

./sysbench fileio run --file-test-mode=rndrd | sed -n '/---/,$p' | ojob ojob.io/formats/map format=yaml

./sysbench threads run | sed -n '/---/,$p' | ojob ojob.io/formats/map format=yaml
