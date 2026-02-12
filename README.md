# NumberReverser
Reverse Number
class NumberReverser(object):
    def __init__(self, num):
        self.num = num

    def reverse_number(self):
        n = self.num
        rev = 0
        while n>0:
            rev = rev * 10 + (n % 10)
            n = n // 10
        return rev

number = 5873
number_reverser = NumberReverser(number)
print(number_reverser.reverse_number())