#罗马数字转整数
![timu] (https://github.com/huanyk/leetcode/blob/master/Roman.jpg)
class solution:
    def romanToInt(self,s:str)->int:!
        a={'I':1}
        ans=0
            for i in range(len(s)):
                if i<len(s)-1 and a[s[i]]<a[s[i+1]]:
                    ans-=a[s[i]]
