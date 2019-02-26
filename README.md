# FEM_BAR_ELEMENT
Program will calculate Displacement, Stress and Strain of BAR Element.


STRUCTURAL BAR: A structural memeber is called BAR when it is loaded axially.
There are 3 methods to solve any physical problem.
  1. Analytical Method: Uses hypothesis, theory, mathematics and calculus to solve the engineering problem. use of complex mathematics and                         calculus.Usually very difficult to form theory and solve it.
  2. Experimental Method: Use of prototype or designing an experiment and obtaining results tao match or solve real world problem.
                          Expensive.
  3. Finite Element Method: or Finite Element Analysis is a numerical method to solve the engineering problem. Uses technique called                                   discretization or finitization of continuous body into finite number of elements. 
  
  Let's understand it by taking a example and using all above 3 stated methods to solve it.
  
  Method 1: Analytical method.
  
  Problem Definition: Calculate the stress induced in a bar whose diameter is 25mm and it  is subjected to a force of 100 KN.

So Normally from the Strength of material equation we can calculate stress as 
                                  Sigma=FA
Where F is the force acting and A is the cross sectional area of the bar. So
 
                                 Sigma =100 KN/490.8738

                                 Sigma= 203.718 MPa

If we assume material is steel with Young’s modulus 210 GPa then we can calculate strain in the material as 
                                  Stress/Strain = E
                              Strain is given by Strain = Stress/E
                                                 Strain = 203.718/2x10^5
                                                 Strain = 0.000101859
                                 Elongation is obtained by =dL/L
                                          dL= x L
                                          dL= 0.000101859x 3.5
                                          dL = 0.0003565065 m
                                          
2. Experimental Method: If we want to solve the this engineering problem by Experimental method. We actully have to find a bar and fix it at one 
                        end and apply a 100KN of force and to measure the displacements we have touse strain gauges. As told earlier this method 
                        is expensive and requires lot of planning of experiment.
                        
3. Numerical Method or FEM or FEA: In FEM every continuous body is discretized into elements or it is finalized. So let's see how it is done.

The basic equation of FEM is K * u = F
Where K is stiffness, u is displacement and F is Force

Since Numerical methods are used in FEM to solve the problems and Numerical Methods use Matrices we express or write FEM equation as 
{K} . {u} = {F}
Where {K} is stiffness Matrix, {u} is displacement Matrix and {F} is Force Matrix.

1st of all stifness matrix is formed. 
2nd displacement is calculated by multiplying inverse of stiffness mtrix and force matrix.
3rd stress and strain are calculated using standard formulas.


                                  
