# aurads-paysim
These are instructions on Loading PaySim data into Neo4j AuraDS.  They're intended to be a prerequisite to running the notebook [here](https://github.com/GoogleCloudPlatform/vertex-ai-samples/blob/master/notebooks/community/neo4j/graph_paysim.ipynb).

## Account Signup
First off, you're going to need to sign up for AuraDS.  You can do that [here](https://neo4j.com/cloud/graph-data-science/).

## Login to AuraDS and Create a Database
Once you have an account, you can login to it [here](https://console.neo4j.io/).

![](./images/01%20-%20login.png)

After you've logged in, you'll see the main screen.  Click `Create a Database`.

![](./images/02%20-%20main.png)

For "Database name" put "paysim"

For the "How big is you graph" questions, answer:
* Number of nodes - 500,000
* Number of relationships - 1,000,000

Under "Which algorithms are you going to use?" select: "Node Embedding"

Then click "Calculate Estimate" at the bottom of the screen.  

![](./images/03%20-%20estimate.png)

When that's complete, hit "Create Database."

![](./images/04%20-%20create.png)

You'll be presented with the password for your new database.  Be sure to copy that somewhere.

![](./images/05%20-%20password.png)

Your database will probably take a minute or two to setup.

![](./images/06%20-%20wait.png)

When that's all done you'll see this screen:

![](./images/07%20-%20ready.png)

Click on the database name, "paysim," to get to this page:

![](./images/08%20-%20detail.png)

## Import Data
Now click on the "Import Database" tab.

![](./images/09%20-%20import.png)

Click "Select a .dump file" and select the paysim.dump file from [here](xxx).

![](./images/10%20-%20import.png)

Click "Upload" to ignore the warning that this will overwrite your database.  The database is brand new and empty, so that's not really an issue.

![](./images/11%20-%20import.png)

A progress bar will be displayed while the upload proceeds.

![](./images/12%20-%20loading.png)

The database will then spend a few minutes processing the upload.

![](./images/13%20-%20loading.png)

When all done, it looks like the screenshot above.

Now that you're all done with the database setup, you're ready to run the notebook that will showcase using Neo4j AuraDS with GCP Vertex AI.  That is [here](https://github.com/GoogleCloudPlatform/vertex-ai-samples/blob/master/notebooks/community/neo4j/graph_paysim.ipynb).