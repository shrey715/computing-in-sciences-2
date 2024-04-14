# Prey - Predator Model

## Introduction

The prey-predator model is a mathematical model that describes the interaction between two species, one of which is the prey and the other the predator. The model is based on the Lotka-Volterra equations, which were developed independently by Alfred J. Lotka and Vito Volterra in the early 20th century.

The model is used to study the dynamics of populations in ecosystems and has applications in fields such as ecology, biology, and economics. It is a simple model that assumes that the populations of the prey and predator are the only factors that affect their growth rates.

University of New Mexico: [Link of the model](https://www.cs.unm.edu/~forrest/classes/cs365/lectures/Lotka-Volterra.pdf)

## The Model

- #### Basic Idea

Population change of a species depends on 3 primary factors:
- Birth rate
- Death rate
- Interaction with other species (Prey or predator)

Sexual reproduction is a non-linear process usually, while asexual reproduction is linear. 

- #### Expressions

It's expressed as coupled differential equations:

for the prey,

$$ \frac{dx}{dt} = \alpha x - \beta xy $$

where, $\alpha x$ is the ```birth rate- death rate``` and $\beta xy$ is the ```interaction``` with the other species.


for the predator,

$$ \frac{dy}{dt} = \gamma xy - \delta y $$

where, $\gamma xy$ is the ```interaction``` with the other species along with the ```birth rate```  of predator and $\delta y$ is the ```death rate```.

- #### Integration of equations of motion/evolution

The equations are integrated to find the population of the prey and predator at any given time. The solutions to the equations are periodic, with the populations of the prey and predator oscillating between high and low values.

## Steady States

The model has two steady states, which are points in the phase space where the populations of the prey and predator do not change over time. The first steady state is when both populations are zero, and the second steady state is when both populations are at a non-zero value.

Steay states are important because they represent the equilibrium points of the system, where the populations of the prey and predator are in balance.

These steady states can be found by setting the derivatives of the equations to zero and solving for the values of the populations that satisfy this condition.

Mathematically, the steady states are given by: 

$$ \frac{dx}{dt} = \frac{dy}{dt} = 0 $$

Solving for this, we get the steady states of the system as:

$$ x = 0, y = 0 $$

But this is the trivial solution, pretty much pointless to us.
The non-trivial solution is:

$$ x = \frac{\delta}{\gamma}, y = \frac{\alpha}{\beta} $$

## Velocity Field

The velocity field of the prey-predator model is a vector field that describes the direction and magnitude of the movement of the populations of the prey and predator in the phase space. The velocity field is determined by the equations of motion of the model and can be visualized as a set of arrows that point in the direction of the movement of the populations.

We notice that the velocity field is a closed loop, which means that the populations of the prey and predator oscillate between high and low values over time. The velocity field is an important tool for understanding the dynamics of the model and can be used to predict the behavior of the populations in the future.

The velocity field forms a vortex, which means that the populations of the prey and predator move in a circular motion in the phase space. This circular motion is a characteristic feature of the prey-predator model and is a result of the interactions between the two species.

This vortex is at the equilibrium points of the system, that is, the steady states where the populations of the prey and predator do not change over time. The vortex is a stable structure that keeps the populations of the prey and predator in balance and prevents them from growing indefinitely.

## Graphs

Graphs of the prey-predator model show the populations of the prey and predator as a function of time. The graphs are periodic, with the populations oscillating between high and low values over time. The graphs show the cyclic nature of the model and the interactions between the prey and predator.

We use complex numbers to represent the populations of the prey and predator in the phase space. The real part of the complex number represents the population of the prey, while the imaginary part represents the population of the predator. The complex number is a vector that points in the direction of the movement of the populations in the phase space.

