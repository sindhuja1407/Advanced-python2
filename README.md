#a poultry farm has group of hens ans cows..need
#to find num of cows & hens separatly, if tottal legs & total heads together given:
#testcase 1: legs:16 heads:6 cows=2 hens=4
#testcase 2: legs:7 head :3 output : no solution
#take away
#trial and error method
#assumptions
heads=int(input("enter head:"))
legs=int(input("enter legs:"))
flag=False
for cows in range(0,heads+1):
    hens=heads-cows
    cal_legs=cows*4+hens*2
    if cal_legs==legs:
        flag=True
        break
if flag:
    print("Cows: ",cows)
    print("Hens: ",hens)
else:
    print("no solution")
