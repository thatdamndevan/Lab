tup = ()
print("*insertion sort*")
n=int(input("enter total number of elements:  "))
for i in range(n):
        tup+=(int(input("enter worms to enter to tuple:  ")),)
print("original is: ",tup)
lst=list(tup)
for i in range(1,n):
        temp=lst[i]
        j=i-1
        while(j>=0 and temp>lst[j]):
                lst[j+1]=lst[j]
                j = j-1
        lst[j+1]= temp
print("sorted tuple is:  ", tuple(lst))
