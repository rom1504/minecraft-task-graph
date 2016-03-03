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

## Technical representation

[graph.json](graph.json) contains a first try at what such a graph could look like.

Defining a good representation can be done before writing the tasks, or after, when it's clearer how users can use the graph, or how it can be easier to write the tasks.