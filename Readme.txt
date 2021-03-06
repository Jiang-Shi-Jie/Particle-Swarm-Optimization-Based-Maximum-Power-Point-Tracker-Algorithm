Problem Statement:

Photovoltaic cell characteristic is non-linear whose output power varies as function of the irradiance and temperature. The reason for the non-linear is because, the value of irradiance and temperature changes throughout the day, thus decreasing the output efficiency. Also, the efficiency of these Photovoltaic modules is not satisfied by the power requirement. Hence, an algorithm to increase the efficiency of the PV module needs to be designed to solve the discrepancies among the efficiency of the cell and the power requirement. 
			Hence, the objective of this project is to design and model the Particle Swarm Optimization assisted MPPT algorithm and enhance the efficiency of the photovoltaic system.


Motivation:

At present, most of the street lights are powered through conventional energy sources. But, there is a huge disparity between the growing demand and available resources. Hence demand for renewable energy that is, Solar power based street lights are increased. 
The Solar powered devices are best suitable in places where there is scarcity of renewable resources. The initial cost of these solar powered devices is more. Therefore, the integration of a robust MPPT controller is necessary. Maximum power point tracking (MPPT) consists of extracting the maximum power from the PV generator. With MPPT more devices can be powered with less wattage panel. 

        
Particle Swarm Optimization Based MPPT Algorithm
Step 1 (Parameter Selection): In the proposed system, the particle position is defined as the duty cycle value d of the dc–dc converter, and the fitness value evaluation function is chosen as the generated power P. From the algorithm point of view, a larger number of particles result in more accurate MPP tracking even under complicated shading patterns. However, a larger number of particles also lead to longer computation time. Therefore, a trade-off should be made to ensure good tracking speed and accuracy.

Step 2 (PSO Initialization): In PSO initialization phase, particles can be placed on fixed position or be placed in the space, randomly. Basically, if there is information available regarding the location of the Global_MPP in the search space, it makes more sense to initialize the particles around it. The particles are initialized on fixed positions which cover the search space [Dmin, Dmax] with equal distances in this paper. Dmax and Dmin are the maximum and minimum duty cycle of the utilized dc-dc converter, respectively. 

Step 3 (Fitness Evaluation): The goal of the proposed MPPT algorithm is to maximize the generated power PPV. After the digital controller output, the PWM command according to the position of particle i (which represents the duty cycle command), VPV and current IPV can be measured and these values can then be utilized to calculate the fitness value PPV of particle i. It should be noted that in order to acquire correct samples, the time interval between successive particle evaluations has to be greater than the power converter’s settling time.

Step 4 (Update Individual and Global Best Data): If the fitness value of particle i is better than the best fitness value in history p_(best,i), set current value as the new p_(best,i). Then, choose the particle with the best fitness value of all the particles as the g_best. This step is similar to step 3 of the standard PSO method.

Step 5 (Update Velocity and Position of Each Particle): After all the particles are evaluated, the velocity and position of each particle in the swarm should be updated.

Step 6 (Convergence Determination): Two convergence criteria are utilized in this paper. If the velocities of all particles become smaller than a threshold, or if the maximum number of iterations is reached, the proposed MPPT algorithm will stop and output the obtained g_best solution.                 

Step 7 (Reinitialization): Typically, PSO method is used to solve problems that the optimal solution is time invariant. However, in this application, the fitness value (global maximum available power) often changes with environments as well as loading conditions. In such cases, the particles must be reinitialized to search for the new GMPP again. The following constraint is utilized to detect the insolation change and shading pattern changes.


CONCLUSION
The scope of this project was to increase efficiency of PV module. Photovoltaic cell characteristic is non-linear whose output power varies as irradiance and temperature varies.A DC-DC Boost converter which steps up the voltage from the output of solar panel which is 16-21v to a voltage required to power the device. Then a DC-DC Boost convertor is Designed to increase the output voltage, suitable inductor and capacitance values were found. A DC-DC Boost converter modelling is done to check stability of the circuit.  

The efficiency of the PV module is increased by using a particle swarm optimization(PSO) assisted MPPT algorithm. Particle Swarm Optimization technique is implemented and increase in output power is demonstrated . This method is tested for varying atmospheric conditions. PSO method was found to track MPP faster and accurately even under partially shaded and varying atmospheric conditions. 


