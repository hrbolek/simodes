# ReadMe

## Main Idea

1. Having a package which allows run ODE simulations along with DES simulations.
2. Having an environment where all informations are stored in a single place.

## Dependency 
This package uses SciPy for ODE integration. 

## Solution
This package converts ODE model with solver into generator. Generator outputs are planed to come live by event calendar.
Such a conversion from ODE into DES has made all magic.

The Redux idea is utilized for the management of simulation. All tasks in the simulation are converted into actions and then dispatched over the storage.
Storage itself has three pilars:

- ODE models state (time, state and state derivation)
- Event calendar (list of events and related functions plus active event)
- Log manager (kind of heterogenous database)

## Examples
Examples are available in notebooks directory, where Jupyter notebooks are stored. All of them are prepared for running in Google Colab.
