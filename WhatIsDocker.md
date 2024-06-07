![alt text="docker"](/docker-definition.webp)

# What is Docker Summary

- Docker is a set of **PaaS** products that use OS-level virtualization to deliver containerized software.
- Open-source **containerized** platform

## How does Docker Work?

- Docker creates, manages, and runs continers
- Contains libraries, bin, config file, dependencies
- All containers share **one underlying OS**

![alt text="how does docker work"](/how-does-docker-work.webp)

## Why is Docker popular?

- Dockers technology heavily relies on **Cgroups** or **control groups**
- Allows the ability to allocate, share and/or restrict resources across processes and namespaces
- Same features and benefits of \*\*virtual machines (VMs), such as
  - application separation
  - cost-effective scalability
  - disposability

![alt text](/why-is-docker-so-popular.webp)

- Lighter than VMs because they dont carry the payload of the OS and hypervisor; instead they only carry the required dependencies

* shared software
* reduced images sizing means lower cloud storage costs
* Containers are faster and easier to deploy, provision, and restart than VMs, which makes them a better fit for dev teams and **CI/CD** pipelines

## Why Use Docker?

- Docker native Linux containerization
- **Portability**: runs without alteration across desktops, data center and cloud environments
- **Granularity** - updaes are lighter and more granular. Each Docker container can only run one process at a time
- **Automation** - Automated container creation using source code
- **Reusability** - Existing containers can be utilized as basis images and templates
- **Shared Libraries** - Large open-source registry of user-contributed containers through shared libraries

## Docker Components

- **Docker Engine** - funamental technology that manages creation
- **Server-side Daemon** - hosted server-side daemon hosts images, containers, networks and storage created by the Engine
- **CLI** - Users can interact with daemon using CLI
- **Dockerfiles** - **containers** **built** by Docker
- **Docker Compose files** - files specify how components in container are put together

- \*_Docker Hub_ - software-as-a-service central repository that allows publication and sharing of container-based programs

- **Universal Control Plane** - unified cluster and app admin interface via web

- **Compose** - command-line utility for configuring multi-container application services, viewing container status, streaming log output, and running single-instance processes

- **Content Trust** - security to register user signs and image metadata to validate the integrity of distant Docker registries

## Docker Deployment and Orchestration

- Uses Docker Engine good for a few containers
- Use **Docker Compose** for large scale containers and workflows

  ### Docker Compose

  - Docker Compose generates **YAML** file indicates which serves are included, deployment, operate
  - Also, create persistante storage volumes, designate base notes, and document and config service requirements

  ### Kubernetes

  - In larger, more sophisticaed setups, need a container orchestration tool to monitor and manage container lifecycles.
  - Can also use **Docker Swarm** for orchestration, most devs prefer Kubernetes
  - **Kubernetes** manages container-based systems by scheduling and automating processes like deployment, updates, discovery, storage provisioning, load balancing, health monitoring, and more.

## Advantages and Disadvantages of Docker

### Advantages

- Rapid composing, creating, deploying, scaling, and managing containers
- Portability register and share containers across private and pubich env
- Compared to VMs more efficient development, lower resource usage, and faster deployment

  ![alt test](/advantages-and-disadvantages-of-docker.webp)

### Disadvantages and drawbacks

- Potential large number of containers can be challenging to manage
- Distribution and connectivity across multiple hundreds of ephemeral containers can be challenging
