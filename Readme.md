# INTRODUCTION

---

* This repository contains Python codes for the Football Pi-Car Controller. 
* The codes are implemented in Python3.9.
* The codes were run on Raspberry with the dependency of **OpenCV**, which can install with pip command as

```
pip install opencv-python
```

# START

---

* Ensure the fields (ball, goal, goal markers) are deployed completely. In our experiments, we used tennis balls and blue goal markers.

* *Note: The different targets will affect the algorithm's performance. If other targets are used, the HSV value of new targets must be re-calibrated and initialized in the* Class `FootballCar()` of `./Football_Robot.py`.

* Ensure the codes are located in the folder. /Picar-4wd/` and the two servos are mounted on PWM 1, and 2 of the striker.

* Ensure two Pi-Cars are connected to the computer and run the following commands separately.

  ```
  python start_goalkeeper.py
  python start_striker.py
  ```

  The striker and goalkeeper will now loop several times (the number of loops can be controlled in the `start_<player>.py` file).


