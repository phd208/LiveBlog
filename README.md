# LiveBlog
Mini-microservices blog app built with Node, React, Docker and Kubernetes

The goals of this project was to get a tast of microservices architecture and to build as much as possible from scratch. It was not meant as a template for future projects but just as a learning experience.

The mini-app allows user to make blog posts and to make comments on them.

Initial setup involved a react app generated using create-react-app and an express-based project for each of the services: posts, comments, query and moderation that are able to communicate with one another through the event-bus service. Then, a docker container was created for each one of the services, inside a kubernetes cluster.
