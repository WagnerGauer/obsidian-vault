the syntax of static methods consist of the keyword static followed by the [[method definition]]. What sets these methods apart is that they can only be called by the class itself and not a [[class instance]].

class MyClass {
  static classProperty = "I am a class property";

  static staticMethod1() {
    console.log("Static method 1");
  }

  static staticMethod2() {
    console.log("Static method 2");
    console.log(MyClass.classProperty); // Accessing class property
    this.staticMethod1(); // Calling another static method
  }
}

// Calling static methods
MyClass.staticMethod1(); // Outputs: Static method 1
MyClass.staticMethod2();
// Outputs:
// Static method 2
// I am a class property
// Static method 1
