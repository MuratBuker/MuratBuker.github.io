---
tittle: Using Jekyll For a Mark Down Blog !
date: today
categories: [homelab, website, blog, markdown]
tags: [markdown, vs code, kubernetes, nginix]
---

# Installing K3S Cluster



~~~bash
curl -sfL https://get.k3s.io | INSTALL_K3S_VERSION="v1.26.12+k3s1" sh -s - server --node-taint 'node-role.kubernetes.io/master=true:NoSchedule'
~~~~  

~~~~bash
curl -sfL https://get.k3s.io | K3S_TOKEN="K10631f4f17992bb7d3283318d18bcf75c742f59257d0159cf415bd3dd340c23ebd::server:f29eceec3fdf971bd9935a7eb1d26fc0" K3S_URL="https://192.168.1.130:6443" K3S_NODE_NAME="worker-node01" INSTALL_K3S_VERSION="v1.26.12+k3s1" sh -

~~~~
