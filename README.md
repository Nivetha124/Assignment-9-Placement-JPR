# Assignment-9-Placement-JPR

# 1 Count the number of pair of two consecutive odd number in array of N elements (non overlapping)
15
10,7,4,5,9 ,12,4,3,11,13,17,5,6,96,4
Pair of consecutive odd nos:(5,9), (3,11), (13,17)
hence O/P: 3

def count_non_overlapping_odd_pairs(n):
    count=0
    i=0
    while i<len(n)-1:
        if n[i]%2!=0 and n[i+1]%2!=0:
            count+=1
            i+=2
        else:
            i+=1
    return count
n=[10,7,4,5,9,12,4,3,11,13,17,5,6,96,4]
result=count_non_overlapping_odd_pairs(n)
print("no of non overlapping odd pairs is:",result)


# 2. Find the sum of the digits of given number until the sum becomes single digit I/p: 8939 O/p:2
8+9+3+9 is 29, then 2+9 is 11 then 1+1 is 2

def sumno(n):
    sum=0
    while n>0 or sum>9:
        if n==0:
            n=sum
            sum=0
        else:
            m=n%10
            sum+=m
            n=n//10
    return sum
n=8939
print(sumno(n))
                                                                         (OR)
def digSum(n):
    if (n == 0):
        return 0
    if (n % 9 == 0):
        return 9
    else:
        return (n % 9)
n = 8939
print(digSum(n))

# 3. Count the number of three consecutive negative number sub set in the array (non overlapping) 23,3 , -3,4,-2,-6,-7,-3,7,-3,-22,-5,34 o/p = 2
# 4. Get the string and print each characters in new line

def charprin(m):
    for i in m:
        print(i)
m=input("enter the input as a string: ")
print(charprin(m))

# 5. Print the given string in Upper Case

input=input("enter the input as a string: ")
print(input.upper())

# 6. Find the given string is palindrome or not

def ispalindrome(s):
    if s==s[::-1]:
        print("palindrome")
    else:
        print("not palindrome")
s="malay"
print(ispalindrome(s))


# 7. Count the number of letters(a-z, A-Z) in the given string Eg: “Welcome 7Eleven” o/p:13

string="Welcome 7Eleven"
alpha=0
for i in string:
    if (i.isalpha()):
        alpha+=1
print("Number of Alphabets is", alpha)

# 8. Count the unique digits in the given number Eg:235326 unique digits 2 3 5 6 so, o/p: 4







