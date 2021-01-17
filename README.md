# queus-ds
class stack:
    def __init__(self):
        self.list = []
        self.top = -1
        self.max = 5
    def isempty(self):
        if self.top == -1:
            return True
        else:
            return False
    def isfull(self):
        if self.top == self.max - 1:
            return True
        else:
            return False
    def push(self,data):
        if self.isfull():
            print('stack is overflow')
        else:
            self.top += 1
            self.list.append(data)
            print(self.list)
    def pop(self):
        if self.isempty():
            print('the stack is underflow')
        else:
            self.top -= 1
            self.list.pop()
            print(self.list)

s = stack()
s.push(10)
s.push(8247)
s.push(102)
s.push(13)
s.push(2510)
s.push(10)


