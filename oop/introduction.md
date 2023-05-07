# Object Oriented Programming

## Objects
Objects have poperties and methods. Exemples:

    const books = [
        {
            title: "Book 1",
            category: "Science",
            author: "Mark",
            read: function () {
                console.log(`Reading ${this.title}`)
            }
        }
    ]

Some objects is more difficult to understand, because they are abstracts, like:
- Authentication
- Authorization

## Class
A class allows you to create multiple instanced objects. All objects created from a class inherit the class's prototype, as well as its properties and methods. Exemple:

    class Rectangle {
        constructor(width, height) {
            this.width = width;
            this.height = height;
        }

        area() {
            return this.width * this.height;
        }
    }

## Encapsulation
Encapsulation is a fundamental concept in object-oriented programming that refers to the practice of bundling data and behavior within a single unit, typically a class or an object. This helps to hide the implementation details of the class or object from the outside world, and provides a way to ensure that the data is accessed and modified in a controlled manner. Exemple: 

    const person = {
        name: 'John Doe',
        age: 30,
        getAge: function() {
            return this.age;
        },
        setAge: function(newAge) {
            this.age = newAge;
        }
    };

    console.log(person.getAge());