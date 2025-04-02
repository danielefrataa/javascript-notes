
Hello! this is my recap to deep understanding fundamental JavaScript. 

## OOP (Object Oriented Programming)

### Inheritance

*An object is a real-world entity, while a class is a blueprint or template used to create objects.*

Class = Definition (it's Like a recipe)
Object = Concrete instance (like a cake made from the recipe)

Constructor functions are a fundamental concept in OOP, especially in JS which originally didn't have class syntax. Construtors provide a way to create objects and implement class-like behavior ES6 the   *class* keyword

Here's key concept: 
1. Extends -> mewarisi class
2. super () -> memanggil/method parent wajib di subclass
3. this -> hanya bisa digunakan super () constructor inheritance

diffrent beetwen super() vs super. 
1. Super () hanya untuk inisiasi child class.
2. Super. it called method from parent class

Best practice
- Always call super() first in child constructors.
- Favor composition over deep inheritance (avoid "inheritance chains" like A → B → C → D).
- Use super.method() to extend (not replace) parent methods.
- Avoid overriding constructors unless necessary.

        class Admin extends User {
        login() {
            super.login(); // Keep parent logic
            console.log("Admin logged in");
        }
        }



### Polymorishm 
