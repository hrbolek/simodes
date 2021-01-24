# ReadMe

## Main Idea
Having a package wich allows run ODE simulations along with DES simulations.
Having an environment where all informations are stored in single place.

## Dependency 
This package uses scipy for ODE integration. 

## Solution
This package convers ODE model with solver into generator. Generator outputs are planed to come live by event calendar.
Such a conversion from ODE into DES make all magic.

For simulation management the Redux idea is utilized. All simulation tasks are converted into actions dispatched over storage.
Storage itself has three pilars:

- ODE models state (time, state and state derivation)
- Event calendar (list of events and related functions plus active event)
- Log manager (kind of heterogenous database)

## Examples
Examples are available in notebooks directory, where Jupyter notebooks are stored. All of them are prepared for running in Google Colab.
