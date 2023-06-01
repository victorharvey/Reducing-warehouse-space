## Reducing Warehouse Space with the Pareto Principle 📦
*Let us say you have 4,864 unique SKUs and have 144,339 order lines with 59,372 unique orders. How do you prioritise warehouse operations?*

Let us say you have 4,864 unique SKUs and have 144,339 order lines with 59,372 unique orders. How do you prioritize warehouse operations?

The solution comes from understanding the cost breakdown of a warehouse:
> Fixed Cost - Rent, Amortisation
> Variable Cost - Picking Operators

Generally speaking, warehouses try to:
> Optimize space 
> Optimize racking location 
> Increase labor productivity 

To achieve this some companies focus on the picking process which is normally broken down as follows:
> Warehouse management system creates a work order
> A system guides an operator around the warehouse from location to location
> Operators stops at each location picking products until the work order is filled and ready for packing

Generally speaking, the walking from location to location in the warehouse can account for up to 70% of an operator’s time in a work order.

The solution is in improving operator productivity by reducing the picking distance between each location.

This is done by:
> increasing the picking location density
> Placing all SKU with large number of orders (high rotation) in the same area 

Of Course a warehouse is packed on a 3 dimensional plane.

So, as the operator moves in 2 dimensions (left/right, forward/backwards) to pick items for packing the third dimension (up/down) is used for storage.

The picking location at the operator level is restocked from the higher level during replenishment waves.

The replenishment process itself is a delicate balance between:
> Productivity
> SKU Density

Strategies could be:
> Full Pallet Replenishment - High in Productivity / Low in SKU density
> Half Pallet Replenishment - Medium in Productivity / medium SKU density
> Shelves Replenishment  - Low in Productivity / High in productivity 

The Pareto principle (80/20 rule) is a good principle to follow to optimize the space, location and operator productivity.

What percentage of the active reference (item,brand) makes 80% of the volume.

Using data from Kaggel I explore how to apply this Pareto Principle to optimize the layout of a Warehouse:
- 1 month of picking orders
- 144,339 order lines
- 59,372 orders
- 4,864 active references

Code can be found in the comments below. 

Using the data I have generated a chart:
> Y Axis - Percentage of Boxes Ordered (%)
> X Axis - Percentage of SKU (%)

We can see that:
High rotation SKU: Make up ~20% of SKUs but are over ~80% of Boxes ordered (Purple Line) 
Low rotation SKU: Make up ~80% of SKUs but are only ~20% of outbound volume. (Purple Line)

Actions to take:
High rotation SKUs should equal to High Replenishment policy
Low rotation SKUs should equal  to a Low Replenishment Policy

What this means is that 20% of the SKUs (high runners) should be located in Full and Half Pallet locations. 

While 80% of the SKUs (low runners) should be in Shelves.
Question becomes, does this principle operate the same way once you automate the warehouse?


## About me 🤓
Supply Chain Professional with international experience and a passion for data science. 
Connect with me on LinkedIn: Profile [Profile](https://www.linkedin.com/in/victorkharvey/) \
