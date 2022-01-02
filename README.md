# Reverse-number

class Solution:
    def reverse(self, x: int) -> int:
        t=x
        rev=0
        if t<0:
            t=-1 * t
            s=-1
        else:
            s=1    
        while (t>0):
            a=t%10
            rev= rev *10 + a
            t=t//10
            
        rev=rev * s
        if -2**31 <rev <2**31-1:
            
            return rev
        else:
            return 0 
