
This is the repository for the [Verifibaility Node](https://verifiability.org). 
Here, we have made available a number of public repositories where we publish artefacts for our projects.

We also link to repository tools developed and used by members of the Node.

The image below displays an overview of our Node.

![Screenshot 2023-06-23 at 12 31 04](https://github.com/VerifiabilityNode/.github/assets/35529523/83e238f0-1890-4fe5-a79a-0f60dedfad55)

Starting from case studies and experiments, we design the specification of our systems that are converted into a range of intermiddeiate models fed to multiple verification paradigms (such as formal verification, mutation testing, convformance verification and runtime monitoring), which, in turn provide evidence of verification for the system under test. A more detailed workflows of the models can be seen below. We show how we cover the heterogenous nature of autonomous systems and provide multiple avenues for checking system properties, leading to a holistic judgement about the system. 

![Screenshot 2023-06-23 at 12 33 10](https://github.com/VerifiabilityNode/.github/assets/35529523/0679e825-4643-4d79-81bd-0f17002318c5)


Starting from the system requirements and system properties (which are artefacts typically written in natural language), a formal design model (using the Robo* framework) can be built based on the specified design. The system controller (RoboChart) is built based on the requirement specifications, assurance cases, and human agent models  (Circus). From this point, formal verification techniques (such as proofs in Isabelle/UTP and  model checking in FDR and nuXMV) are being used to offer mathematical assurances about the system.  Furthermore, discrete unit testing and hybrid system testing mechanisms are being developed for RoboChart models. 


In order to capture the physical aspects inherent to robotics, the RoboChart controller is extended to take into consideration the kinematics and dynamics of the system under test, of the other agents, and also the environment; the combination of the (discrete) controller behaviour and the (continuous) physical aspects are captured in RoboSim models. Such models can be used to automatically generate SDF models, which, in conjunction with simulation code, are fed to popular robot simulators/middleware (e.g., CoppeliaSim and ROS). Simulation takes a vital role in the testing of robots due to practicality. With simulation, one can verify the continuous aspects of the system’s correctness and apply corrections before the physical system is used. For instance, in this Node, we consider system-wide conformance/mutation testing (using Matlab/Simulink), runtime monitoring (ROS Monitoring), and adversarial attacks checks. In summary, we offer evidence of verification based on multiple verification paradigms; in turn, the obtained evidence is directly applied into the development of the physical system.


A more detailed workflow of the models used across the Node can be found below.
