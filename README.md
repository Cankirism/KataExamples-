# KataExamples-
https://www.codewars.com examples solutions

# 1- Two to One Examples : 
Take 2 strings s1 and s2 including only letters from ato z. Return a new sorted string, the longest possible, containing distinct letters,</br>

each taken only once - coming from s1 or s2. #Examples: ``` a = "xyaabbbccccdefww" b = "xxxxyyyyabklmopq" longest(a, b) </br>  -> "abcdefklmopqwxy"
a = "abcdefghijklmnopqrstuvwxyz" longest(a, a) -> "abcdefghijklmnopqrstuvwxyz" ``` </br>
<b >Solution in Python </b> </br>
def longest(s1, s2):</br<
    tumu = s1 + s2 </br>
    tekil ='' </br>
    for a in tumu : </br>
        if a not in tekil : </br>
            tekil = tekil + a </br>
        
    return ''.join(sorted(tekil))    

