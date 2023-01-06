There are 3 main parts of this game I coded. 
1. Pathfinding: A* algorithm that will help AI units move more efficently. 
2. Strategy: The rule base iteration system
3. PCG: Procedural map generation

The rule base system will gather information about the game state and add it to our knowledge base. 
Then if we find a unification in the knowledge base for a rule, we gather it to later arbitrate. The rule that make it arbitration are fired in the game state.

The PGC System uses kruskal algorithm to create a random MST and then creates a map with tiles that have the same connections. 
Some tiles have sets of which a random one is choosen. This can add cycles back into the MST if the players harvest the trees to create a path

To run the game use 

> C:\Users\chris\.jdks\openjdk-17.0.1\bin\java.exe "-javaagent:C:\Program Files\JetBrains\IntelliJ IDEA 2021.3.1\lib\idea_rt.jar=56689:C:\Program Files\JetBrains\IntelliJ IDEA 2021.3.1\bin" -Dfile.encoding=UTF-8 -classpath C:\Users\chris\IdeaProjects\DrexelCode\611_CS\Portfolio\S3-CS387\out\production\S3-CS387;C:\Users\chris\IdeaProjects\DrexelCode\611_CS\Portfolio\S3-CS387\libs\jargs.jar;C:\Users\chris\IdeaProjects\DrexelCode\611_CS\Portfolio\S3-CS387\libs\java-cup-11a-runtime.jar;C:\Users\chris\IdeaProjects\DrexelCode\611_CS\Portfolio\S3-CS387\libs\xercesImpl.jar;C:\Users\chris\IdeaProjects\DrexelCode\611_CS\Portfolio\S3-CS387\libs\jdom.jar s3.base.Main
