<p align="center">
  <img
    src="https://assets.moonlight.io/vi/moonlight-logo-dark-800w.png"
    width="400px"
    alt="Moonlight">
</p>

<p align="center" style="font-size: 48px;">
  <strong>Asteroid Load Balancer</strong>
</p>

<p align="center">
  A load balancer for neo full nodes
</p>

# Overview

Asteroid Load Balancer is a lightweight reverse proxy for neo full-nodes.  Currently, light applications need to manage node hopping to guarantee they are hitting a fully synched, available full-node.  This implementation provides an option for hitting a single server and allowing it to do the management and negotiation with full-nodes.

The current platform is very simple and uses a polling method for tracking block height and node state.  Node selection is random, but will eventually be dependent on latency.  Further future improvements will include the addition management tools.

The default deployment will register the City of Zion Nodes

Note: Listening port is 8080

<p align="center">
  <img
    src="fig1.svg"
    alt="Moonlight">
</p>

# Deployment
```sh
git clone https://github.com/Moonlight-io/asteroid-load-balancer.git
make build   
make run
```
