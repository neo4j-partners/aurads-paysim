# aurads-paysim
These are instructions on Loading PaySim data into Neo4j AuraDS.

## Account Signup
First off, you're going to need to sign up for AuraDS.  You can do that [here](https://neo4j.com/cloud/graph-data-science/).

## Login to AuraDS
Once you have an account, you can login to it [here](https://console.neo4j.io/).

![](./images/1%20-%20login.png)

After you've logged in, you'll see the main screen.  Click `Create a Database`.

![](./images/2%20-%20main.png)


For "Database name" put "paysim"

For the "How big is you graph" questions, answer:
* Number of nodes - 500,000
* Number of relationships - 1,000,000

Under "Which algorithms are you going to use?" select: "Node Embedding"

Then click "Calculate Estimate" at the bottom of the screen.  

![](./images/3%20-%20estimate.png)

When that's complete, hit "Create Database."

![](./images/4%20-%20create.png)

You'll be presented with the password for your new database.  Be sure to copy that somewhere.

![](./images/5%20-%20password.png)

Your database will probably take a minute or two to setup.

![](./images/6%20-%20wait.png)

When that's all done you'll see this screen:

![](./images/7%20-%20ready.png)

Click on the database name, "paysim," to get to this page:

![](./images/8%20-%20detail.png)


## paysim

The generator code is [here](https://github.com/voutilad/PaySim-demo)