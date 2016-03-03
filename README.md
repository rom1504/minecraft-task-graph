# minecraft-task-graph
Define a graph of tasks for minecraft

## Objectives

The objective is to represent minecraft tasks.

* craft an item
* dig a block

## Requirements

Handle the complexity of minecraft.

* task requirements
* task production
* task genericity
* task cost

## Technical representation

[graph.json](graph.json) contains a first try at what such a graph could look like.

Defining a good representation can be done before writing the tasks, or after, when it's clearer how users can use the graph, or how it can be made easier to write the tasks.

## Strategy

This project is pretty difficult, so instead of trying to define everything from schema to data to tools head on, I think it makes sense to start at it from all the different levels, and eventually form something coherent.

Axes:

### Defining a graph format

How should the edge and vertexes be defined.

### Write the data

Is it easy to write the data manually ? Should it be automated ? Can be it linked to already existing [data](github.com/PrismarineJS/minecraft-data)

### Use the data

Start building applications that use the data, even if the data doesn't exist. That will require to build some basic example for the application to work.

For example create a recipe combiner application, and try to learn from this.

## Use cases

### Bots

Can be used to do minecraft bots like [rbot](https://github.com/rom1504/rbot)

### Player help

An interface where players could ask "How do I get a diamond sword, I only got a wooden pickaxe ?".
And the interface would display multiple paths to achieve that tasks, with cost estimates.

### Game understanding

What do players do on a minecraft server ? 

An interesting thing to do would be logging players action, and seeing if what they do look like some of the tasks in the task graph.
It might even be possible to predict what they will do next.

## Related work

### Discussions

* A github issue on the minecraft bot framework mineflayer [#275](https://github.com/PrismarineJS/mineflayer/issues/275) about combining tasks

### Smart bots

* [rbot](https://github.com/rom1504/rbot) a node.js bot with a domain specific language to define tasks
* [bat](https://github.com/Gjum/Bat) a python bot, with a curse interface with some smart commands
* [minebot](https://github.com/michaelzangl/minebot/wiki) a bot based on plugging itself on the vanilla client, which already handle some high level tasks
* lot of other bots : this list should be completed

### Research projects

* The AGI framework opencog is working on some high level minecraft bot : [Minecraft_Bot_Development_Roadmap](http://wiki.opencog.org/wikihome/index.php/Minecraft_Bot_Development_Roadmap) 

### Task graphs/networks

Lot of work has been done in task planning and it should be explored to
 see what can be done, see for example [Automated_planning_and_scheduling](https://en.wikipedia.org/wiki/Automated_planning_and_scheduling)

