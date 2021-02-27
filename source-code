
import networkx as netx
import matplotlib.pyplot as plt

graph=netx.DiGraph()
graph.add_node(0)
graph.add_node(1)
graph.add_node(2)
graph.add_node(3)
graph.add_node(4)
graph.nodes[0]['pos']=(0,4)
graph.nodes[1]['pos']=(3,2.5)
graph.nodes[2]['pos']=(2,0)
graph.nodes[3]['pos']=(-2,0)
graph.nodes[4]['pos']=(-3,2.5)
graph.add_edge(0,1,weight=5)
graph.add_edge(0,2,weight=3)
graph.add_edge(0,4,weight=2)
graph.add_edge(1,2,weight=2)
graph.add_edge(1,3,weight=6)
graph.add_edge(2,1,weight=1)
graph.add_edge(2,3,weight=2)
graph.add_edge(4,1,weight=6)
graph.add_edge(4,2,weight=10)
graph.add_edge(4,3,weight=4)
node_pos=netx.get_node_attributes(graph,'pos')
arc_weight=netx.get_edge_attributes(graph,'weight')
netx.draw_networkx(graph, node_pos, node_size=450)
netx.draw_networkx_edges(graph, node_pos,edge_color= 'black')
netx.draw_networkx_edge_labels(graph, node_pos,label_pos=0.3, edge_labels=arc_weight)
plt.axis('off')
plt.show()

print("There is no way to nodes from 4. node.")
uzunluk1=0
uzunluk2=0
uzunluk3=0

dortten_bire = netx.dijkstra_path(graph,source=4,target=1)
print("\nShortest path(4,1):",end="")
print(dortten_bire)
temp=4
for integer in dortten_bire:
    if integer==4:
        continue
    else:
        uzunluk1+=arc_weight[(temp,integer)]
        temp=integer
print("Shortest path length(4,1):",uzunluk1)

dortten_ikiye=netx.dijkstra_path(graph,source=4,target=2)
print("\nShortest path(4,2):",end="")
print(dortten_ikiye)
temp=4
for integer in dortten_ikiye:
    if integer==4:
        continue
    else:
        uzunluk2+=arc_weight[(temp,integer)]
        temp=integer
print("Shortest path length(4,2):",uzunluk2)

dortten_uce=netx.dijkstra_path(graph,source=4,target=3)
print("\nShortest path(4,3):",end="")
print(dortten_uce)
temp=4
for integer in dortten_uce:
    if integer==4:
        continue
    else:
        uzunluk3+=arc_weight[(temp,integer)]
        temp=integer
print("Shortest path length(4,3):",uzunluk3)
print("##################################################")

graph.remove_node(3)
node_pos=netx.get_node_attributes(graph,'pos')
arc_weight=netx.get_edge_attributes(graph,'weight')
netx.draw_networkx(graph, node_pos, node_size=450)
netx.draw_networkx_edges(graph, node_pos,edge_color= 'black')
netx.draw_networkx_edge_labels(graph, node_pos,label_pos=0.3, edge_labels=arc_weight)
plt.axis('off')
plt.show()

print("There is no way to 0 from 4. node")
uzunluk1=0
uzunluk2=0
uzunluk3=0

dortten_bire=netx.dijkstra_path(graph,source=4,target=1)
print("\nShortest path(4,1):",end="")
print(dortten_bire)
temp=4
for integer in dortten_bire:
    if integer==4:
        continue
    else:
        uzunluk1+=arc_weight[(temp,integer)]
        temp=integer
print("Shortest path length(4,1):",uzunluk1)

dortten_ikiye=netx.dijkstra_path(graph,source=4,target=2)
print("\nShortest path(4,2):",end="")
print(dortten_ikiye)
temp=4
for integer in dortten_ikiye:
    if integer==4:
        continue
    else:
        uzunluk2+=arc_weight[(temp,integer)]
        temp=integer
print("Shortest path length(4,2):",uzunluk2)
input()










