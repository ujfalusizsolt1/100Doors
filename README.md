# 100Doors
doors = [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0]
counter = 1
currentstep = 0
while currentstep < 100:
    for counter in doors:
        if doors[counter - 1] == 0:
            doors[counter - 1] = 1
        elif doors[counter - 1] == 1:
            doors[counter - 1] = 0
        counter = counter + currentstep
    counter = 0
    currentstep = currentstep + 1
print("The following doors are open: ")
while counter < 100:
    if doors[counter] == 1:
        print(counter, ", ")
    counter = counter + 1
