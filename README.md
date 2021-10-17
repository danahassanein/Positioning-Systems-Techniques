# Positioning-Systems-Techniques
### Implementing indoor positioning systems tequniques such as N-Lateration, Static-Fingerprint, and Mobility Prediction with HMM.

## N-Lateration:
The objective is to conceive and implement, with the language of your choice, the basic N-lateration algorithm. In this directed work, I will propose a global architecture view of an indoor positioning scenario involving N=4 Access Points and an object/human identified as a Mobile Object (Terminal). 2 approaches based, either on model propagation, or Time of Fligth, provide distances between Emitters and Receivers.

The work to do is :

1. Design the V1 version of the implementation (following scrum/agile methodology), which
favorize the time to validation of positioning technic implementation ;

2. Propose the Object Class Diagram with prioritized functions ;

3. Conceive the two main algorithms :

     - The N-lateration algorithm which compute the estimated position by minimizing the
sum of distances to 4-spheres inside the perimeter of the 4 spheric volumes
agregated ;

     - The factory design pattern (for the given data set) ;

4. Compare the result provided by your implementation with a geometric resolution of the
senario provided.

## Static-Fingerprint:
Consist in building a matrix of an environment. Each case of the environment is characterize with
informations :

   - Geographic information, for examples :
     - Lattitude, longitude, altitude (universal or global reference
system of positioning);
     - The postal address, the stage, the room ;
     - The relative positioning in a 2D plan or 3D plan (local reference system of positioning) ;
   - Geographic information, for examples :

     - Lattitude, longitude, altitude (universal or global reference
system of positioning);
     - The postal address, the stage, the room ;
     - The relative positioning in a 2D plan or 3D plan (local reference system of positioning) ;
   - Descriptive information :
     - Signal : Received Signal Strength, Emitted Signal (power) Strength, wave orientation, ratio RSS/ESS => wave propagation model (Friis, …)
     - Quality of communication : received messages over emitted, packet losts, number of damaged messages, …
   - But also
     - Needs to catch the actual environment photography of either the MT
(Terminal-centric PS) or each component of the infrastruture-centric PS
     - Then determine by matching the k best fingerprint closest to the catched environment (above) and determine by weighted barycenter computing the positioning of the Object or Human

## Markov Model usefull for anonymisation and for prediction:

What is Markov Model or Hidden Markov Model ?

An interesting computer science object interesting to :
  - modelize an automata,
  - a statistical and valued graph
which allow, firstly to summarize actions performed, and secondly to predict the next position or
action.
MM is composed of nodes and transitions
