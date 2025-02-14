<a name="readme-top"></a>

---

<br />
<div align="center">
  <a href="https://github.com/OriginTrail/edge-node-installer">
    <img src="images/banner.jpg" alt="OriginTrail Edge Node Banner">
  </a>

  <h3 align="center"><b>OT-Edge-Node</b></h3>

  <p align="center">
    </br>
    <a href="https://docs.origintrail.io/">OriginTrail Docs</a>
    ·
    <a href="https://github.com/OriginTrail/edge-node-installer/issues">Report Bug</a>
    ·
    <a href="https://github.com/OriginTrail/edge-node-installer/issues">Request Feature</a>
  </p>
</div>

</br>

<details open>
  <summary>
    <b>Table of Contents</b>
  </summary>
  <ol>
    <li>
      <a href="#about-the-project">📚 About The Project</a>
        <ul><li><a href="#what-is-the-decentralized-knowledge-graph">What is the Decentralized Knowledge Graph?</a></li>
        <li><a href="#what-is-the-difference-between-a-core-node-and-an-edge-node">What is the difference between a Core Node and an Edge Node?</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">🚀 Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#edge-node-setup">Edge Node Setup</a></li>
        <li><a href="#build-on-dkg">Build on DKG</a></li>
      </ul>
    </li>
    <li><a href="#license">📄 License</a></li>
    <li><a href="#contributing">🤝 Contributing</a></li>
    <li><a href="#social-media">📰 Social Media</a></li>
  </ol>
</details>

---

## DKG Edge Node v1.0.1

This installer provides an easy way to set up and run a DKG Edge Node on your system. 

For more details on the DKG Edge Node, visit the official documentation [here](https://docs.origintrail.io/build-with-dkg/dkg-edge-node).

<br/>

## About The Project

<details open>
<summary>

### **What is the Decentralized Knowledge Graph?**

</summary>

<br/>

<div align="center">
    <img src="images/nodes.png" alt="Knowledge Asset" width="200">
</div>

OriginTrail Decentralized Knowledge Graph (DKG), hosted on the OriginTrail Decentralized Network (ODN) as trusted knowledge infrastructure, is shared global Knowledge Graph of Knowledge Assets. Running on the basis of the permissionless multi-chain OriginTrail protocol, it combines blockchains and knowledge graph technology to enable trusted AI applications based on key W3C standards.

</details>

<details open>
<summary>

### **What is the difference between a Core Node and an Edge Node?**

</summary>

<br/>

The OriginTrail DKG V8 network is comprised of two types of DKG nodes - Core Nodes, which form the DKG network core and host the DKG, and Edge Nodes, which run on edge devices and connect to the network core. The current beta version is designed to operate on edge devices running Linux and MacOS, with future support for a wide range of edge devices such as mobile phones, wearables, IoT devices, and generally enterprise environments. This enables large volumes of sensitive data to safely enter the AI age while maintaining privacy.
</details>
<p align="right">(<a href="#readme-top">back to top</a>)</p>
<br/>

## Prerequisites

Before proceeding, ensure your system meets the following requirements:


### System Requirements


- **OS**: Linux (Ubuntu 24.04, Ubuntu 22.04 and Ubuntu 20.04 are currently supported)

- **RAM**: At least 8 GB

- **CPU**: 4 Cores

- **Storage**: At least 20 GB of available space

- **Network**: Stable internet connection

### Software Dependencies

Ensure the following services are installed:

- Git


## Edge Node Setup

### 1. Clone the Repository
To begin, copy the following code:

 ```bash
git clone https://github.com/OriginTrail/edge-node-installer
```


### 2. Set the Environment Variables File
Once you have cloned the repository, navigate to the directory and set the environment variables:

1. Open the `.env.example` file:

 ```bash
nano .env.example
```

2. Fill in the required parameters.


3. After completing configuring the environment file, rename it to `.env`:

 ```bash
mv .env.example .env
```


### 3. Execute the Installer
To execute the installation, run the following command:

 ```bash
bash edge-node-installer.sh
```


### 4. Usage
Once the installation is complete, you can access the user interface by navigating to:

```bash
    http://your-nodes-ip-address
```

The default login credentials are:

- **Username:** my_edge_node
- **Password:** edge_node_pass

**Important:** It is highly recommended to change the default credentials.

</br>

## Build on DKG

<br/>

The OriginTrail SDKs are client libraries for your applications, used to interact and connect with the OriginTrail Decentralized Knowledge Graph.
From an architectural standpoint, the SDK libraries are application interfaces into the DKG, enabling you to create and manage Knowledge Assets through your apps, as well as perform network queries (such as search, or SPARQL queries), as illustrated below.

<div align="center">
    <img src="images/sdk.png" alt="SDK" width="200">
</div>

The OriginTrail SDK libraries are being built in various languages by the team and the community, as listed below:

-   dkg.js - V8 JavaScript SDK implementation
    -   [Github repository](https://github.com/OriginTrail/dkg.js/tree/v8/develop)
    -   [Documentation](https://docs.origintrail.io/dkg-v8-upcoming-version/v8-dkg-sdk/dkg-v8-js-client)
-   dkg.py - V8 Python SDK implementation
    -   [Github repository](https://github.com/OriginTrail/dkg.py/tree/v8/develop)
    -   [Documentation](https://docs.origintrail.io/dkg-v8-upcoming-version/v8-dkg-sdk/dkg-v8-py-client)

---

<br/>
<p align="right">(<a href="#readme-top">back to top</a>)</p>

## License

Distributed under the Apache-2.0 License. See `LICENSE` file for more information.

<br/>

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

By testing the DKG Edge Node, and the installer, and sharing your feedback, you help us refine the setup process and improve the overall experience. If you encounter any issues or have suggestions, please let us know! 🐛
For detailed instructions on setting up the DKG Edge Node in an automated environment on Ubuntu, check out the official documentation [here](https://docs.origintrail.io/build-with-dkg/dkg-edge-node/run-an-edge-node/automated-environment-setup-ubuntu).

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<br/>

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Social Media

<br/>

<div align="center">
  <a href="https://medium.com/origintrail">
    <img src="images/icons/medium.svg" alt="Medium Badge" width="30" style="margin-right: 10px"/>
  </a>
  <a href="https://t.me/origintrail">
    <img src="images/icons/telegram.svg" alt="Telegram Badge" width="30" style="margin-right: 10px"/>
  </a>
  <a href="https://x.com/origin_trail">
    <img src="images/icons/x.svg" alt="X Badge" width="30" style="margin-right: 10px"/>
  </a>
  <a href="https://www.youtube.com/c/origintrail">
    <img src="images/icons/youtube.svg" alt="YouTube Badge" width="30" style="margin-right: 10px"/>
  </a>
  <a href="https://www.linkedin.com/company/origintrail/">
    <img src="images/icons/linkedin.svg" alt="LinkedIn Badge" width="30" style="margin-right: 10px"/>
  </a>
  <a href="https://discord.gg/cCRPzzmnNT">
    <img src="images/icons/discord.svg" alt="Discord Badge" width="30" style="margin-right: 10px"/>
  </a>
  <a href="https://www.reddit.com/r/OriginTrail/">
    <img src="images/icons/reddit.svg" alt="Reddit Badge" width="30" style="margin-right: 10px"/>
  </a>
  <a href="https://coinmarketcap.com/currencies/origintrail/">
    <img src="images/icons/coinmarketcap.svg" alt="Coinmarketcap Badge" width="30" style="margin-right: 10px"/>
  </a>
</div>

---
