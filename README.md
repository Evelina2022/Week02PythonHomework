# Week02Python_Homework
In Week01 homework we developed a project "Multiplication for Kids".

Add the new features to your project. Add features working with Git and GitHub.

1) After student completed the test display the number of correctly answered questions

2) Assume that the passing level is 7 correct answers out of 10 questions, and display the test outcome pass or fail

3) Display 10 question summary. In the summary you need to display each question from the test. For every question you need to display:

```text
    - question number
    - question
    - student's answer
    - correct answer
    - answer status (CORRECT or WRONG)
```
Example:

*** SUMMARY ***

Q1: 2 x 3 = ?; Student Answer: 6; Answer: 6; Status: CORRECT
Q2: 6 x 8 = ?; Student Answer: 56; Answer: 48; Status: WRONG

from random import  randint  

```def main():
        correct= 0 

        questions = 0

        for questions in range(10):
            num_1 = randint(1,10)
            num_2 = randint(1,10)
            questions += 1


            print("Q",questions,":", num_1 ,"X",num_2,"?")  
            answer = int(input("Student Answer: "))

            if answer == num_1*num_2:
                print("Answer: ",num_1*num_2,"Status: CORRECT")
                correct += 1 

            else:
                print("Answer: ",num_1*num_2," Status: WRONG")

        if correct >= 7:
            print("Test passed")
        else:
            print("Test failed try again!!!")


        print("The number of points received are", correct, "out of", questions)
  ```main()

