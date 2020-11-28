unitslist=["0","I","II","III","IV","V","VI","VII","VIII","IX"]
tenslist=["0","X","XX","XXX","XL","L","LX","LXX","LXXX","XC"]
hundredslist=["0","C","CC","CCC","CD","D","DC","DCC","DCCC","CM","M"]


while True:
 inputnumber=int(input('Enter the number you want to translate to Roman numeral:'))

 hq=int(inputnumber/100)
 roman = hundredslist[hq] 
 hr=inputnumber%100
 tq=int(hr/10)
 roman = roman + tenslist[tq]
 tr=hr%10
 roman = roman + unitslist[tr]
 print('Your Roman numeral is ',roman, '\n')
