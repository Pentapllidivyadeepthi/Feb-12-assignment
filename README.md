# Feb-12-assignment
dal=100
wf=90
soap=20
surf=200
rice=600
cno=int(input('enter customer number :'))
cname=input('enter customer name :')
dalq=int(input('enter no.of packets of dal:'))
wfq=int(input('enter no.of wheat flour packets:'))
soapq=int(input('enter no.of soaps:'))
surfq=int(input('enter no.of surf packets:'))
riceq=int(input('enter no.of rice bags:'))
bill=(dal*dalq)+(wf*wfq)+(soap*soapq)+(surf*surfq)+(rice*riceq)
print('bill',bill)
if bill>3000 :
    tax=bill*10/100
    print('tax',tax)
    if bill>=5000 :
        dis=bill*10/100
        print('dis',dis)
    else :
        dis=bill*8/100
        print('dis',dis)
else :
    tax=bill*18/100
    print('tax',tax)
    if bill>2000 :
        dis=bill*5/100
        print('dis',dis)
    elif bill>1000 :
        dis=bill*3/1000
        print('dis',dis)
    else :
        dis=0
mainbill= bill+tax-dis
print("bill amount is :",mainbill)
