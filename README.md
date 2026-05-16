# python-oops-concepts
Python programs demonstrating classes, objects, constructors, inheritance, encapsulation, polymorphism, and method overriding using Object-Oriented Programming concepts.
# OOP Concepts in Python

# Base Class
class Animal:

    # Constructor
    def __init__(self, name):
        self.name = name

    # Method
    def sound(self):
        print("Animal makes a sound")


# Inheritance + Method Overriding
class Dog(Animal):

    def sound(self):
        print(self.name, "barks")


class Cat(Animal):

    def sound(self):
        print(self.name, "meows")


# Encapsulation
class Student:

    def __init__(self, name, marks):
        self.name = name
        self.__marks = marks   # Private variable

    def display_marks(self):
        print("Marks:", self.__marks)


# Polymorphism
def animal_sound(animal):
    animal.sound()


# Objects Creation
dog = Dog("Tommy")
cat = Cat("Kitty")

# Calling Methods
animal_sound(dog)
animal_sound(cat)

# Encapsulation Example
s1 = Student("Deepak", 95)
print("Student Name:", s1.name)
s1.display_marks()
