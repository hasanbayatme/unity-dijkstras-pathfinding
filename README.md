# Unity Dijkstra's Pathfinding

Dijkstra's Pathfinding Algorithm Unity Implementation.

It is the implementation of [Dijkstra's Pathfinding Algorithm](https://en.wikipedia.org/wiki/Dijkstra%27s_algorithm) in [Unity (Game Engine)](https://unity3d.com) that let's you find the shortest path between two Nodes in a Graph.

![Dijkstra_Animation](https://upload.wikimedia.org/wikipedia/commons/5/57/Dijkstra_Animation.gif)

In this example we are going to find the shortest path from **Node A** to **Node F**:

![Sample 1](https://i.imgur.com/WHQn8lf.gif)

In this example we will try to follow the path using a simple Cube object:

![Sample 2](https://i.imgur.com/dcDpawc.gif)

## Getting Started

- [Download](#download) the project
- Open in Unity
- Go to Demo scene
- [See Usage](#usage)

## Download

Follow one of the below ways to download the project:

- Clone (Run the below command in Terminal or Command Prompt)

```bash
git clone https://github.com/EmpireWorld/unity-dijkstras-pathfinding.git
```

- [Download ZIP](https://github.com/EmpireWorld/unity-dijkstras-pathfinding/archive/master.zip)
- [Download Latest Version](https://github.com/EmpireWorld/unity-dijkstras-pathfinding/releases/latest)

## Usage

### Editor Usage

Click on **Graph** object to use the Editor Integration.

### Runtime Usage

You can use the Graph **GetShortestPath** method to get the shortest path and follow it:

```csharp
Path path = myGraph.GetShortestPath ( start, end );
for ( int i = 0; i < path.nodes.Count; i++ ) {
  Debug.Log ( path.nodes [i] );
}
Debug.LogFormat ( "Path Length: {0}", path.length );
```

Check the [Follower Script](https://github.com/EmpireWorld/unity-dijkstras-pathfinding/blob/master/Assets/Scripts/Follower.cs) for usage example.

## Resources

[:speech_balloon: Forum Thread](https://forum.unity.com/threads/unity-dijkstras-pathfinding.505212/)

## License

MIT @ [Hasan Bayat](https://github.com/EmpireWorld)

Made with :heart: by [Hasan Bayat](https://github.com/EmpireWorld)
