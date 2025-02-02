---
layout: default
title: Optimize Applications
nav_order: 5
---

# Optimize your Python application
{: .no_toc }
In this procedure, you will learn how to optimize your python application. To improve the performance, programmers usually use profilers to find the code that takes too much time during execution. By the end of this procedure, you will be able to understand the optimization report generated by PyCharm.

## Pre-requisites
Before optimization, make sure you have met the following requirements:
* You have installed Python from [https://www.python.org](https://www.python.org).
* You have opened an existing project or created a new project.

## Instructions
1. The following is a piece of code for demonstration, and you will optimize it using PyCharm.

    ![Sample Code](../../assets/images/docs/profile/code.png "Sample Code")

2. To generate a optimization report, click the ![Profile](../../assets/images/docs/profile/icon.png "Profile") icon on the main toolbar.

    ![Toolbar](../../assets/images/docs/profile/toolbar.png "Toolbar")

3. Pycharm will then execute your code and generate a report as bellow. In the report, you can see how much time each function has taken during the execution.

    ![Report](../../assets/images/docs/profile/report.png "Report")

4. Now you know that the ```built-in``` method has taken the most time. Right click on that row, and choose ```Show on Call Graph``` in the popup menu.

    ![Menu Graph](../../assets/images/docs/profile/menu_graph.png "Menu Graph")

5. Pycharm will show you a call graph, and you can see the function ```bar``` in your code has called the ```built-in``` method.

    ![Call Graph](../../assets/images/docs/profile/call_graph.png "Call Graph")

6. Right click in the orange rectangle and choose ```Navigate to Source``` in the popup menu, and Pycharm will bring you to the function to be optimized.

    ![Navigate](../../assets/images/docs/profile/menu_nav.png "Navigate")

---
Congratulations! You have learnt how to optimize your Python application using Pycharm. If you have any issues, check out [Troubleshooting]({{ site.baseurl }}{% link docs/trouble.md %}).
