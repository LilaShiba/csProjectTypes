# Computer Science Project Guides

Welcome to the Computer Science Project Guides! This document provides an enhanced understanding of different types of projects you will encounter in this course. Each project type is described in detail and has a designated rubric to help you comprehend the expectations and assessment criteria. Refer to the relevant rubric when working on your projects.

| Type            | Description                                                | Emoji               |
|-----------------|------------------------------------------------------------|---------------------|
| Code-a-long     | Projects where you follow along with existing code         | 💻                   |
| Boiler Plate    | Projects where you build upon an existing boilerplate      | 🔧                   |
| Original        | Projects involving research and creating something new     | 🌟                   |


## Explanation of Types:

- **Code-a-long**: These projects involve following along with existing code, typically from tutorials, to learn and practice coding concepts. They focus on understanding and implementing existing solutions.

- **Boiler Plate**: These projects revolve around taking an existing boilerplate or framework and building upon it. You will enhance and customize the codebase to add new features, improve functionality, or optimize performance.

- **Original Project**: These projects involve conducting research, exploring new ideas, and creating something unique. You may need to investigate existing solutions, propose new algorithms, or develop innovative software. The emoji signifies the creative thinking and originality required for such projects.

## Rubrics

<details>
<summary>Expand to see different rubrics</summary>

### Code-a-long Rubric

| Criteria            | Description                                               |
|---------------------|-----------------------------------------------------------|
| 📚 Code Comprehension | Demonstrates understanding of the existing code and its functionality |
| ✅ Accuracy of Replication | Accurately follows the code and reproduces the expected output |
| 💡 Problem Solving   | Identifies and resolves any issues or errors encountered during coding |
| 🎨 Code Quality       | Writes clean, well-structured, and readable code |

<br>

### Boiler Plate Rubric

| Criteria            | Description                                              |
|---------------------|----------------------------------------------------------|
| 🚀 Feature Enhancement | Successfully adds new features or functionality to the codebase |
| 📈 Code Modification | Enhances the existing code to improve performance or optimize it |
| ⚠️ Error Handling   | Implements robust error handling mechanisms              |
| 📄 Documentation     | Provides clear and concise documentation for the expanded code |

<br>

### Original Project Rubric

| Criteria            | Description                                              |
|---------------------|----------------------------------------------------------|
| 🔍 Research Depth   | Demonstrates in-depth research and understanding of the topic |
| 💡 Originality      | Proposes innovative ideas or approaches                  |
| 🚀 Implementation   | Successfully implements the proposed solution or concept |
| ⭐ Impact           | Assesses the potential impact or significance of the created project |
| 📝 Explanation      | Provides a clear and comprehensive explanation of the project |
| 🎛️ Prototype       | Develops a functional prototype showcasing the project's features |
| 💻 Code Quality     | Writes clean, well-structured, and readable code         |
| 📚 Documentation    | Provides detailed documentation for the project          |
| 🗂️ Organization     | Demonstrates organized and well-structured project files and folders |
| 🔄 Iterative Development | Shows evidence of iterative development and improvement |

</details>

## Examples

### Code-a-long: Jedi Training Simulator

💻 Project Description: In this project, you will follow along with the provided code to build a Jedi Training Simulator. Using inheritance, you will create classes for different types of Jedi and Sith, each with unique attributes and abilities.

<details>
<summary>Expand</summary>

```python
class ForceUser:
    def __init__(self, name, side):
        self.name = name
        self.side = side

    def use_force(self):
        print(f"{self.name} uses the Force!")

class Jedi(ForceUser):
    def __init__(self, name):
        super().__init__(name, side="Light")
        self.lightsaber_color = "Blue"

    def use_lightsaber(self):
        print(f"{self.name} swings a {self.lightsaber_color} lightsaber!")

class Sith(ForceUser):
    def __init__(self, name):
        super().__init__(name, side="Dark")
        self.lightsaber_color = "Red"

    def use_lightsaber(self):
        print(f"{self.name} wields a {self.lightsaber_color} lightsaber!")

luke = Jedi("Luke Skywalker")
luke.use_force()          # Output: Luke Skywalker uses the Force!
luke.use_lightsaber()     # Output: Luke Skywalker swings a Blue lightsaber!

vader = Sith("Darth Vader")
vader.use_force()         # Output: Darth Vader uses the Force!
vader.use_lightsaber()    # Output: Darth Vader wields a Red lightsaber!
```
In this code, we have a base class called ForceUser, which represents individuals who can use the Force. The Jedi and Sith classes inherit from the ForceUser class and add specific behaviors and attributes. By following along with the code, you will learn about inheritance and how to create classes with unique functionalities. The project simulates a Jedi Training Simulator, where different Jedi and Sith can use the Force and wield lightsabers.

Remember to choose your preferred project type and have fun customizing your Star Wars-themed project based on your interests and learning goals! May the Force be with you! 🌟✨🚀🔧💻

</details>

### Boiler Plate: Droid Customization

🔧 Project Description: In this project, you will work with an existing codebase for a Star Wars-themed game. Your task is to expand the game by adding new droid characters with different functionalities and customizations. Use inheritance to create specialized droid classes based on the existing Droid class.

<details>
<summary>Expand</summary>

```python
  
class Droid:
    def __init__(self, name, model):
        self.name = name
        self.model = model

    def speak(self):
        print(f"{self.name} says 'Beep boop!'")

class Astromech(Droid):
    def __init__(self, name, model):
        super().__init__(name, model)
        self.abilities = ["Repairing starships", "Hacking systems"]

    def use_ability(self):
        print(f"{self.name} uses their astromech abilities to {self.abilities[0]}!")

class Protocol(Droid):
    def __init__(self, name, model):
        super().__init__(name, model)
        self.languages = ["Binary", "Human languages"]

    def speak_languages(self):
        print(f"{self.name} can speak {', '.join(self.languages)}!")

# Code execution
r2d2 = Astromech("R2-D2", "R2 series")
r2d2.speak()                    # Output: R2-D2 says 'Beep boop!'
r2d2.use_ability()              # Output: R2-D2 uses their astromech abilities to Repairing starships!

c3po = Protocol("C-3PO", "3PO series")
c3po.speak()                    # Output: C-3PO says 'Beep boop!'
c3po.speak_languages()          # Output: C-3PO can speak Binary, Human languages!
```
In this project, you will be working on expanding a Star Wars-themed game. The existing codebase includes a Droid class, and your task is to create specialized droid classes using inheritance. The Astromech class represents droids with astromech abilities, such as repairing starships and hacking systems. The Protocol class represents droids capable of speaking different languages, including binary and human languages. By expanding upon the existing codebase, you will learn how to create specialized classes and customize the game with new droid characters.

</details>

### Original: Galactic Creatures
🌟 Project Description: In this project, you have the freedom to research and create your own unique Star Wars-inspired creatures. Design and implement a hierarchy of creature classes using inheritance. Each creature should have distinct characteristics, abilities, and interactions.

<details>
<summary>Expand</summary>
  
```python3
  
  class Creature:
    def __init__(self, name, species):
        self.name = name
        self.species = species

    def introduce(self):
        print(f"I am {self.name}, a {self.species} creature!")

class JediCreature(Creature):
    def __init__(self, name, species):
        super().__init__(name, species)
        self.force_powers = ["Telekinesis", "Mind control"]

    def use_force_power(self):
        print(f"{self.name} uses {self.force_powers[0]} with great precision!")

class SithCreature(Creature):
    def __init__(self, name, species):
        super().__init__(name, species)
        self.force_powers = ["Force lightning", "Force choke"]

    def use_force_power(self):
        print(f"{self.name} unleashes a powerful blast of {self.force_powers[0]}!")

# Code execution
yoda_species = JediCreature("Yoda's Species", "Unknown")
yoda_species.introduce()                       # Output: I am Yoda's Species, an Unknown creature!
yoda_species.use_force_power()                 # Output: Yoda's Species uses Telekinesis with great precision!

nightsister = SithCreature("Nightsister", "Dathomirian")
nightsister.introduce()                        # Output: I am Nightsister, a Dathomirian creature!
nightsister.use_force_power()                  # Output: Nightsister unleashes a powerful blast of Force lightning!
```
The Galactic Creatures project provides you with a unique opportunity to delve into the vast universe of Star Wars and create your own creatures. You can research various species and create a hierarchy of classes to represent different creatures. Each class should have distinct characteristics, abilities, and interactions. This project enables you to practice inheritance and class design while exploring your creativity in designing Star Wars-inspired creatures.

</details>
