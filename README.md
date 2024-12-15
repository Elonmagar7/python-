# Simple Python Program to do basic Arithmetic operation between 2 numbers

num1=int(input("Enter any number ="));
num2=int(input("Enter any number ="));
operator=int(input("Enter any number in betn(1-5) for addn,subtrcn,divisn,multiplicn,mod respectively  ="));
while operator<1 or operator>4:
       print(f"{operator} isn't in betn 1-4.")
       operator=int(input("Enter number in between 1 and 4 again= "))
if operator==1:
    sum=num1+num2
    print("Addition = ",sum)
elif operator==2:
    sub=abs(num1-num2)
    print("Subtraction = ",sub)
elif operator==3:
    div=num1/num2
    print(f"Quotient = {div:.2f}")
elif operator==4:
    mul=num1*num2
    print("Multiplication = ",mul)
elif operator==5:
    rem=num1%num2
    print("Remaindern = ",rem)


# program by Using the Anynomous lambda function inside a function

#Program type-1
def func(fx,v):
   return fx(v)
arb= lambda n:n**3
n= int(input("Enter any number = "))
print("The Cube of Entered number is : ",func(arb,n))

#program type-2
def f(v):
   return lambda n:n*v
ar=f(3)
num=int(input("Enter any number ="))
print(f"The  3 time  of {num}  = {ar(num)}")


  

