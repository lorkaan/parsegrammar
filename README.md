# ParseGrammar

A library containing Directed Graph representing symbol to symbol translation with a Grammar class representing a start symbol and any terminal symbols.

The Directed Graph is useful for representing finite state machines in automation bots, with the Grammar class adds a Flow Network functionality wwith multiple possible sinks (terminal states) and regular expression matching acting as "weights"

## Examples

For examples of the ParseGrammar library used see:
- [Pexpect Parser](https://github.com/lorkaan/pexpectparser)
	- [Pypi](https://pypi.org/project/pexpectparser/)
- [VPN Bot](https://github.com/lorkkan/vpnBot)

Installation
============

For Pip:
```
pip install -u parsegrammar
```

If using PipEnv:
```
pipenv shell

pipenv install parsegrammar
```
Usage
=====
## Import:
```
import grammar as gram
```

## Creating Classes
```
pGraph = gram.Graph()

pGrammar = gram.Grammar(<start_symbol>, <end_symbol>, pGraph)
```

where `<start_symbol>` is a vertex within pGraph
where `<end_symbol>` is a vertex, or list/set of verticies, within pGraph

The `<start_symbol>` can not be an isolated vertex.

## Adding to the Graph
```
graph.addEdge(username, passPrompt, password)
```
