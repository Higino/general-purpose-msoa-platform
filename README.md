# general-purpose-msoa-platform
A general purpose multi provider service oriented architecture platform so you can build services in convention over configuration design paradigm 

# Conventions
Every microservice defines its own infrastructure
Every microservice should aim for zero dependencies
A dependency is defined as a shared resource not owned (created) by some particular service
When dependencies are needed they are created in common-infra directory
