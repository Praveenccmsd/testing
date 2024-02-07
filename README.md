# Effective UI Test Automation With Serenity BDD and Selenium - Course Exercises

This repository contains the sample code for the [Effective UI Test Automation With Serenity BDD and Selenium](https://www.udemy.com/course/serenity-bdd-web-testing/?referralCode=3E5878CF6F4676EF507B) course on Udemy. Each module in the course has two branches, a starting point and a solution. (These branches are mentioned in each module as you do them).

The [Effective UI Test Automation With Serenity BDD and Selenium](https://www.udemy.com/course/serenity-bdd-web-testing/?referralCode=3E5878CF6F4676EF507B) teaches the fundamentals of UI Test Automation with Serenity BDD, and will give you a unique insight on how to use Serenity BDD the way it is intended. You'll discover:

* How to write well-structured automated web tests with Serenity BDD, to maximise reuse and minimise maintenance costs
* How to use Page Objects and Action Classes to make your test code more concise and more expressive, so you can write tests faster AND spend less time maintaining them later on;
* How to write effective locators using XPath and CSS, including Serenity BDD's powerful dynamic locators
* How to handle waits and asynchronous applications in Serenity BDD
* How to use data-driven testing with Serenity to get higher coverage and better reporting
* How to run tests in parallel and get feedback faster
* How to run your Serenity BDD tests remotely on Selenium Grid and services such as SauceLabs and BrowserStack.
* How to tailor your Serenity BDD reports, so they tell your stakeholders EXACTLY what they need to know
* And much more

By the end of the course, you'll be able to build automated testing frameworks for your web applications quickly and effectivly from scratch, harnessing the full power of Serenity BDD.

# TodoMVC Exercise

In this exercise, you will complete a series of simple tests against the [TodoMVC](https://todomvc.com/examples/angularjs/#/) application using core Serenity BDD features.

You can see a [sample solution for this exercise here](https://github.com/serenity-dojo/serenity-web-training/tree/todomvc-solution).

You can also see the sample report generated by Github actions here:
* [Main Serenity Report](https://serenity-dojo.github.io/serenity-web-training)
* [Serenity Summary Report](https://serenity-dojo.github.io/serenity-web-training/serenity-summary.html)

## Get the code

Git:

    git clone https://github.com/serenity-dojo/serenity-web-training/tree/todomvc-start
    cd serenity-junit-starter
    git checkout todomvc-start
    git checkout -b my-todomvc-exercise

You will find the tests to implement in the `WhenAddingTasks` and `WhenCompletingATask` classes.

## Exercise 1

Open the `WhenAddingTasks` and implement the `addingASingleTask()` method. Use a Serenity action class to implement the steps. Make sure the steps and assertions appear in the reports.

## Exercise 2

Open the `WhenAddingTasks` and implement the `addingMultipleTasks()` method. You can reuse methods developed in the previous exercise.

## Exercise 3

Open the `WhenCompletingATask` class and implement the `activeTasksShouldNotShowCompletedTasks()` method.

## Exercise 4

Open the `WhenCompletingATask` class and implement the `completedTasksShouldNotShowActiveTasks()` method.

## Exercise 5

Open the `WhenDeletingATask` class and implement the `deletedItemsShouldDissapearFromTheList()` method.

## Exercise 6
Write a data-driven test to test the following scenarios:
* When you add the items "Feed the cat" and "Walk the dog", and complete "Feed the cat", and then filter by "Completed", you should only see "Feed the cat"
* When you add the items "Feed the cat" and "Walk the dog", and complete "Feed the cat", and then filter by "Active", you should only see "Walk the dog"
* When you add the items "Feed the cat" and "Walk the dog", and complete "Feed the cat", and then filter by "All", you should all the items

See the sample reports here:
* [Full Report](https://serenity-dojo.github.io/serenity-web-training)
* [Emailable Summary Report](https://serenity-dojo.github.io/serenity-web-training/serenity-summary.html)