# GROUP 03
* Nathan Mbock, nathanjeanemmanueljolly.mbock@studenti.unipd.it
* Damien Brocheton, damien.brocheton@studenti.unipd.it
* Louis Plantey, louis.plantey@studenti.unipd.it

# IR2425 Group 03 Assignment 2


## Build Instructions

To set up and build the project, follow these steps:

1. **Clone the repository**:  
   Clone the repository into the `src` folder of your Catkin workspace:
   ```bash
   cd ~/catkin_ws/src
   git clone https://nathan_mbock-admin@bitbucket.org/nathan_mbock/ir2425_group_03.git
   ```

2. **Build the project**:  
   From the root of your Catkin workspace, run:
   ```bash
   cd ~/catkin_ws
   catkin build
   ```

## Launch Instructions

To launch the project, you need to manually start each node. The nodes are located in:  
`.../catkin_ws/src/ir2425_group_03/src`

### Launching Nodes
For each node file, open a terminal and execute the following commands:

1. Source the setup file:
   ```bash
   source ~/catkin_ws/devel/setup.bash
   ```
2. Lanch the simulation:
   ```bash
   ~/catkin_ws/src/ir2425_group_03/assignment2/exec.sh
   ```

3. Lanch node_a to get the line coefficent:
   ```bash
   rosrun assignment2 node_a.py
   ```

4. Lanch node_b to scan the aprilTags:
   ```bash
   rosrun assignment2 node_b_main.py
   rosrun assignment2 node_b_camera.py
   rosrun assignment2 node_b_nodesDetection.py
   ```
5. Lanch node_c to get move the robot to scan the room and move the objects:
   ```bash
   rosrun assignment2 node_c.py
   ```
