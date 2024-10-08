# Learn-Java-Building-Cars
Learn the basic concepts of Java by building a car system.

## Challenge 1: Create a Car and Update Mileage
**Objective:** Create a car and update its mileage.

1. Define a `Car` class with the following attributes:
   - `name` (String)
   - `mileage` (double)

2. Create an instance of `Car`, set its name and initial mileage.
3. Add a method `addMileage(double miles)` to update the mileage.
4. In the main program, create a `Car`, call the `addMileage` method to add some miles, and then print out the new mileage.

---

## Challenge 2: Print the Change in Mileage
**Objective:** Calculate and print the change in mileage without storing it directly in the class.

1. Before updating the mileage, capture the current mileage in a local variable.
2. After calling `addMileage()`, calculate the change by subtracting the old mileage from the new mileage and print the result.

---

## Challenge 3: Create Multiple Cars and Print Their Details
**Objective:** Create multiple `Car` objects and print their name and mileage using a loop.

1. Create several instances of the `Car` class (e.g., Mini, Corsa, Fiat).
2. Store them in an array or list.
3. Use a `for` loop to iterate through the cars and print their names and current mileage.

---

## Challenge 4: Get User Input - Allow a New Car to be Added by a User
**Objective:** Introduce user input to add a new car.

1. Prompt the user to enter the name and mileage of their car.
2. After getting input, create a `Car` object with the entered values.
3. Print the message: `"You added a new car with the name of [ENTER NAME] and mileage of [ENTER MILEAGE]."`

**Hints:**
- How to read user input from the console: [GeeksforGeeks Console Readline](https://www.geeksforgeeks.org/console-readline-method-in-java-with-examples/)
- How to log variables using string interpolation (plus operator): [Baeldung String Interpolation](https://www.baeldung.com/java-string-interpolation)

---

## Challenge 5: Add Multiple Cars
**Objective:** Allow the user to keep adding multiple cars.

1. Modify the program to keep the console open and keep prompting the user to add cars.
2. Each time the user enters the details for a car, create a new `Car` object and store it in a list.
3. After each addition, print all cars currently in the list with their mileage.

---

## Challenge 6: Add an Exit Option
**Objective:** Create an exit option for the user.

1. Modify the program so that if the user enters the letter `'q'` when asked for the car name, the program exits.
2. If the user doesn’t enter `'q'`, the program continues prompting for new cars.

---

## Challenge 7: [ADVANCED] Add a Dependency (Owner - Person Class)
**Objective:** Introduce the concept of dependencies between classes by creating an `Owner` (Person) class and linking it to the `Car` class.
Hint - https://medium.com/@aydinserbest34/understanding-dependencies-in-object-oriented-programming-and-testing-7e9059f54561
### Steps:

1. **Create a `Person` class**:
   - The `Person` class should have the following attributes:
     - `name` (String)
     - `age` (int)

2. **Modify the `Car` class**:
   - Add an attribute `owner` to the `Car` class that stores a `Person` object.
   - When creating a `Car` object, allow an owner to be assigned (either via constructor or method).

3. **Modify user input**:
   - When adding a new car, ask for the owner’s name and age.
   - Create a `Person` object for the owner and assign it to the car.

4. **Display the owner's information**:
   - When printing the car’s details, also print the owner’s name and age.

---

## Challenge 8: [ADVANCED] Create Subclasses of Cars
**Objective:** Introduce inheritance by creating different types of cars (e.g., ElectricCar, GasCar) that extend the `Car` class.
Hint - https://www.w3schools.com/java/java_inheritance.asp
---

### Steps:

1. **Create the `ElectricCar` subclass**:
   - Extend the `Car` class to create an `ElectricCar` class.
   - Add an attribute `batteryLevel` (double) to represent the percentage of battery left.
   - Override the `addMileage()` method to reduce the battery level when the car drives.

2. **Create the `GasCar` subclass**:
   - Extend the `Car` class to create a `GasCar` class.
   - Add an attribute `fuelLevel` (double) to represent the amount of fuel left in the tank.
   - Override the `addMileage()` method to reduce the fuel level when the car drives.

3. **Modify user input**:
   - When creating a car, ask the user if they want to create an `ElectricCar` or a `GasCar`.
   - Create the appropriate car type based on the user’s choice.

4. **Display the car’s type**:
   - Modify the `displayDetails()` method in both subclasses to include information about the battery level (for electric cars) or fuel level (for gas cars).

---

