This simulation aims to produce realistic acceleration times given a car's data.
It simulates the force the engine puts through the tyres and pushes the car forward, the various drag forces from the body and tyres, and longitudinal load transfer and acceleration G force. Also, it takes into account the time cars need to shift gears. The scope was to find the optimal acceleration times, therefore a tyre model with slip ratio wasnt included, wheelspin isnt simulated, but instead a calculation of the maximum force the tyre can put on the road based on tyre characteristics and vertical load.
The results of the simulation for the cars used are very close to the ones that various websites report for the real cars.
Below are the version changelogs and some plots from the program.

v5:
- 5.1 : little rpm 'blip' from the clutch slip after every gear change, depending on the car's shift delay coefficient
- code generalized more to support various different cars, FWD and AWD now supported.

v4:
- fixed physics breaking when launching from high rpm
On the right are the simulation results compared to a real world measurement for the McLaren Speedtail
<img width="812" alt="image" src="https://github.com/vougioukakis/car-acceleration-simulation/assets/121321765/11f387fc-2377-4f70-9839-6010a1fc0fc3">


v2:
- simulating launch RPM
- simulating shift time and rpms dropping in between
- fixed physics breaking when launching from a standstill

v3:
- using the data of the mclaren f1 and mclaren speedtail
- launching is more realistic:
    - longitudinal load transfer is now simulated, with much better 0-60 times (McLaren F1 from 4+ seconds to 3+)
- added aerodynamic drag of wheels
- downforce now plays a role in rolling resistance

