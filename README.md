This simulation aims to produce realistic acceleration times given a car's data.
It simulates the force the engine puts through the tyres and pushes the car forward, the various drag forces from the body and tyres, and longitudinal load transfer and acceleration G force. Also, it takes into account the time cars need to shift gears. The scope was to find the optimal acceleration times, therefore a tyre model with slip ratio wasnt included, wheelspin isnt simulated, but instead a calculation of the maximum force the tyre can put on the road based on tyre characteristics and vertical load.
The results of the simulation for the cars used are very close to the ones that various websites report for the real cars.
Below are the version changelogs and some plots from the program.
# Version 5
- code generalized more to support various different cars, FWD and AWD now supported.

# Version 4
- fixed physics breaking when launching from high rpm
<img width="400" alt="image" src="https://github.com/vougioukakis/car-acceleration-simulation/assets/121321765/c39a6378-7f3a-4423-b412-a8c10a569e44">
<img width="393" alt="image" src="https://github.com/vougioukakis/car-acceleration-simulation/assets/121321765/1892968f-57a1-402f-ab45-ba7baa585707">
<img width="398" alt="image" src="https://github.com/vougioukakis/car-acceleration-simulation/assets/121321765/f270498b-066d-4c2b-85b5-2168fb272684">
<img width="394" alt="image" src="https://github.com/vougioukakis/car-acceleration-simulation/assets/121321765/2d1f69cf-e665-4280-bb3e-1b2fcd0e446e">

On the right are the simulation results compared to a real world measurement for the McLaren Speedtail
<img width="812" alt="image" src="https://github.com/vougioukakis/car-acceleration-simulation/assets/121321765/11f387fc-2377-4f70-9839-6010a1fc0fc3">


# Version 3
I skipped uploading v2
v2:
- simulating launch RPM
- simulating shift time and rpms dropping in between
- fixed physics breaking when launching from a standstill

v3:
- using the data of the mclaren f1 and mclaren speedtail
- launching is more realistic:
    - cant always use 100% of the traction when launching from a standstill because of random factors
    - longitudinal load transfer is now simulated, with much better 0-60 times (McLaren F1 from 4+ seconds to 3+)
- added aerodynamic drag of wheels
- downforce now plays a role in rolling resistance


# Version 1

<img width="480" alt="SCR-20240623-rfnl" src="https://github.com/vougioukakis/car-acceleration-simulation/assets/121321765/d10a68e8-de94-4ef5-87ff-679f645f2085">
<img width="483" alt="SCR-20240623-rflq" src="https://github.com/vougioukakis/car-acceleration-simulation/assets/121321765/b6bd815c-c0e9-4064-8c05-6fa38e4f0818">
<img width="467" alt="image" src="https://github.com/vougioukakis/car-acceleration-simulation/assets/121321765/880cc4d1-d199-4bc4-b3e5-55dfceacb4ed">
<img width="474" alt="image" src="https://github.com/vougioukakis/car-acceleration-simulation/assets/121321765/6285a530-2eff-471d-92df-80e65446351c">


