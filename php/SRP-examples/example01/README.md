<h1 align="center">Single Responsibility Principle(SRP) | PHP | Example 01</h1>

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
the UserManager class has an additional responsibility of sending emails, violating the SRP.

```bash
class UserManager {
    public function createUser($userData) {
        // Create user logic
    }
    
    public function deleteUser($userId) {
        // Delete user logic
    }
    
    public function updateUser($userId, $newData) {
        // Update user logic
    }
    
    public function sendEmail($userId, $message) {
        // Sending email logic
    }
}
```

## :white_check_mark: Good Example ##


```bash
class UserManager {
    public function createUser($userData) {
        // Create user logic
    }
    
    public function deleteUser($userId) {
        // Delete user logic
    }
    
    public function updateUser($userId, $newData) {
        // Update user logic
    }
}
```




## :memo: Sources ##

- Author : Farid Haghgooyan
- [Linkedin](https://www.linkedin.com/in/farid-haghgooyan/)
- [website](https://mrhaghgooyan.com/)


<a href="#top">Back to top</a>
