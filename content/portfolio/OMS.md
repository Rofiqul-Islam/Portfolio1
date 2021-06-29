---
title: OMS (Ontology Management System)
date: 2020-07-13T12:49:27.000+06:00
thumbnail: images/portfolio/Ontology.jpeg
service: Java, SpringBoot, Hibernate, Neo4j, Postgres, ReactJS
client: Software Engineering, CSI 5324, Baylor University 
shortDescription: Ontology Management System - enables experts to create and manage ontologies

  The system is for our experts who are going to build the ontologies, they will be adding/deleting/modifying nodes and edges and adding properties to nodes and edges. Experts can create categories for nodes (building components, physical activity, academic papers…) and categories for edges (IS_A, HAS_A…). Category is effectively a template for creating nodes and edges. Each category will define the type of a node or an edge. Next, both edge and node categories enable experts to define templates of properties that need to be filled when creating nodes or edges of that particular category. For instance, there is a category of a type “Building components” and I want that every node created in this category will have a name, next it will have 0 to N subcategories. Each subcategory will have a name and any number of properties, for example, String position, Date date, Enum orientation (west, north…). Same with categories for edges.

  Special category is the category “academic articles”. Experts can specify a search string, this search string will retrieve potentially hundreds of articles from Pubmed. The system scrapes title, doi and abstract from each article. All imported articles will have predefined subcategories and properties (will be provided in the separate document). Later, experts will fill the properties. There is a feature of assigning the nodes to the reviewer. Reviewers can approve or reassign the node or edge.

  There will be multiple experts working on one database at once, so some websockets will be definitely needed. We will use a graph database Neo4j on the backend and react front end with a Neo4j react graph library to build the ontologies. It is very important that our experts will create ontologies that are DAG (directed acyclic graph) compliant. We will use the PostgreSQL database for storing the accounts of our experts.
challenge: Ontology create, edit, delete, search. Visulize live ontology.
solution: Neo4J manages the graph operation of Ontology and ReactJS library pulls the heavy burden to visualize Ontology.

---
