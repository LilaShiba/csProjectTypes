# Computer Science Project Guides

Welcome to the Computer Science Project Guides! This document provides an enhanced understanding of different types of projects you will encounter in this course. Each project type is described in detail and has a designated rubric to help you comprehend the expectations and assessment criteria. Refer to the relevant rubric when working on your projects.

| Type            | Description                                                | Emoji               |
|-----------------|------------------------------------------------------------|---------------------|
| Code-a-long     | Projects where you follow along with existing code         | 💻                   |
| Boiler Plate    | Projects where you build upon an existing boilerplate      | 🔧                   |
| Original        | Projects involving research and creating something new     | 🌟                   |


## 📋 Rubrics 📋

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

## 🧪 Examples 🧪

Take a look at how one topic can support all 3 types of projects!


<details>
<summary>Expand</summary>

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
</details>



# 🏗️ Project  Structuring 🏗️

Choosing the right project, structuring it, and building a realistic timeline are key to a successful coding journey. Here's a step-by-step guide on how to approach this process:
<details>
<summary>Expand</summary>
    
### 1. Project Selection 🎯

In the Jedi Training Simulator, you will find a variety of projects. From "Jedi Fundamentals" to "Galactic Creatures", each project is unique and provides a different set of challenges. Pick a project that aligns with your interests and the skills you want to develop. Remember, there's no right or wrong choice; it's about choosing a project that motivates you!

### 2. Project Structuring 🏗️

Once you've selected your project, the next step is to structure it:

* **Understand the Problem:** Read the project description carefully and understand what it is asking you to do. You can't solve a problem you don't understand!

* **Identify Key Components:** Break down the project into smaller, manageable tasks. For example, if you chose the "Droid Customization" project, you might break it down into tasks like "Create Droid class", "Create specific Droid sub-classes", etc.

* **Plan Your Code:** Before you start coding, think about the design of your program. What classes do you need? How will they interact with each other?

### 3. Timeline Building 🗓️

Creating a realistic timeline can help you manage your time effectively:

* **Estimate Time for Each Task:** Try to determine how long each task in your project will take. Remember, it's better to overestimate than underestimate.

* **Prioritize Tasks:** Some tasks will be more important than others. Prioritize based on dependencies (some tasks can't be done until others are completed), difficulty, and importance.

* **Set Milestones:** Set targets for when you want to complete each task. Be sure to include some buffer time for unforeseen challenges or delays.

<details>
<summary>Expand</summary>

Here's an example of what your project breakdown and timeline might look like:

**Project:** Droid Customization

**Tasks:**
1. Create Droid class (Estimated time: 1 day)
2. Create specific Droid sub-classes (Estimated time: 2 days)
3. Implement droid abilities (Estimated time: 1 day)
4. Test and debug (Estimated time: 2 days)

**Timeline:**
- Day 1: Task 1
- Day 2-3: Task 2
- Day 4: Task 3
- Day 5-6: Task 4

</details>

Remember, coding is an iterative process. You might not get everything right the first time, and that's okay! The most important thing is to keep learning and improving. May the Force be with you!
</details>

##  ✅ Project Approval Process ✅

Before you begin coding your selected project, you'll need to get your project timeline approved. This process ensures that you've thought through your project plan and that you're ready to start coding.

Follow these steps for the project approval process:

<details>
<summary>Expand</summary>
    
### 1. Create Project Proposal 📝

Once you've chosen a project and have structured it along with a timeline, the next step is to prepare a project proposal. This proposal should include:

- **Project Title**: The name of the project you've chosen.
- **Project Description**: A brief summary of what the project is about.
- **Task Breakdown**: A list of the tasks you plan to complete, broken down into manageable chunks.
- **Timeline**: An estimated timeline for each task.

Your proposal might look something like this:

```markdown
    
**Project Title:** Droid Customization

**Project Description:** This project involves expanding an existing codebase to add new Droid characters with unique functionalities to a Star Wars-themed game.

**Task Breakdown:**
1. Create Droid class
2. Create specific Droid sub-classes
3. Implement Droid abilities
4. Test and debug

**Timeline:**
- Day 1: Create Droid class
- Day 2-3: Create specific Droid sub-classes
- Day 4: Implement Droid abilities
- Day 5-6: Test and debug
```
    
2. Submit Project Proposal 📥
Once you've created your project proposal, submit it for approval. Be sure to check for any feedback or suggestions!

3. Incorporate Feedback 🔄
You may receive feedback on your project proposal. This can be about the feasibility of the tasks, the estimated time, or the overall structure of the project. Incorporate the feedback into your proposal. This iterative process will help you refine your project planning skills.

4. Get Approval 🎉
Once your proposal meets all the requirements and you've incorporated any necessary feedback, you'll receive approval to start coding!

Remember, the project approval process is a learning experience designed to enhance your project planning skills. May the Force be with you!

</details>
