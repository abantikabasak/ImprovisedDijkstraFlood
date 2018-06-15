# ImprovisedDijkstraFlood
This repository contains shape files of Bankura Road Network as well as the codes required for the working of the Improvised Dijkstra Algorithm. The format for inputs and what each file signifies is specified in the README file.

bnk_road.shp : Shape file for Bankura Road Network

GraphInput.py: 
Takes the nodes and edges as inputs from the shape file of Bankura Road network and from q_result.csv ,assigns indices to nodes,
stores them in 2 separate csv files bnk_node.csv for nodes and bnk_edge.csv for edges

LocateNodeIndex.py : 
Whenever you consider a point on the Bankura Road Network having x-coordinate x and y-coordinate y then the corresponding index 
will be displayed as output.

Input format:
x,y<ENTER>

FloodLevelShapeGenerations.py : Generates the Bankura Road Network which shall be modified after every flood level and generates bnk.road0,
bnk.road1,bnk.road2,bnk.road3,bnk.road4 which consist of shape files.

final_improvised_dijkstra.py : Final improvised dijkstra algorithm where you need to input the starting index and the destination index of the nodes
and the shortest but safest path is likely to change after each level of flood adversity. Those paths get stored as shape files as Path0 for flood level 0,
Path1 for flood level 1 and so on.

Finally all these Road Networks and Paths for different flood levels are visualised in the final.qgis file.


