def postfix(s):
    s=s.split()
    n=len(s)
    stack=[]
    for i in range(n):
        if s[i].isdigit():
            stack.append(int(s[i]))
        elif s[i]=='+':
            a=stack.pop()
            b=stack.pop()
            stack.append(int(b)+int(a))
        elif s[i]=='-':
            a=stack.pop()
            b=stack.pop()
            stack.append(int(b)-int(a))
        elif s[i]=='*':
            a=stack.pop()
            b=stack.pop()
            stack.append(int(b)*int(a))
        elif s[i]=='/': 
            a=stack.pop()
            b=stack.pop()
            stack.append(int(b)/int(a))
            return stack.pop()
s="2.8 *"
v=postfix(s)
print(v)
