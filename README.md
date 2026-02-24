# NumberReverser
Reverse Number
class NumberReverser(object):
    def __init__(self, num):
        self.num = num

    def reverse_number(self):
        n = self.num
        if n < 0:
            n = -n
        rev = 0
        while n > 0:
            rev = rev * 10 + (n % 10)
            n //= 10
        if self.num < 0:
            rev = -rev
        return rev

number = -9876567788769987656788
number_reverser = NumberReverser(number)
print(number_reverser.reverse_number())
