# kinematic
# Inverse Kinematics:
## To calculate the kinematic inverse of a robot arm with 3 degrees of freedom, we use the following equations:

`1. x = l1 * cos(θ1) + l2 * cos(θ1 + θ2)`

`2. y = l1 * sin(θ1) + l2 * sin(θ1 + θ2)`

`3. z = l3 * cos(θ3)`

## where:
`- x, y, z: coordinates of the end of the robotic arm`

`- L1, L2, L3: link lengths (arm parts)`

`- θ1, θ2, θ3: bond angles1`

#### To obtain the values ​​of angles θ1, θ2, θ3 from the values ​​of x, y, z, the equations can be used:

`θ1 = atan2(y, x)`

`θ2 = acos((x^2 + y^2 - l1^2 - l2^2) / (2 * l1 * l2))`

`θ3 = atan2(z, sqrt(x^2 + y^2))`

#### These equations enable us to calculate the angles needed to place the end of the arm in a specific position (x, y, z).

# Forward Kinematics:
## As for the motor front, we use the following equations:

`x = l1 * cos(θ1) + l2 * cos(θ1 + θ2)`

`y = l1 * sin(θ1) + l2 * sin(θ1 + θ2)`

`z = l3 * cos(θ3)`

## where:
`- x, y, z: coordinates of the end of the robotic arm`

`- L1, L2, L3: link lengths (arm parts)`

`- θ1, θ2, θ3: bond angles`

#### These equations enable us to calculate the coordinates of the end of the arm (x, y, z) from the values ​​of the joint angles (θ1, θ2, θ3).

## Explanation in detail:
### 1. The motor inverse aims to find the values ​​of the joint angles necessary to place the end of the arm in a specific position (x, y, z). This is done using mathematical equations that link coordinates and angles.
### 2. Anterior motor aims to calculate the coordinates of the end of the arm (x, y, z) from the values ​​of the joint angles (θ1, θ2, θ3). This is done using the same mathematical equations, but in reverse order.
### 3. These equations are essential in the design and control of multi-degree motion robot arms.
