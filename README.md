# Autonomous Mobile Robots

## 1. Prerequisites

You can find a shell script that will install all dependencies [here].

### 1.1 ROS Kinetic

Install ROS via the script or following the installation instructions for [ROS].

### 1.2 Catkin workspace

Make sure you initialized your catkin workspace:

```
mkdir catkin_ws
cd catkin_ws
mkdir src
cd src
catkin_init_workspace
cd ..
catkin_make
```
### 1.3 Bugfix for Stage and KDL

For the amr packages to work you will need to apply the bugfix provided [here].

[ROS]: https://wiki.ros.org/kinetic/Installation/Ubuntu
[here]: https://github.com/HBRS-AMR/AMR-Wiki/tree/master/ROS-Installation

## 2. Using the amr packages

Clone your repository into the src folder of your catkin workspace.

Then go to the root folder of your catkin workspace and execute ```catkin_make``` in a terminal. Don't forget to source your workspace.

## 3. Git workflow

If you are unsure about how to use git please look at the
[Git workflow](https://github.com/HBRS-AMR/AMR-Wiki/blob/master/git.md).

## 4. Assignments

When solving assignments please use the following guidelines:

* Look at the [submission details](https://github.com/HBRS-AMR/AMR-Wiki/blob/master/Submission_Details.md)
* Write readable code, this includes proper names for variables (e.g. wheel_speed_left instead of wsl) and functions (e.g. getDistanceToObstacle() instead of distance())
* Follow the Python naming conventions ([Google Python Style Guide], [Python Style Guide])
* Use short and descriptive commit messages (not like [this])
* Commit frequently, don't commit the whole assignment in one go
* Use a [git branching model], don't work on your master branch directly
* Make sure to merge all your changes into the master branch before the deadline. Grading is based on your master branch at the time of the deadline. No late submissions.
* Repositories are private to prevent plagiarism, if two people have the same code they'll both receive 0 points for the assignment


[Google Python Style Guide]: https://google.github.io/styleguide/pyguide.html
[this]: https://xkcd.com/1296/
[Python Style Guide]: https://www.python.org/dev/peps/pep-0008/
[git branching model]: https://nvie.com/posts/a-successful-git-branching-model/
