

# 📦 Kubernetes YAML Examples

This repository contains a **comprehensive set of Kubernetes YAML manifests** for learning and practicing different Kubernetes concepts. Each file demonstrates a specific Kubernetes resource or configuration, making it a handy reference for both beginners and advanced users.

---

## 📂 Repository Structure

### 🔹 Core Workloads

* `podspec.yaml`, `devpod.yaml`, `expod.yaml` – Basic Pod specifications
* `dep.yaml`, `nginx-deployment.yaml` – Deployments
* `rc.yaml`, `repc.yaml` – ReplicationController examples
* `replicasetpod.yaml`, `replicasetmatchlabel.yaml`, `matchexpressionset.yaml` – ReplicaSet demos

### 🔹 Services & Networking

* `svc.yaml`, `nginx-service.yaml` – ClusterIP services
* `Nodeport.yaml`, `lb.yaml` – NodePort & LoadBalancer services
* `headless.yaml` – Headless service
* `svcwithoutsel.yaml`, `ep.yaml` – Endpoint service
* `ingressdeploy.yaml` – Ingress with deployment

### 🔹 Storage

* `pv.yaml`, `pvc.yaml`, `pvpod.yaml` – PersistentVolume, PersistentVolumeClaim, and pod usage
* `emptydirpod.yaml` – Using `emptyDir`
* `resource-pod.yaml`, `rquota.yaml` – Resource requests, limits & quotas

### 🔹 Configs & Secrets

* `cm.yaml`, `cm-pod.yaml` – ConfigMaps
* `sec.yaml`, `secenvpod.yaml`, `secvolpod.yaml` – Secrets (env & volume usage)

### 🔹 Probes

* `livenessprobe.yaml` – Liveness probe
* `readinessprobe.yaml` – Readiness probe
* `startupprobe.yaml` – Startup probe

### 🔹 Scheduling

* `nodeselector.yaml`, `nodeaffinity.yaml` – Node selection & affinity
* `podaff.yaml`, `podaffnity.yaml`, `podantiaff.yaml`, `podantiaffinity.yaml` – Pod affinity & anti-affinity
* `with-affinity-antiaffinity.yaml` – Combined scheduling rules
* `toleration.yaml` – Tolerations for taints

### 🔹 RBAC & Security

* `role.yaml`, `rolebind.yaml` – Role & RoleBinding
* `clusrole.yaml`, `clusbinding.yaml` – ClusterRole & ClusterRoleBinding
* `ru.yaml`, `sf.yaml`, `mb-config.yaml` – Security-related configs

### 🔹 Miscellaneous

* `components.yaml` – Multi-component manifest
* `ns.yaml` – Namespace definition
* `metrics.yaml` – Metrics-related resource
* `multicont.yaml` – Multi-container pod
* `lrange.yaml` – Label range selector demo

---

## 🚀 How to Apply

1. Clone the repository:

   ```bash
   git clone https://github.com/<your-org>/<your-repo>.git
   cd <your-repo>
   ```

2. Apply any manifest to your Kubernetes cluster:

   ```bash
   kubectl apply -f dep.yaml
   kubectl get pods
   ```

3. Clean up:

   ```bash
   kubectl delete -f dep.yaml
   ```

---

## 🎯 Learning Outcomes

By using this repository, you will learn:

* How to deploy applications with **Pods, Deployments, and ReplicaSets**
* Exposing apps via **ClusterIP, NodePort, LoadBalancer, and Ingress**
* Managing storage with **Persistent Volumes, PVCs, and EmptyDir**
* Configuring **ConfigMaps and Secrets** securely
* Implementing **Probes for health checks**
* Applying **scheduling techniques** (nodeSelector, affinity, tolerations)
* Setting up **RBAC for access control**

---

## 📌 Next Steps

* Add **Helm charts** for templated deployments
* Provide **real-world multi-tier app examples**
* Integrate with **CI/CD pipelines** (ArgoCD, Flux, Jenkins)

.

