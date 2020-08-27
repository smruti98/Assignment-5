# Assignment-5

#2.1 Given,miles = c(65311, 65624, 65908, 66219, 66499, 66821, 67145, 67447) To find function diff,min.max and mean.
miles = c(65311, 65624, 65908, 66219, 66499, 66821, 67145, 67447)
ANSWERS..........................
diff(miles)
[1] 313 284 311 280 322 324 302
It gives the difference of two consecutive values.
min(miles)
[1] 65311
 max(miles)
[1] 67447
 mean(miles)
[1] 66371.75
 
#2.2 Given commutes=c(17,16,20,24,22,15,21,15,17,22) To find the max,min and mean function.the 24 was a mistake.
 #It should have been 18.
 ANSWERS...........................
 max(commutes)
 [1] 24
 > min(commutes)
 [1] 15
 > mean(commutes)
 [1] 18.9
 > comuutes{4}=18
 Error: unexpected '{' in "comuutes{"
 > commutes[4]=18
 > max(commutes)
 [1] 22
 > sum(commutes>=20)
 [1] 4
 > sum(commutes<=17)
 [1] 5
 (length(commutes)-sum(commutes<=17))/length(commutes)*100
 [1] 50
 
 
 #2.3 ,Given bills=c(46,33,39,37,46,30,48,32,49,35,49,35,30,48)
 ANSWERS.............................
 sum(commutes<=17)
 [1] 5
 > sum(bills)
 [1] 557
 > min(bills)
 [1] 30
 > max(bills)
 [1] 49
 > mean(bills)
 [1] 39.78571
 > sum(bills>=40)
 [1] 6
 ((length(bills)-sum(bills>=40))/length(bills))*100
 [1] 57.14286

 
 
 #2.4 Given,prices=c(9000,9500,9400,9400,10000,9500,10300,10200)
 ANSWERS....................................................
 prices=c(9000,9500,9400,9400,10000,9500,10300,10200)
 > mean(prices)
 [1] 9662.5
 > max(prices)
 [1] 10300
 > min(prices)
 [1] 9000
 
 
 #2.5 Given > x = c(1,3,5,7,9)x = c(1,3,5,7,9) y = c(2,3,5,7,11,13)
 ANSWERS............................................................
 1. x+1
 2. y*2
 3. length(x) and length(y)
 4. x + y
 5. sum(x>5) and sum(x[x>5])
 6. sum(x>5 | x< 3) # read | as 'or', & and 'and'
 7. y[3]
 8. y[-3] simpleR - Using R for Introductory Statistics
 Univariate Data page 8
 9. y[x] (What is NA?)
 10. y[y>=7]
 ANSWERS.............................
 x = c(1,3,5,7,9)
 > y=c(2,3,5,7,11,13)
 > x+1
 [1]  2  4  6  8 10
 > y*2
 [1]  4  6 10 14 22 26
 > length(x)
 [1] 5
 > length(y)
 [1] 6
 > x+y
 [1]  3  6 10 14 20 14
 Warning message:
   In x + y : longer object length is not a multiple of shorter object length
 > sum(x)
 [1] 25
 > sum(y)
 [1] 41
 > sum(x)+sum(y)
 [1] 66
 > x+y
 [1]  3  6 10 14 20 14
 Warning message:
   In x + y : longer object length is not a multiple of shorter object length
 > y+x
 [1]  3  6 10 14 20 14
 Warning message:
   In y + x : longer object length is not a multiple of shorter object length
 > sum(x>5)+sum(x[x>5])
 [1] 18
 > y[3]
 [1] 5
 > y[-3]
 [1]  2  3  7 11 13
 > y[x]
 [1]  2  5 11 NA NA
 #Here,NA means that the elements present in y in the last two positions,those elements when become order for x
and there are no elements in those orders.
>y[y>7]
[1] 11 13



##2.6> x = c(1, 8, 2, 6, 3, 8, 5, 5, 5, 5)
Use R to compute the following functions. Note, we use X1 to denote the first element of x (which is 0) etc.
1. (X1 + X2 + · · · + X10)/10 (use sum)
2. Find log10(Xi ) for each i. (Use the log function which by default is base e)
3. Find (Xi ??? 4.4)/2.875 for each i. (Do it all at once)
4. Find the difference between the largest and smallest values of x. (This is the range. You can use max and
                                                                      min or guess a built in command.)
ANSWERS.......................................................................
x = c(1, 8, 2, 6, 3, 8, 5, 5, 5, 5)
> sum(x[1:10])
[1] 48
> log(x[1:10])
[1] 0.0000000 2.0794415 0.6931472 1.7917595 1.0986123 2.0794415 1.6094379 1.6094379 1.6094379 1.6094379
> x[1:10]-4.4/2.875
[1] -0.5304348  6.4695652  0.4695652  4.4695652  1.4695652  6.4695652  3.4695652  3.4695652  3.4695652  3.4695652
> max(x)-min(y)
[1] 6
