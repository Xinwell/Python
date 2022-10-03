## Assignment
### 26.9.2022
### Xin Liu
### Exercise 1
x = lambda num1,num2: num1*num2

x(5,6)
   	    
### Exercise 2
from math import pi

r = 10

area=pi*r**2

print(area)

### Exercise 3
def calculator(num1, num2,operation):

        result = None
        
        if operation == 'a':
        
            result = num1 + num2
            
        elif operation == 's':
        
            result = num1 - num2
            
        elif operation == 'm':
        
            result = num1 * num2
            
        elif operation == 'd':
        
            result = num1/num2
            
        return result
        
    if __name__ == '__main__':
    
        print(calculator(2,5,'d'))
        
### Exercise 4
class Rectangle:

        def init(self,l,w):
        
            self.length = l
            
            self.width = w
            
        def area(self):
        
            return self.length * self.width
            
    obj = Rectangle()
    
    obj.init(10,5)
    
    print('Area of Rectangle is: ',obj.area())

### Exercise 5
class Shape:

        def __init__(self,name,length):
        
            self.name = name
            
            self.length = length
            
        def area(self):
        
            return 0
            
    class Square(Shape):
    
        def __init__(self,name,length):
        
            super().__init__(name,length)
            
        def area(self):
        
            return self.length * self.length
            
        def describe(self):
        
            return 'This is a: {}'.format(self.name)
            
    if __name__=='__main__':
        s = Square('square',5)
        
        print('The area is: ')
        
        print(s.area())
        
        print(s.describe())
