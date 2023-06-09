<h1 align="center">Liskov Substitution Principle (LSP) | PHP | Example 01</h1>

<p align="center">
  <img alt="Github top language" src="https://img.shields.io/github/languages/top/faridhaghgooyan/programming-challenges?label=PHP&color=56BEB8&language=php">

  <img alt="Github language count" src="https://img.shields.io/github/languages/count/faridhaghgooyan/programming-challenges?color=56BEB8">

  <img alt="Repository size" src="https://img.shields.io/github/repo-size/faridhaghgooyan/programming-challenges?color=56BEB8">

  <img alt="License" src="https://img.shields.io/github/license/faridhaghgooyan/programming-challenges?color=56BEB8">


  <img alt="Github stars" src="https://img.shields.io/github/stars/faridhaghgooyan/programming-challenges?color=56BEB8" />
</p>


<p align="center">
  <a href="#x-bad-example">Bad Example</a> &#xa0; | &#xa0; 
  <a href="#white_check_mark-good-example">Good Example</a> &#xa0; | &#xa0;
  <a href="#memo-Sources">About Author</a> 
</p>

<br>

## :x: Bad Example ##
The bad example violates the LSP by throwing an exception in the Car class, making it unsuitable for substitution.

```bash
class Vehicle {
    public function startEngine() {
        // Start the vehicle's engine
    }
}

class Car extends Vehicle {
    public function startEngine() {
        throw new Exception('Cannot start the engine of an electric car');
    }
}

class ElectricCar extends Vehicle {
    public function startEngine() {
        // Start the electric car's engine
    }
}


```

## :white_check_mark: Good Example ##
The LSP is followed as the derived classes (Car, ElectricCar) can be substituted for their base class (Vehicle) without issues.

```bash
class Vehicle {
    public function startEngine() {
        // Start the vehicle's engine
    }
}

class Car extends Vehicle {
    public function startEngine() {
        // Start the car's engine
    }
}

class ElectricCar extends Vehicle {
    public function startEngine() {
        // Start the electric car's engine
    }
}


```




## :memo: Sources ##

- Author : Farid Haghgooyan
- [Linkedin](https://www.linkedin.com/in/farid-haghgooyan/)
- [website](https://mrhaghgooyan.com/)


<a href="#top">Back to top</a>
