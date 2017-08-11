# decision-tree-builder [![NPM version][npm-image]][npm-url] [![NPM Downloads][npm-downloads-image]][npm-url]

A tool to build data classification rules using visual flowchart-style decision tree.
Uses [d3.js v4](https://d3js.org/) for SVG drawing.

## terminology
* **Property:** a (data) attribute being evaluated as part a decision (e.g. Property: "animal")
* **Value:** a value being used in a conditional statement to evaluate a property 
(e.g. does Property "animal" equal the Value "cat")
* **Operator:** the logical operator used to evaluate a properties value (e.g. "equals", "less than" etc.) 
* **Decision:** a conditional operation determining which of two paths the program will take
* **Result Node:** aka a leaf node, represents the final result when an input is evaluated by the decision tree

## notes
* we do not provide any validation of decision tree logic, it's up to you!
	* for example; you could make a change to a parent node which renders its children completely redundant, 
	and it will still be valid.  

## todo
* start drafting API..
	* Interaction flow, somewhere to start:
	    * User click node to add/edit
	        * selectNode()
            * if children returns data for that node..
            * else object scaffold with empty values..?
	    * We need to define a schema for defining properties, operators, and values. Then: 
	    * Select a property
	    * Select an operator
	    * Select a value
	    * Cancel / Add / Update
	    	   
	  
	    	  	   
[npm-image]: https://badge.fury.io/js/decision-tree-builder.svg
[npm-url]: https://www.npmjs.com/package/decision-tree-builder
[npm-downloads-image]: https://img.shields.io/npm/dt/decision-tree-builder.svg	   