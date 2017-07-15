## Extended kalman filter project for vehicle lidar & radar sensor fusion
This is a project for Udacity Self-Driving Car Nanodegree program. In this project, I implemented a unscented kalman filter to estimate the state of a moving object of interest with noisy lidar and radar measurements. All codes are written with C++ and tested on the Udacity simulator 

## Requirement 
- C++
- Udacity simulator : [here](https://github.com/udacity/self-driving-car-sim/releases)
- uWebSocketIO : [uWebSocketIO](https://github.com/uWebSockets/uWebSockets) for either Linux or Mac
- For window users : [Windows 10 Bash on Ubuntu](https://www.howtogeek.com/249966/how-to-install-and-use-the-linux-bash-shell-on-windows-10/) to install uWebSocketIO. 

## Other Important Dependencies
* cmake >= 3.5
  * All OSes: [click here for installation instructions](https://cmake.org/install/)
* make >= 4.1
  * Linux: make is installed by default on most Linux distros
  * Mac: [install Xcode command line tools to get make](https://developer.apple.com/xcode/features/)
  * Windows: [Click here for installation instructions](http://gnuwin32.sourceforge.net/packages/make.htm)
* gcc/g++ >= 5.4
  * Linux: gcc / g++ is installed by default on most Linux distros
  * Mac: same deal as make - [install Xcode command line tools](https://developer.apple.com/xcode/features/)
  * Windows: recommend using [MinGW](http://www.mingw.org/)

## Run the Project 
Once the install for uWebSocketIO is complete, the main program can be built and run by doing the following from the project top directory.

1. mkdir build
2. cd build
3. cmake ..
4. make
5. ./ExtendedKF

## About the Project 
I constructed the C++ software mostly based on the lecture. But, I tried to pick the best initial values(position, noise value and so on) to get best performance (low RMSE).The performance of my unscented kalman filter is evaluated by the RMSE(Root mean squared error) of position x,y and velocity vx,vy. I got 0.0689, 0.0811, 0.3319, 0.2284 for each , which is quite accurate number to the ground truth and better performance than Extended Kalman Filter! 
This is my result image:  
![Test image](https://github.com/KHKANG36/Unscenteded-Kalman-Filter-Project/blob/master/dataset1.png)


## Discussion/Issues 
Later, I will visualize my NIS performance (I already implemented it in source code) and find best performance by analyzing it. 
