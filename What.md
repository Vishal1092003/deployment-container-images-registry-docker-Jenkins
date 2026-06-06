```#docker => it is a software tool which helps in managing and running the container```

```#container => it is an isolated package or isolated environment that contain your code ,tool and settings needed to run it .```

```#image =>this is just version of your application.```

```#registry => A Registry is a digital warehouse (like GitHub or Google Drive) where you store and share your Docker images```


<img width="1030" height="450" alt="image" src="https://github.com/user-attachments/assets/6802ca6d-a20e-4930-bd6a-09dad362afac" />


# Role of Kubernetes

Kubernetes helps manage and orchestrate containers at scale.

## Key Responsibilities

1. **Deploys containers across multiple servers**
   - Runs containers on a cluster of machines instead of a single server.

2. **Scales applications automatically**
   - Increases or decreases the number of container instances based on demand.

3. **Restarts failed containers**
   - Monitors container health and automatically replaces failed containers.

4. **Load balances traffic**
   - Distributes incoming requests across multiple container instances.

5. **Manages updates and rollbacks**
   - Performs rolling updates with minimal downtime and can revert to previous versions if needed.

6. **Orchestrates containers across a cluster**
   - Coordinates thousands of containers running on multiple machines.

---

# Simple Analogy

| Component | Analogy |
|------------|----------|
| **Docker** | Builds and runs a single container |
| **Container** | The packaged application |
| **Image** | The blueprint/template for the application |
| **Registry** | The warehouse that stores and shares images |
| **Kubernetes** | The manager that coordinates many containers across many machines |

---

# Typical Workflow

```text
Registry → Image → Container
                ↑
              Docker

Kubernetes → Manages, scales, and orchestrates containers

<img width="962" height="392" alt="image" src="https://github.com/user-attachments/assets/96ffe263-556e-40a1-99bc-2d19f47116a3" />


