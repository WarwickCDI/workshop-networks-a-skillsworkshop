Networks: A Skills Workshop
================

# Introduction

Do you want to learn a new skill as a historian? The Information and
Digital Group Technology for Research (IDGT4R) team has been asked to
lead an introductory practitioners’ approach on the applications of
social networks as a complimentary 90-minute component to a composite
session (Networks: A Skills Workshop). This practical part to be
preceded by a talk from Kate Davidson (Sheffield) on Social Network
Analysis from her article on Early Modern Social Networks: Antecedents,
Opportunities, and Challenges in American Historical Review.

## Learning objectives

• Upskill yourself with some techniques for exploring and visualizing
social networks

• Load and explore historical network data using Gephi

• Visualise historical network data with Gephi

• Reflect on some of the technicalities around network analysis

## Requirements

• Properly installed Gephi software version 0.9.2. You can find
installation guide here. Issues with Java, speak to helpdesk. Email if
stuck. If you encounter Gephi issues with Java, then you can also look
at this blog post and video

• Managed Windows Desktop access to Gephi or via Software Centre

• Access to a computer with internet connection for downloading data

• Data source for this workshop: Quakers

# Activity 1: Quakers Network

### Setup the folder for your work

Think about where on your computer that you want to work and create a
folder there. Preferably with a short path like “C:\\quakers”.

### Overview of the dataset and tabular content

Download the Quaker dataset as shown below in text and screenshots.

Go to the [sample data sets
page](https://github.com/melaniewalsh/sample-social-network-datasets) ->
Code -> Download Zipped folder into your project folder -> Unzip folder
with software such as [7zip](https://www.7-zip.org/) -> navigate
unzipped folder to “..\\sample-datasets\\quakers\\” and copy files into
your Gephi project folder or keep them where they are and use in your
Gephi project.

|                      |                      |
|----------------------|----------------------|
| ![](images/fig1.png) | ![](images/fig2.png) |

We are going to examine the relationships between 17th Century Quakers.
We have downloaded the data from [Melanie Walsh’s GitHub
repository](https://github.com/melaniewalsh/sample-social-network-datasets/tree/master/sample-datasets/quakers)
which contains other network datasets. The original data is taken from
this [excellent Programming Historian
tutorial](https://programminghistorian.org/en/lessons/exploring-and-analyzing-network-data-with-python).
Please refer to these pages for more information about the network.

We have a total of 96 nodes. Each node is a Quaker. If a Quaker has a
relationship with another Quaker then there is a line (edge) between the
two nodes. You will notice that there are 3 data files:

1.  quaker-nodes.csv
2.  quaker-edges.csv
3.  quakers-network.graphml

The quaker-nodes.csv and quaker-edge.csv files contain the nodes and
edges of our network respectively. The quaker-edges.csv file lists the
edges between the different nodes. The quakers-network.graphml file
contains both the nodes and edges of our network in one file.

Let us consider each of the files in turn:

#### quaker-nodes.csv

Each line contains the details of one node. You can view this file by
opening it in Excel or online
[here.](https://github.com/melaniewalsh/sample-social-network-datasets/blob/master/sample-datasets/quakers/quaker-nodes.csv)
Each node has an id, a label, the historical significance of the quaker,
their gender, birthdate, deathdate and something called other_id.

Have a look through the file and consider:

-   Are there more males than females?

-   What does the historical significance tell you?

-   Do you see any other trends?

#### quaker-edges.csv

Each line gives us the source and target node (you can view the file in
Excel or online
[here](https://github.com/melaniewalsh/sample-social-network-datasets/blob/master/sample-datasets/quakers/quaker-edges.csv)).
Network software will use this file to raw a line (edge) between the
source and target node, where the names in this file correspond to the
label in the quaker-nodes.csv file. Briefly looking through the file, do
you:

-   See any patterns?

-   Are some people very connected?

-   What do you think these patterns might mean?

#### quakers-network.graphml

Both the nodes and edges are included in this file. The file is
formatted as xml (see the file
[here](https://github.com/melaniewalsh/sample-social-network-datasets/blob/master/sample-datasets/quakers/quakers-network.graphml)
if you are curious) which is usually written out by a piece of software
for networks. We do not need to know much about this file as we have
already familiarised ourselves with the nodes and edged in the previous
files. The graphml file contains these nodes and edges, along with some
further data about the colour and position the nodes should have.

### Import into Gephi and ‘first draw’

We have our network data, but we want to see the network. The power of
networks is in seeing the collective interconnections between nodes and
exploring the emergent properties of the network – which we cannot see
by examining nodes or edges in isolation.

One rather excellent piece of software for this is
[Gephi](https://gephi.org/) (though alternative packages, including
those for the R and Python programming languages, are
[available](https://alternativeto.net/software/gephi/)).

Here we will go through the process of loading our csv files into Gephi
(to create our network) and loading in the graphml file (our complete
network).

1.  Click new project. Go to File -> New Project to create a new Gephi
    project file. Alternatively, you can use the link in the welcome
    dialog that pops up when you first open Gephi.

    ![](images/fig3.png)

2.  Click on file and select ‘Import Spreadsheet’

    ![](images/fig4.png)

3.  Choose the quaker-nodes.csv file and choose open.

    ![](images/fig5.png)

4.  You should see the import dialogue box. As shown below, Gephi should
    identify the file as a Nodes table, and you should see the columns
    from the csv.

    ![](images/Nodes%20table.png)

5.  Click on Next and Finish to see the import report. The import report
    should show you that 96 nodes have been imported.

    ![](images/fig7.png)

6.  Click on OK and your network will contain nodes!

    ![](images/fig8.png)

7.  Go through the same (above) process of importing a spreadsheet but
    select the quaker-edges.csv file. It should recognise the file as an
    edges table.

    ![](images/fig6.png)

8.  Clicking Next and Finish, the import result should now show **96
    nodes** and **162 edges**.

    ![](images/edges%20table%20import%20report%20dialog.png)

9.  You should now see the network!

    ![](images/Visualisation%20of%20Nodes%20and%20Edges%20after%20imports.png)

10. asdfasdf
