Mode
====
listOfValues = []
fileName = "GAPDHdata.txt"
with open(fileName) as f:
    next(f)
    for line in f:
        listOfValues.append(line.strip())
print "listOfValues1 =", listOfValues

header = listOfValues.pop(0).strip()
print header
print listOfValues
myData = [float(value.strip()) for value in listOfValues]
print myData

myData.sort()
print myData

def mode(myData):
    numCounter = 0
    mode = 0
    for item in myData:
       if list.count(item) > numCounter:
           numCounter = list.count(item)
           mode = item
           return mode
           print mode(list)
