# ATM-Program

while True:
   balance=10000
   print(" ATM " )
   print("""
   1)         balance
   2)         withdraw
   3)         Deposit
   4)         Quit  
   """)
   try:
     Option=int(input("Enter option:"))
   except Exception as e:
       print("Error", e)
       print("Enter 1,2,3 or 4 only")
       contiune
   if Option==1:
       print("Balance ",balance)
   if Option==2:
       print("Balance ",balance)
       Withdraw = float(input("Enter Withdraw amount"))
    
       if Withdraw>0: 
           forewardbalance = (balance-Withdraw)
           print("foreward Balance ",forewardbalance)    
       elif withdraw>balance:
           print("No funs in account")
       else:
           print("None withdraw made")
   if Option==3:
       print("Balance ", balance)
       Deposit = float(input("Enter deposit amount"))
       if Deposit>0:
           forewardbalance=(balance+Deposit)
           print("forewardbalance" , forewardbalance)
       else:
           print("None deposit made")
   if Option==4:
    exit()
