# vCluster Playground 🚀

Welcome! This playground gives you a real Kubernetes environment to explore **vCluster** — a tool that lets you create lightweight, isolated virtual Kubernetes clusters inside a host cluster.

📖 [vCluster Documentation](https://www.vcluster.com/docs)

---

## What is vCluster?

vCluster runs a virtual Kubernetes cluster inside a namespace of a real cluster. Each virtual cluster has its own API server and resources, fully isolated from others — perfect for development, testing, and multi-tenancy.

---

## Get Started

**1. Create a virtual cluster**
```bash
vcluster create dev-cluster -n dev
```

**2. Connect to your virtual cluster**
```bash
vcluster connect dev-cluster -n dev
```

**3. Explore inside the virtual cluster**
```bash
kubectl get nodes
kubectl get namespaces
```

**4. List all virtual clusters**
```bash
vcluster list
```

**5. Disconnect from the virtual cluster**
```bash
vcluster disconnect
```

**6. Delete the virtual cluster**
```bash
vcluster delete dev-cluster -n dev
```

---

> 💡 **Tip:** Don't worry about breaking anything — this is a sandboxed environment. Feel free to explore!
