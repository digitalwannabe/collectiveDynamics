<h1>Collective Dynamics</h1>

Real-time simulation tool\
Based on models discussed in the course
[Modelling Interacting Particle Systems in Science](http://ufind.univie.ac.at/en/course.html?lv=250031&semester=2021S)\
by Prof. Sara Merino Aceituno, University of Vienna, 2021\
\
Made using GPU compute shaders and [VL](https://visualprogramming.net/)
\
Draft version. At the moment Windows only.\
Requires a fairly powerful PC, in best case with dedicated GPU.

<h2>Implemented Models</h2>

<h3> Cucker-Smale Particle Model of Flocking </h3>
  
  As discussed in Carrillo, José A., et al. [Particle, Kinetic, and Hydrodynamic Models of Swarming](https://link.springer.com/chapter/10.1007/978-0-8176-4946-3_12)  
  Mathematical modeling of collective behavior in socio-economic and life sciences. Birkhäuser Boston, 2010. 297-336, Section 2.3.
  
* The model is fully implemented according to equations 2.3 in the paper.
* A noise term (Brownian Motion) has been added, calculated using a fast gpu pseudo random number generator 


<h3> Friction, Attraction, Repulsion </h3>
  
  As discussed in D’Orsogna, Maria R., et al. [Self-propelled particles with soft-core interactions: patterns, stability, and collapse.](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.96.104302)
  Physical review letters 96.10 (2006): 104302.
  
* TODO


<h3> Myxobacteria </h3>
  
  As discussed in Degond, Pierre, Angelika Manhart, and Hui Yu. [An age-structured continuum model for myxobacteria.](https://www.worldscientific.com/doi/abs/10.1142/S0218202518400043)
  Mathematical Models and Methods in Applied Sciences 28.09 (2018): 1737-1770.
  
* TODO


<h1>To use the tool</h1>


* Download zip below OR clone/download repo and navigate to *demo* folder 
* Unpack zip and run collectiveDynamics.exe
* To reset a slider click it using your mouse wheel
* In order to use custom initial positions and velocities:
  * Create a \*.csv file (e.g. using Excel or python) with 3 values (X,Y,Z) per row, separated by a comma (see /assets/initialPositions.csv as an example)
  * Load them using the specified field in the tool
  * Reset if necessary
* If you run into performance issues (below 30 fps) you can try to load less particles, see point above.


<h1>To run/edit/compile the code</h1>

* Download and install [VL](https://visualprogramming.net/) version 2021.4 or higher
* Run collectiveDynamics.vl
* To see/edit the compute shaders representing the models right click on *particleSystemPBR*, select open. In the newly opened window right click on *Simulation*, select open. Here you will see the shaders, right-click again to view them in a text editor.
* To compile click the button in the top left corner and hit *Export*



