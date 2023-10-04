The most common class method is the [[constructor method]]. 
Other kinds of methods which can be defined in a [[class definition]] include [[instance methods]], [[static methods]], [[getter methods]], and [[setter methods]]. 







class Person {
  constructor(firstName, lastName) {
    this.firstName = firstName;
    this.lastName = lastName;
    this.fullName = `${this.firstName} ${this.lastName}`
  }
}

const person = new Person("John", "Doe");
console.log(person.fullName); // Accessing the getter method
