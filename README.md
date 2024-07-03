# LittleSLAM

## LittleSLAMabout

LittleSlam is a SLAM learning program.
Enter the 2D laser scanner data (scanning) and a file that stores the odometri data, and
Output the trajectory of the robot position and the 2D point group map on GNUPLOT.

LittleSlam is based on scanning matching, fusion of laser scanners and odometri,
It consists of elemental technology such as the loop closure based on Graph-Based Slam.

LittleSlam is a program created as a teaching material for reference books [1].
We adopt simple algorithms giving priority to easy -to -understand.
Therefore, the performance drops compared to the full -spec SLAM program,
It is easier to understand the contents.


## Execution environment

LittleSlam is described in programming language C ++.
The execution environment that confirmed the operation is as follows.Both are 64 -bit versions.

| OS | C++ |
|:--:|:---:|
| Windows 7 | Visual C++ 2013 (Visual Studio Community 2013)|
| Windows 10 | Visual C++ 2015 (Visual Studio Community 2015)|
| Linux Ubuntu 14.04 LTS | gcc 4.8.4|
| Linux Ubuntu 16.04 LTS | gcc 5.4.0|

The operation on the 32 -bit OS has not been confirmed, so if you need it, please try it yourself.


## Required software

The following software is required to execute LittleSlam.

| software | content | version |
|:------------:|:----:|:----------:|
| Boost        | C++General -purpose library |1.58.0 |
| Eigen3       | Linear algebraic library|3.2.4 |
| gnuplot      | Graph drawing tool  |5.0 |
| CMake        | Build support tool |3.2.2 |
| p2o          | Graph-based SLAMSorba|beta |

The version was used in the development of LittleSlam, not a clear condition.
If it is more than this, it usually works.
There is a possibility that it will operate even in the following versions.

## How to use

- Windows[Click here](doc/install-win.md)

- Linux[Click here](doc/install-linux.md)

## data set

Six data files are available for experiments.The list is shown in the table below.
[here](https://furo.org/software/little_slam/dataset.zip)You can download it.


| file name      | content        |
|:--------------------|:-------------|
| corridor.lsc        | Corridor (single loop) |
| hall.lsc            | Somework (single loop) |
| corridor-degene.lsc | Corridor (degeneration) |
| hall-degene.lsc     | Somework (degeneration) |
| corridor-loops.lsc  | Corridor (multiple loop) |
| hall-loops.lsc      | Somework (multiple loop) |

## Customization

LittleSlam is a learning program, and some improvements from the basic form
You can customize it to complete.  
See Click here for more information.

## Reference book

The following books are SLAM's commentary.In addition to giving general explanations of SLAM
As a specific example, LittleSlam is used as a teaching material and the details of the source code are explained.

[1] Masahiro Tomo, "Introduction to SLAM -Technology of Robot's Self -Position Estimation and Machine Construction Technology", 2018

## license

- LittleSlam is based on the MPL-2.0 license.

