# BASIC MATHEMATICS

## 1. EXTRACTION OF DIGITS
To get last digit : n%10
To remove last digit : n/10

-----------PSEUDOCODE-----------
while(n>0){
  last_digit = n%10
  n=n/10
}  

Time complexity : O(log10 (n))   --->log because % and / (division is used)

Another method for number of digits : (int)(log10(n)+1)

-----------------------------------------------------------------------------------------------------------------------------

## 2. REVERSE NUMBER
revnum = (revnum*10)+lastdigit

-----------------------------------------------------------------------------------------------------------------------------

## 3. PALINDROME NUMBER
cn = n ------>duplicate the number
if(cn==revnum) then palindrome

-----------------------------------------------------------------------------------------------------------------------------

## 4. ARMSTRONG NUMBER
Sum of cubes of digits give the number itself
eg: 371 ---> (3*3*3)+(7*7*7)+(1*1*1) = 371

sum = sum+(ld*ld*ld)  ---->ld=last_digit

-----------------------------------------------------------------------------------------------------------------------------

## 5. ALL DIVISORS
for(i=0; i<n; i++){
  if(n%i == 0){
    print(i)
  }
}

Time complexity = O(n)
-------------------------------
for(i=0; i*i<=n; i++){
  if(n%i == 0){
   print(i)
   if((n/i) != i){
     print(n/i)
   }
  }
}

Time complexity : O(sqrt(n))

then store it in list and sort it.

NOTE  : n = 1000000 iterations then sqrt(n) = 1000 iterations

-----------------------------------------------------------------------------------------------------------------------------
