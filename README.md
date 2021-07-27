# LiveBlog
Mini-microservices blog app built with Node, React, Docker and Kubernetes

The goals of this project was to get a tast of microservices architecture and to build as much as possible from scratch. It was not meant as a template for future projects but just as a learning experience.

The mini-app allows user to make blog posts and to make comments on them.

Initial setup involved a react app generated using create-react-app and an express-based project for each of the services: posts, comments, query and moderation that are able to communicate with one another through the event-bus service. 

Data is shared between services via async communication, focusing on communicating changes using event sent to an even-bus – which provides a certain level of self-sufficiency to each service, making it relatively easy to hangle temporary downtime or new service creation.

All services are packaged up using Docker, inside a kubernetes cluster in order to facilitate deployment and scaling.
