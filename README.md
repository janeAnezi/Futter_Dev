# Futter_Dev

# Dart Intro
void main() {  // a function that does not require the "return" before execution
    <!-- creating variables -->
  String name = "jane";
  bool isReady = true;
//   name = 20;
  print(name);
  print(isReady);
  
  
  String greeting = greet();
  print(greeting);
  
  int age = getAge();
    print(age);
  
  List names = ['blessing', 'precious', 'ahnnie']; // arrays
  names.add('love');
  names.remove('blessing');
  print(names);
  
  List<int> ages = [20,45,26,12];
  ages.add(25);
  print(ages);
  
  User userOne = User('Grace', 20);
  
  print(userOne.userName);
  print(userOne.age);
  userOne.message();
  
  superUser userThree = superUser('Ahnnie', 11);
  print(userThree.userName);
  userThree.publish();
  
}


String greet() { // function type String
  return('Hello');
}

int getAge() => 22; // function tye Integer

class User { // objects in dart
  String userName;
  int age;
  
  User(String userName, int age) {
    this.userName = userName;
    this.age = age;
    
  }
  
  void message() { // method in object
    print('User Logged in');
  }
}

class superUser extends User {  linking the user object to superuser object
  superUser(String userName, int age) : super(userName, age);
  
  void publish() {
    print('published');
  }
  
}




