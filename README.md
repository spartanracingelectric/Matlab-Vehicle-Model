The file and github branch organization is as following.
File Organization
Required Files:
  sim-runner.m   // This will be in charge of sim UI and running the selected sim. Must be capable of running with any number of working selected .m files

Additional Files:
  (Examples)     // The system is designed to be modular. There should be no dependent files, all should be optional.
  battery.m
  chassis.m
  motor.m
  tire.m
  driver-inputs.m
  motor-controller.m

Github Branch Organization
main      // The main/master branch. Periodic Backups should be made of working models, in order to denote major changes to sim proficiency. All merges into this branch must be PR approved.

(All Additional Branches)   // These represent the offical versions of each individual module of the simulation. 
                            // These are made to represent the founding point of all work done to one particular file. 
                            // All merges to these branches must be approved via PR. 
                            // There should be an equal number of protected branches as .m files

Example of Workflow:

  Existing Files:

    sim-runner.m
    battery.m
    chassis.m
    motor.m
    tire.m
    driver-inputs.m
    motor-controller.m

  Github Branches:
  
    sim-runner
    battery
    chassis
    motor
    tire
    driver-inputs
    motor-controller
