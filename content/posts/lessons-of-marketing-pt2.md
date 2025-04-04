---
title: 'Lessons of Marketing Pt. 2'
date: 2024-12-19
published: true
locale: 'en'
tags: ['Events']
cover_image: ./images/lessons-of-marketing-pt2/cover.png
description: "In our previous publication, we analyzed Robonomics' annual marketing activities. In this blog post, we will look at Robonomics through the lens of crypto community expectations. And we'll discuss why we don't want to follow them."
abstract: "In our previous publication, we analyzed Robonomics' annual marketing activities. In this blog post, we will look at Robonomics through the lens of crypto community expectations. And we'll discuss why we don't want to follow them. Ivan Berman [Fingerling42]" 
---

## Conclusions of the First Lesson

Before we begin, let's consolidate the general conclusions of the first lesson. One of the main differences between Robonomics and other DePIN projects is the amount of attention we pay to activities for the crypto community. We have been and continue to remain focused on implementing XRT tokenomics solely for user needs. The idea is to focus tokenomics on activities that are useful for the operation of the network itself, rather than on crypto activities (staking, airdrops, yarn fests). Although they are expected by the community, they are detrimental in the long term for the product.

As a result, it turned out that by 2024, even if your project is in the most discussed topic of the year (DePIN) and has a long history (more than 9 years), but your tokenomics is focused on the technical side of the project, then you cannot expect support from the crypto community. A sad choice — either you follow the trends, or you look for an another audience, even if your project is technologically based on Web3.

## Dusk Site of Robonomics

Let's say we wanted to look fancy and beautiful for the crypto community by promising an airdrop to everyone who connects their phone to our network to count it as a “device”. What would Robonomics look like if we used marketing tricks? For clarity, we prepared a website mockup (thanks to our designers!) where we gathered the most striking metrics that, based on my observations, are currently the main goals for most projects offering their tokens. Let's look at them, discuss, and try to draw a useful conclusion for Robonomics marketing in 2025.

Behold, the Robonomics website from a parallel dusk universe:

(It is also available for viewing on [Figma](https://www.figma.com/proto/owWejYYXtE70tgU74sDQ5e/Untitled?node-id=1-2&node-type=canvas&t=iLQQ4HrIkYPeyfoo-1&scaling=scale-down&content-scaling=fixed&page-id=0%3A1&starting-point-node-id=1%3A2&share=1))

<rb-image zoom src="./images/lessons-of-marketing-pt2/dusk-robo-site.webp" alt="Dusk Site of Robonomics" />

## Large Number of Devices (but it's impossible to tell if they are connected to the network)

This is one of the favorite metrics for projects as it demonstrates the payload capacity of DePIN infrastructure. And it's even more frustrating that it's so easy to manipulate. For starters, no one will write the explicit "Actual Number of Devices Currently Connected to Our Network". It will always be something indirect or vague, like "supported devices" in our example. What does this really mean? Has each device been tested for compatibility with our software? And how many of them are actually online?

Actually, to get it, we simply took the number of smart device models compatible with Home Assistant and the number of robot models that support Robot Operating System. Since we have an integration for Home Assistant and a wrapper package for ROS, we can claim that *theoretically* all these devices will work with our network. Is this claim false? Formally, no. But does it give a idea of the real performance of the network? Hardly.

In the best case scenario, indicators of the number of connected devices should be displayed online, based on on-chain information, in a way that allows anyone to verify them independently. At the very least, we can show the number of useful transactions. For example, anyone can check how many datalogs are executed in Robonomics daily through the Subscan service.

## Many Users (but it's unclear who they are)

This is another popular metric for any crypto project in general. This time, we similarly estimated the number of users and companies that use supported devices, and assumed that all of them are ready to use our product. By combining vague phrases and theoretical indicators, we can achieve quite impressive numbers. 

But there's another nuance with users in DePIN. Just by providing these statistics, you won't be able to know the quality of these users. Often, it's taken from the simple number of active addresses in the network with non-zero balances. Meanwhile, almost all DePIN projects attract users through staking, airdrops, and loyalty programs. It's practically impossible to distinguish between users who came to the project purely to earn money and users who actually use the infrastructure. But then it's impossible to understand whether the project is fulfilling its main function, or if it's just another hype. Again, the solution here is to categorize users and track whether they generate useful infrastructure transactions.

## Numerous Collaborations (but their results are not visible or useful)

Let me introduce you to this impressive list of colleagues, partners, and projects from various fields with whom Robonomics has collaborated over the years. All examples are real, and evidence for each can be found on the Internet. If you're interested, here's a brief summary:

**Academy**:

- MIT Media Lab — scientific publications and conferences: decentralized technologies in smart cities, the Gaka-chu robot artist project
- ITMO University — numerous scientific publications, conferences and events dedicated to robotics
- Waseda University — Rally Show 2018 on robots, AI and cognitive services at Waseda University
- National Research Council of Italy — scientific publication dedicated to trustable environmental monitoring with sensors network
- University of Applied Sciences Upper Austria — participation in our grant program on the topic of digital twins in logistics
- Victoria University of Wellington — participation in our grant program on the topic of blockchainization for farm pollution in New Zealand with sensor networks
- Hamburg University of Applied Sciences — participation in our grant program on the topic of object identities based on the sensorchain for production processes

**EU & US Institutions**:

- UN Climate Change — delegates for UN Climate Change conferences (COP23, COP24) on on-chain carbon credits topic
- European Parliament — The Economy of Robots workshop at European Parliament
- European Commission — participation in the BC4ECO consortium dedicated to the utilization of distributed ledger technologies
- International Civil Aviation Organization — creation of a development plan for the UAS traffic management system
- US Federal Aviation Administration — project of UAS remote identification system
- World Economic Forum — talk at WEF 2022 on the topic of machine economy

**Robotics and IoT Leaders:**

- open source Robotics Alliance and ROS 2 — support for Rust bindings for ROS 2, search for Web3 applications for robotics
- Boston Dynamics — system for log storage in Web3 cloud for the Spot robot, creating courses on Spot SDK
- KUKA — KUKA manipulator control system via Web3 cloud, the Gaka-chu robot artist project
- Universal Robots — the Eisenkoch robot baker project
- Libelium — water quality control system for rivers and lakes based on a water drone
- FANUC — FANUC manipulator control system via Web3 Cloud
- Home Assistant — smart home integration to decentralized cloud with remote control and backup service functions
- Tasmota — creation of open-source firmware for open-hardware devices, support of Tasmota repository

**Enterprises**:

- Microsoft — adding Robotics-as-a-Service to Microsoft Azure, Ethereum training for company employees
- BMW — winning the BMW-backed MOBI Grand Challenge to create unmanned traffic management
- SAIC Motor — research project on the topic of decentralized infrastructure for UAS fleet management
- Techstars — successful graduation of MerkleBot from Techstars Accelerator Program
- Tata Communications — work on the Distributed Sky initiative to create the UAS traffic management system
- Civic — partnership for the use of their identity verification services
- DJI —  work on the Distributed Sky initiative
- AirMarket — work on the UAS traffic management system
- DroneDeploy — work on a project to create Blockchain Drone Identity (BDID)
- iotAIR — demonstration of machine-to-machine payments and data marketplace using the example of UAS fleet
- InterUSS — work on the Distributed Sky initiative
- bbf: — integration of carbon offset tracking system for solar panels in bbf residential complex
- INEX — integration of smart automation for 20 apartments of the INEX residential complex

**Web3**:

- P2P — launch of a parachain on the Kusama network with the support of P2P Validator
- Protocol Labs — first use of IPFS in DePIN, commitment within the accelerator program
- Parity Technologies — Parity-as-a-Service project on NixOS, demo with first robot launch on Substrate
- Web3 Foundation — a grant on Robotics integration in Polkadot
- Ethereum Foundation — first showcase of cyber-physical systems on Ethereum (Devcon 5)
- Polkadot — working parachain, active participation in ecosystem events
- Kusama — working parachain, active participation in ecosystem events
- Ocean Protocol — IoT data utilization demo for Ocean marketplace
- MixBytes — creation of XCMP + Robobank demo, work on the Distributed Sky initiative
- Crust Network — integration for sending device data to Crust
- RMRK — RMRK pallet support for NFT integration with devices and robots

However, we don't display these badges on the main page. In fact, this is another plague of projects, especially startups, and not just in the DePIN sphere. The problem with collaborations is that they can't be lumped together without considering the context of what was actually accomplished within them. For example, when we talk about Microsoft, Boston Dynamics, and MIT Media Lab, these are three completely different levels of relationships, and consequently, different collaboration outcomes with each other.

Another sin that can be found among startups is announcing collaborations without actually doing the work. After all, in a few months or years, no one will remember whether anything was done or whether it remained just a statement of intent.

Of course, activities with other projects and partners are important. However, we should follow a simple rule — "*Talk is cheap. Show me the code*", or more precisely, any artifacts of your collaboration. We strive to share results in our blog, upload them to GitHub, and compile them into annual R&D books.

Another option is to prominently display only the integrations and collaborations that are currently in use. In Robonomics' case, it would look like this:

- open source Robotics Alliance
- Home Assistant
- Tasmota
- Protocol Labs
- Parity Technologies
- Polkadot
- Kusama
- Crust Network

## Conclusions of the Second Lesson

In conclusion, giant numbers on the page and important badges is not what drives a project. It is worth displaying collaborations and indicators that are useful for the project, in which you see a sustainable continuation, and which are important to you as a growth driver. We will also follow this conclusion, and in 2025, we will try to pay more attention to reporting on the activity of devices integrated into Robonomics, and on the collaborations we use in our current tasks.

I hope you found this analysis interesting and learned a bit more about our views on marketing. At Robonomics, we strive to share important values and results with the community, rather than deceiving you with excessive promises or throwing dust in your eyes.