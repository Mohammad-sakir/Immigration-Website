# Immigration-Website
#Coding Challenge 1(Nested List)#

from __future__ import print_function

score_list = {}

for _ in range(input()):

    name = raw_input()    
    score = float(raw_input())   
    if score in score_list:   
        score_list[score].append(name)         
    else:    
        score_list[score] = [name]      
        
new_list = []

for i in score_list:

    new_list.append([i, score_list[i]])
    
new_list.sort()

result = new_list[1][1]

result.sort()

print (*result, sep = "\n")



#Coding Challenge 2(Python-lists)#


arr = []

for i in range(int(raw_input())):

    s = raw_input().split()      
    for i in range(1,len(s)):       
        s[i] = int(s[i])         
    if s[0] == "append":       
        arr.append(s[1])           
    elif s[0] == "extend":      
        arr.extend(s[1:])           
    elif s[0] == "insert":      
        arr.insert(s[1],s[2])           
    elif s[0] == "remove":       
        arr.remove(s[1])            
    elif s[0] == "pop":       
        arr.pop()            
    elif s[0] == "index":       
        print arr.index(s[1])          
    elif s[0] == "count":     
        print arr.count(s[1])          
    elif s[0] == "sort":       
        arr.sort()             
    elif s[0] == "reverse":      
        arr.reverse()           
    elif s[0] == "print":        
        print arr
        
        
        
##**Coding Challenge 3(Division)**##

from __future__ import division

if __name__ == '__main__':

    a = int(raw_input())    
    b = int(raw_input())
    p = int(a/b)
    n = float(a/b)
    print p
    print n
