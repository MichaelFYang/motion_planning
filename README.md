## Motion Planning Library with ROS

Self-directed independent study.

Completed:

* The `map` package: `roslaunch map viz_map.launch`
	- Probabilistic Roadmap:

	<img src="map/media/prm.png" alt="PRM" width="300"/>

	- Tunable-resolution Grid Map

	<img src="map/media/grid.png" alt="GRID" width="300"/>

In progress:

* The `global_planner` package:
	- A* (green) on PRM:

	<img src="global_planner/media/astar.png" alt="ASTAR" width="300"/>

	- Theta* (green) on PRM (A* in red for comparison): `roslaunch global_planner astar.launch`

	<img src="global_planner/media/thetastar.png" alt="ASTAR" width="300"/>

	- A* (green) on Grid

	<img src="global_planner/media/lpastar.png" alt="ASTARG" width="300"/>

	- LPA* with Simulated Grid Updates [re-evaluated cells in orange]: `roslaunch global_planner incremental.launch lpa:=True`
	<img src="global_planner/media/LPAstar.gif" alt="LPASTAR" width="300"/>

	- D* Lite V2 on Grid [re-evaluated cells in orange]: `roslaunch global_planner incremental.launch`
	<img src="global_planner/media/DstarLite.gif" alt="DSL" width="300"/>

	- Potential Field with local minimum escape on Grid
* Local planner:
	- Dynamic Window Approach
* Trajectory Optimization:
	- Model Predictive Path Integral Control

