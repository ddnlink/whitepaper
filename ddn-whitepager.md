DDN Whitepaper
---------

—— A Blockchain System for Enterprise 

Version 1.0.0

From DDN Foundation

Dec. 12th, 2017

## Special Notes
After several times of discussion and modification, we finally publish the version of v1.0.0. It focuses on the strategic goals and development roadmap of DDN network, which will offer appropriate methods to help organizations gain more autonomy.

You can visit the official website of DDN to learn more information about whitepaper update, roadmap, team members, foundation, partners and recent projects.

**Official Links**
- DDN Official Website：http://ddn.link
- DDN Core Chain Mainnet：http://mainnet.ddn.link
- DDN Core Chain Testnet：http://testnet.ddn.link
- DDN Source Code Library：https://github.com/ddnlink
- DDN Whitepaper：https://github.com/ddnlink/whitepaper

**Social Media Accounts**
- DDN Technology Community：http://ddn.link/community
- DDN Chinese Community – QQ Group：669624212；
- DDN Wechat ID：@DDN_link；
- DDN Weibo：@DDN_link；
- DDN Twitter：@DDN_link；
- DDN Telegram (Chinese)：@ddnlinkCN；
- DDN Telegram (English)：@ddnlink;
- **E-mails**
    * Business Cooperation:  operation@ddn.link；
    * Technical Support:  support@ddn.link；
    * Recruitment:  hr@ddn.link

- **Listed Exchanges**
    * bit-z：http://www.bit-z.com/
    * Bitshares exchange：https://bitshares.org/download/
    * bbaex：https://www.bbaex.com/
    * fubt:  https://www.fubt.top/

## Table of Contents

<!-- TOC -->

- [Special Notes](#special-notes)
- [Table of Contents](#table-of-contents)
- [1. Abstract](#1-abstract)
- [2. Terminology](#2-terminology)
- [3. Goals](#3-goals)
- [4. Background](#4-background)
    - [4.1 The Origin Intention of Internet is Resources Connection](#41-the-origin-intention-of-internet-is-resources-connection)
    - [4.2 User Data Belongs to Users Themselves](#42-user-data-belongs-to-users-themselves)
    - [4.3 The Core of Blockchain is the Rule of Interest Transferring](#43-the-core-of-blockchain-is-the-rule-of-interest-transferring)
    - [4.4 The Ultimate Status of Enterprise is High Degree of Autonomy](#44-the-ultimate-status-of-enterprise-is-high-degree-of-autonomy)
- [5. Significance](#5-significance)
    - [5.1 To Solve Enterprise (or Industrial) Pain Points](#51-to-solve-enterprise-or-industrial-pain-points)
    - [5.2 To Improve Enterprise Operating Efficiency](#52-to-improve-enterprise-operating-efficiency)
    - [5.3 To Expand Market Share](#53-to-expand-market-share)
    - [5.4 To Expand Brand Influence](#54-to-expand-brand-influence)
- [6. Basic Architecture](#6-basic-architecture)
    - [6.1 Architecture diagram](#61-architecture-diagram)
    - [6.2 Key Technology](#62-key-technology)
    - [6.3 Main features](#63-main-features)
        - [6.3.1 Multi-chain parallelism](#631-multi-chain-parallelism)
        - [6.3.2 Modular Design](#632-modular-design)
        - [6.3.3 Visual Customization](#633-visual-customization)
        - [6.3.4 Multi-terminal Use](#634-multi-terminal-use)
- [7.Core Technology](#7core-technology)
    - [7.1 DDN Blockchain](#71-ddn-blockchain)
        - [7.1.1 Consensus Mechanism](#711-consensus-mechanism)
        - [7.1.2 Reward Mechanism](#712-reward-mechanism)
        - [7.1.3 Trustees](#713-trustees)
        - [7.1.4 Peer-to-peer (P2P) networks](#714-peer-to-peer-p2p-networks)
    - [7.2 Sidechain Technology](#72-sidechain-technology)
        - [7.2.1 Virtual Machine](#721-virtual-machine)
        - [7.2.2 Dapp development](#722-dapp-development)
        - [7.2.3 Dapp Operation](#723-dapp-operation)
        - [7.2.4 Dapp Consensus Algorithm](#724-dapp-consensus-algorithm)
        - [7.2.5 Dapp Master Node](#725-dapp-master-node)
    - [7.3 Cross-chain Technology](#73-cross-chain-technology)
        - [7.3.1 Named Router](#731-named-router)
        - [7.3.2 Intelligent Hardware](#732-intelligent-hardware)
        - [7.3.3 Intelligent Assets](#733-intelligent-assets)
        - [7.3.4 Intelligent Wallet](#734-intelligent-wallet)
- [8. Architecture Advantage](#8-architecture-advantage)
    - [8.1 Ownership Clarity](#81-ownership-clarity)
    - [8.2 High Security](#82-high-security)
    - [8.3 Instant Response](#83-instant-response)
    - [8.4 Optimal Experience](#84-optimal-experience)
    - [8.5 Development Friendly](#85-development-friendly)
- [9. Business and Application](#9-business-and-application)
    - [9.1 Business goal: "0" cost of blockchain deployment](#91-business-goal-0-cost-of-blockchain-deployment)
    - [9.2 Application Prospect](#92-application-prospect)
        - [9.2.1 Intellectual Property Protection(IPR)](#921-intellectual-property-protectionipr)
        - [9.2.2 Big Data Management](#922-big-data-management)
        - [9.2.3 Internet of Things](#923-internet-of-things)
        - [9.2.4 Healthcare](#924-healthcare)
        - [9.2.5 Government Administration](#925-government-administration)
        - [9.2.6 Financial Insurance](#926-financial-insurance)
        - [9.2.7 Enterprise Management](#927-enterprise-management)
- [10. Technology Incubation](#10-technology-incubation)
    - [10.1 Incubation Mode](#101-incubation-mode)
    - [10.2 Typical Cases](#102-typical-cases)
        - [10.2.3 Art Management System](#1023-art-management-system)
- [11. Roadmap](#11-roadmap)
    - [11.1 Phase One](#111-phase-one)
    - [11.2 Phase Two](#112-phase-two)
    - [11.3 Phase Three](#113-phase-three)
    - [11.4 Community Autonomy](#114-community-autonomy)
- [References](#references)

<!-- /TOC -->

## 1. Abstract
DDN – with the full name of “Data Delivery Network” – is a new generation of data distribution network. As an enterprise blockchain application platform, DDN aims to make outstanding enterprises even more outstanding. Consisting of multiple public blockchains, consortium blockchains and blockchains for special purpose, DDN network along with the open, transparent and immutable feature of blockchain can effectively protect users’ data assets and are advantageous in data storage and verification, process optimization, intelligent control, financial settlement, etc. With its exclusive network addressing protocol, data distribution protocol and intelligent hardware, DDN can redirect the user's request to the optimal node instantly in processes like network addressing, load balancing and data distribution, to faster data transmission speed and provide with better experience. DDN uses modular develop design, visual operation custom and multiple P2P network compensation structure to make development and application process easier. In this whitepaper, we described the concept and origin of DDN, analyzed the problems facing the Internet currently and provided with detailed solutions. Meanwhile, we listed the development roadmap from the perspective of business.

## 2. Terminology
**Data Delivery Network** (DDN) is a data distribution network, as an underlying network, it can make full use of DDN blockchain technology to do storage, indexing, searching, addressing and distribution work. DDN can overcome the limit of TCP/IP, optimize data transmission to provide a better way of data storage and ensure data value; it can also help enterprise optimize related process, get improved and reach a high degree of autonomy, and finally expand their brand and market influence.

**DDN Blockchain** is an independent third party blockchain program which is different from traditional digital currencies like Bitcoin and Ethereum. It is equipped with cross-chain and sidechain technology; multi-chain parallelism is another hit function. With exclusive modular design and visual operation, DDN will help enterprises to customize their blockchain products instantly.

**Directional Data** (DD) is the data transmitted in DDN network, including all forms exist in traditional networks, like numbers, texts, photos, audios and videos. It differs from traditional network in that these data can store and verify through blockchain, from the time they are created, they do not have the problem of ownership. Every time as they transfer, they will be recorded and you can track the whole transferring history.

**Data Transaction** (DT) means, every time the data moves in DDN network, they belong to a transaction activity. We think in digital world, each change or transfer in digital form should be presented with value or value transferring. Thus DDN is a value network, each data transaction should charge with fees.

**Data Addressing Protocol** (DAP) based on blockchain DNS protocol, avoiding traditional Internet addressing methods to locate data origins rapidly and provide with optimized access nodes.

**Data Storage Protocol**（DSP）is a data storage method based on P2P network used to synchronize users data between personal devices and network distribution. It can assure the security and convenience of data storage, also faster the process of data extraction.

**Data Self Storage** (DSS) makes full use of users’ personal storage devices and put users’ data information on computers, hardware or remote servers controlled by users through DSP. It provides with the first layer of security guarantee for DDN data storage and verification.

**Data Blockchain Storage** (DBS) Hash calculates the valuable information stored by users. On the premise of user permission, it stores on DDN blockchain and allow data storage and verification. It provides with the second layer of security guarantee for DDN data storage and verification.

**Data Delivery Protocol** (DDP) is different from distribution methods based on centralized servers like CDN. DDN based on P2P network, is capable of P2P distribution. It will ensure access speed and prevent data from being disclosed. Thus, it is more secure and it provides with the third layer of security guarantee for DDN data storage and verification.

The word **“Organization”** in the whitepaper means a social entity created with certain goals, tasks and forms. Organizations have well-designed structures and conscious coordinated activity system. It is not only a social cell or basic unit of the society, it’s also so the foundation of the society, such as enterprises, scientific research institutions, social organizations and political parties.

## 3. Goals
DDN aims to make outstanding enterprises even more outstanding.

## 4. Background
DDN is the foundation of the Internet value.

### 4.1 The Origin Intention of Internet is Resources Connection

Tim Berners-Lee, the inventor of the World Wide Web, is also known as “the father of World Wide Web”. He has repeatedly stressed that, WWW is a tool for creativity and efficiency to provide users with better communication environment for work as well as information access. Straightly speaking, it is a network which will connect resources with the nature of open and decentralization.

However, as WWW commercializes, based on commercial purposes, many products are in vicious competition and block certain technologies, which has led to resource monopoly. With the born of industrial giants, the centralized trend is more and more serious, which disobey Lee's intention. DDN is here to solve these problems, with the vision of connecting anything in the world.

### 4.2 User Data Belongs to Users Themselves
There is one fundamental problem that needs to be solved at this stage. That is, once users’ data enter the Internet, they don’t belong to users anymore, but a source of making wealth for data monopolists. Users’ data, especially data created by users are valuable. But it’s difficult to clarify, authorize and protect the ownership of data from Internet, ehich makes it harder to protect users’ interests.

The contents, novels, scripts written by users, the photos and films made by users all have values. Once the above contents are uploaded to the Internet, they are easy to be used without paying the originators or without the permission of the originators, or even some people will use these contents which belongs to others to make profits due to the difficulty of storage, verification and rights protection. As a result, users’ interests will be greatly damaged.

Meanwhile, when users make requests and ask for data usage, they’ll have to pay a great amount of money to the data monopolists, even if the data they ask to use belong to users themselves. Also, in some cases, to use or to transfer data will cost you a lot, thus data sharing process will be less efficient.

DDN blockchain technology will help users (individuals or organizations) to protect data ownership, to make data valuable as they are and to lay foundation of personal wealth. In this way, users’ (individuals or organizations) interest will be protected, finally change status quo.

### 4.3 The Core of Blockchain is the Rule of Interest Transferring

From the technical aspects, blockchain is “a distributed ledger”. Specifically, blockchain is a public accounting system based on P2P network. With the features of open, transparent and immutable, this system is developed by cryptography algorithm. P2P network means decentralization and distribution; cryptography algorithm means each transaction and content will be encrypted through hash calculation, only encrypted data will be disclosed, transaction activities are transparent and once transactions are confirmed, they can’t be tampered; as for public accounting system, it removes intermediary, everyone gets a copy of the ledger, so that it can ensure authenticity and reliability of the data.

In economic terms, blockchain is “a code technology for interests transferring rules”. There are four key words need to be noticed: the first is interests. It is different from values. Values are something inside that can’t be transferred by human wills, but interests can be changed and transferred. Next is transferring. That is, transaction. On blockchain systems, whether P2P payments or data storage, they can all be considered as transactions. The third one is rules, such as all kinds of incentives, which is originated from human nature like interests seeking and economic theories like profit maximization. The last one is code technology. Blockchain is a kind of technology without political complexion, it is neither good nor bad. What it achieves and what ways it takes are all decided by the developers and their codes.

DDN has its own rules, for example, DDN intelligent disk will get rewards according to the space users used to store files, pictures and videos; the bandwidth contributed by users when they access to the Internet will also help them get paid.

Some rules can be set with a specific business scenario, for instance: products of Ebookchain will reward users for writing articles, users can also set a price for their works; community chain will cut promotion and operation cost, users who help with project promotion can be rewarded; Lims system will make governments work more efficient, so that enterprises in charge of detection will not be restricted by enterprises that are under detection.

### 4.4 The Ultimate Status of Enterprise is High Degree of Autonomy

DDN firmly believes that in future world, organizations based on blockchain will achieve a high degree of autonomy. For enterprises, DDN will help them to become “decentralized, de-organized and de-managed”, finally to achieve autonomous. For individuals, DDN will help them to realize “organized, capitalized and value based” goals, to create a small hub.

**Decentralized**: it means centralization in a decentralized way; it means the centralized decision-making process is the core of the organization, but the people involved in organizational decision-making process are always decentralized. Decentralization has nothing to do with politics. It is a distributed form of decision-making, thinking and working patterns. Different ideas will thus make the best of the other worlds. When different sources collide with each other, centralization is a burden. Therefore, decentralization is the inevitable choice to optimize an organization.

**De-organized**: it means de-organized organization. The core of an organization is system, i.e. the rules of control. However, in real world, people are inherently uncertain, so the implementation of the system is often inadequate, or even goes against the original intentions. Blockchain can be understood as the system's faithful executor without any emotion, and will not change directions at will, so as to eliminate any human factors. Thus, a blockchainized organization will be a de-organized organization.

**De-managed**: the management methods of a highly autonomous organization (de-organized organization) are way better than other forms of organizations. It will achieve more efficient management and realize certain goals according to the rules. Different needs can be easily realized through different autonomous organizations, for example: if management work like human resources, accounting and technology development can be done by special autonomous organizations, then its management ways will be more open. A centralized management model that requires a lot of manpower would not exist.

Individuals to achieve “**organized, capitalized and value based**” goals: when the forms of organizations are weakened and the efficiency is greatly improved, the way for individuals to achieve certain goals will become simple and straightforward. In the future, with a single Dapp, one can easily manage people, assets and belongings as organizations do, one can easily finish works that need a lot of people to coordinate,  that is the beginning of personal organization. When individual organizations become prominent and realize value and wealth aggregation, individuals also become an asset to realize capitalization, and personal value will be maximized and based on value.

## 5. Significance

DDN believes that “blockchain is the future of Internet, blockchain is future Internet”. With the mission of “making outstanding enterprises even more outstanding”, DDN will use our own tech to help prominent enterprises build Internet applications and management systems based on blockchain. We will facilitate autonomous organization and achieve the following goals.

### 5.1 To Solve Enterprise (or Industrial) Pain Points

With the born features of “secure, open and immutable”, blockchain can solve four challenges facing traditional Internet: data can easily be tampered, and trust is hard to obtain; denial of service attacks is everywhere, security is a big problem; data is easy to steal and hard to protect; resources are monopolized and data is difficult to obtain. As a blockchain application platform for enterprises, DDN can provide a lot of application scenarios, which will help enterprise to solve pain points that they cannot or difficult to or with high cost.

### 5.2 To Improve Enterprise Operating Efficiency

DDN can optimize product process, promote management level, achieve high degrees of autonomy and significantly improve management and operation efficiency. Based on their own business, DDN can help enterprises finish more valuable missions, strengthen their market positions, lower the cost, increase their market competitiveness and help enterprises to grow in a healthy way.

### 5.3 To Expand Market Share

Based on DDN autonomous organization, the service targets of enterprises can also enter system to become one of the members, the relationship between the customers and the company will turn into a sharing, co-building and win-win relationship, business or service will become their common tasks. Especially, enterprises with a more open and inclusive attitude will make more appealing incentive mechanisms for users (clients) to turn the service objects into the enterprise's own salesmen and evangelists, and constantly expand the coverage of their products (or service).

### 5.4 To Expand Brand Influence

DDN will help enterprises build autonomous organization, the enterprise and employees, enterprise and customer, enterprise management and product operation will be highly unified, thus to make the company management and service more thoroughly, make the company brand more influenced. In turn, it helps industry leading enterprises to further consolidate their leadership, exert their industrial influence and charisma, and generate demonstration effect in the society, which greatly improves the brand value of the company.

## 6. Basic Architecture

### 6.1 Architecture diagram

DDN network is composed of blockchain node servers. The entire network is run in parallel by multiple blockchains，and each blockchain consists of more than 101 node servers, so the number of node servers in the network is much larger than N*101(N is the number of blockchains). These node servers come with load balancing capabilities. Users provide IP and URL for requesting data, each node will play the role of equalizer and, and finally, the URL content requested by the users will be returned to the users. The basic architecture is as follow:

 

### 6.2 Key Technology
**Data storage**: Blockchain technology, construct a strong secure P2P network by DPOS consensus algorithm; storage important content based on the P2P network, such as texts, images, audio and video, and use distributed protocols to allow users to browse the content.

**Data routing**: Network load balancing technology, comprehensively schedule and assign user requests to nearby networks based on their own load, and then find the optimal node for the user.

**Data exchange**:  According to the features of the data, directly do named retrieval to the blockchain, and get the corresponding content quickly.

**Performance management**: server node self-diagnosis, self-management, real-time monitoring of network changes, kicking out of the downtime node, then to ensure the overall performance of the network and the best state of operation.

### 6.3 Main features

#### 6.3.1 Multi-chain parallelism

DDN completely structures on the P2P network, consists of a number of independent blockchain products, public blockchain, alliance blockchain, private blockchain for parallel running; meanwhile, each independent chain adopts a double-layer structure of blockchain and distributed storage to form a complex and orderly underlying network. 

#### 6.3.2 Modular Design

In technical research and development, DDN will further refine the core functions and split them into independent NPM packages, making collaborative development and use more efficient. General business modules such as user management module, authorization management module, process operation module, smart contract customization module and so on will be independent engineering, which is convenient to maintenance and integration. At the same time, DDN will use more development languages to extend the core P2P network.

#### 6.3.3 Visual Customization

The number of DDN nodes is too large, so to ensure the security and efficiency of the entire network, the visual deployment and management will be pursued to the utmost. For different business scenarios, provide visual combinatorial operations. Users can easily combine into a complete DDN blockchain product combined with their own needs.

#### 6.3.4 Multi-terminal Use

DDN wallets, browsers, asset exchanges and other products will provide a wide range of online products, such as PC, mobile and web, make users easy to use.

## 7.Core Technology

### 7.1 DDN Blockchain

#### 7.1.1 Consensus Mechanism
DDN blockchain is based on delegated proof-of-stake(DPOS)consensus. DPOS use the trustees to create blocks. Trustees are trusted accounts elected by the community, which ranked in the top 101 of the number of votes. Other trustee accounts that did not make it to the top 101 would be listed as candidates. To become a full trustee, users must go to the community to build credibility and gain the trust from enough users. Users can use the percentage of the number of DDN held by themselves to vote. When the 101 block generation cycle is complete, the top 101 delegates will be readjusted and those who fall in rank would be downgraded to candidates. The 101 blocks of each cycle are represented by 101 randomly generated blocks, each block's interval time is 10 seconds, the newly created block is broadcast to the network, and added to the blockchain, after getting 6-10 confirmations, the transaction will be confirmed, a complete 101 block cycle takes about 16 minutes.

#### 7.1.2 Reward Mechanism
DDN network consists of numerous public chains, alliance chains and private chains. The token name of core public chain is DDN, which is issued and managed by DDN Foundation. DDN Foundation is also responsible for cross-chain operations and commercial pledge of other chains. DDN's total supply is 100 million, and the block reward will reduce 1 DDN by every 340 days (about 1year), the 1st year is 5 DDN/block, the 2nd year is 4 DDN/block, and so on, until the 5th year down to the 1DDN/ block, and then maintain the amount of this award will not change. Various operations based on the public chain need to pay a certain amount of fees, such as: transfer, vote and so on need to pay 0.1 DDN, the application trustee needs to pay 100 DDN and so on, the service charge will be distributed to each node.

Other blockchains based on the DDN blockchain will be managed by joint ventures, DDN only provides technical support, does not participate in operations management, does not participate in investment, do not do any form of endorsement. According to the needs of cooperative enterprises, the specific data will be different. For example, the number of nodes, the total supply of token, the number and methods of rewards, the type of transaction and the transaction cost, etc., all can be flexibly customized. Once configured and the main network run, those will never be changed. In principle, it is recommended that enterprises maintain 101 or more nodes, at least maintain 21 nodes running. Therefore, DDN network have more than N*101 nodes.

#### 7.1.3 Trustees
To become a trustee, users need to register the trustee account, they can register through any version of the client, and use the full node program to open the function of forging blocks. All the DDN accounts can be registered as trustees. The new trustees all start with candidates. The initial vote rate of candidates is 0, candidates must gain community support to get enough votes to make himself a trustee in the top 101. To register as a trustee, users should pay a certain network fee.

#### 7.1.4 Peer-to-peer (P2P) networks
DDN uses a standard peer-to-peer(P2P) network built on HTTP protocol. It uses JSON to communicate data and the P2P module contains node data such as system version, IP, port number and so on.

### 7.2 Sidechain Technology
DDN blockchain has powerful, easy to use, programmable sidechain, it can provide simple and fast extension services for third party developers and develop and design personalized Dapps. Its main features are:

#### 7.2.1 Virtual Machine
The DDN blockchain adopts sandbox mechanism, running unauthenticated javascript code through a virtual machine. The virtual machine is a branch of node.js, and connect with DDN main blockchain through API. 

Dapp run in a virtual machine, uses the DDN algorithm as its consensus algorithm, this mechanism can prevent many possible attacks, and make users run Dapp more safely on the machine. Users can run Dapps on the client.


#### 7.2.2 Dapp development
DDN blockchain virtual machine API is easy to use, developers can choose any NPM library, use all the asynchronous programming capabilities of java script, build any application code based on DDN.

#### 7.2.3 Dapp Operation
DDN implements a time-dependent system, DDN virtual machines can track the CPU time used to run a Dapp, therefore, node owner can earn DDN as income. DDN encourages node owners to provide CPU calculation, internal storage, memory and other resources to earn more reward, promote DDN network cover more widely, more strongly, more safely.

#### 7.2.4 Dapp Consensus Algorithm
The Dapp owner can track how his Dapp is used. The transactions within the Dapp are handled by the master node, which is the owner of the Dapp owner who must have a DDN account, which is similar to a multi-signed account, its main task is to create consensus and sign new blocks on the Dapp master node. Once a new Dapp block is created and signed within the primary node, the block needs to be converted to a SHA266 hash. The Dapp owner then submits the hash to DDN blockchain, DDN stores the hash as a Dapp block. Once the DDN blockchain receives a transaction containing the Dapp hash, the trustee compares the hash with the previous hash and saves it.

#### 7.2.5 Dapp Master Node
Dapp master node is a DDN node, which installed with the Dapp and opened block creation function for the Dapp, only the owner of a multi-signed Dapp account can run the master node by using the key, the master node is the core of the Dapp system. The master node processes transactions and creates new blocks. Then the DDN blockchain or the bitcoin blockchain ensures its security.

### 7.3 Cross-chain Technology
The sidechain is an extension of a single chain and an application anchored on a main chain. The main chain disappears and the sidechain will no longer exist. In the face of different business scenarios, the DDN blockchain can quickly generate new main chains, and many main chains run in parallel, there is no difference between those sidechains, and there is no influence on each other. The disappearance of one chain will not affect the existence of another chain. Nor will the data be affected.

To realize the exchange of multiple chains, DDN network will introduce the cross-chain technology to further extend the blockchain. The basic principles are shown in the figure:
 

#### 7.3.1 Named Router
DDN consists of multiple DDN blockchains, named routers are effective for the entire network. Distributed networks, intelligent addressing, capitalization and so on are the basic components of DDN networks. Named routers can effectively connect these networks, simplify user operations, and improve indexing efficiency and retrieval speed. Named routers can effectively unify user assets, blockchains, data and resource URL, and achieve a perfect browsing experience based on node load balancing and intelligent addressing.

#### 7.3.2 Intelligent Hardware
User has diverse needs for personal data storage, so in order to meet more personalized needs of users, DDN will further improve the distributed storage algorithm, improve the usage experience of distributed network, and further optimize the file storage protocol, improve storage efficiency and security; introduce data mining machine, intelligent network disk and other hardware devices to improve the security of personal security; through hardware compensation, increase more network nodes, enhance the efficiency of DDN network addressing.

#### 7.3.3 Intelligent Assets
Data capitalization will be the norm of future organizations, DDN will fully support the digitalization of real assets, such as physical property, personal value, securities, corporate equity, and capitalization of value data, such as personal contribution, enterprise income and so on, so as to help enterprises to manage and upgrade simply and conveniently.


#### 7.3.4 Intelligent Wallet
Assets should have circulation, in addition to helping users manage personal assets conveniently, DDN wallet should also provide the function of asset transfer, sale and exchange, so that assets can really flow. Intelligent wallet should be simple and easy to use, but also safe and reliable.

## 8. Architecture Advantage

### 8.1 Ownership Clarity
The premise of the transaction is that the ownership of the data is clear. Therefore, whether from the legal level, or the technical level, firstly, the ownership must be clear. Especially in the scope of the Internet, the law must have technical support, you can do nothing unless it is technically operational. Now, we can't guarantee that our data will still belong to us when it is posted online, so we must first technically make sure that we have the ownership. DDN can easily achieve data confirmation, authorization, and protection of rights. Therefore, the use of DDN can not only achieve "data has ownership", but also can achieve "data has value."

### 8.2 High Security
The way that DDN processes personal ID card is "three-layer protection". The first layer is to allow the user to save all the data himself, and allow the user to use intelligent net disk to synchronize their data directly through the DSP; The second layer is the DDN blockchain certificate data, endow the data with ownership, allow users to have their own digital assets forever; The third layer is point-to-point transmission, which allows users to browse strictly encrypted data information through DAP and DDP.

### 8.3 Instant Response
Cache-free DDN network is an instant application, it rarely uses cache, and its content is always up-to-date. Only when the user exits, the optimal resource list or content will be cached, it is convenient for next use. In addition, DDN can be oriented to all kinds of data produced by individual users, and large websites built by enterprise users, if it involves all kinds of transactions and authorized operations, it can interact with the DDN network.

### 8.4 Optimal Experience
DDN has the characteristics of instant, fast, efficient and simple. Users can easily build their own decentralization website, blog, e-commerce website and other platforms based on DDN. With the same usage and experience, the cost is almost zero. As the coverage of DDN becomes wider and wider, more and more nodes will be deployed, and the performance of dap and DDP will become better and better, and the user experience of using the network will be better. Therefore, the whole DDN system is the best practice of a gain compensation system.

### 8.5 Development Friendly
The core features of DDN will be further refined to make collaborative development more efficient. Each module is set up as an independent project. Through modularization function, it is convenient to maintain and integrate. DDN will support more development languages to extend the core P2P network. At the same time, it provides visual combination operation, easily combine complete blockchain products, and make development friendlier.

## 9. Business and Application

### 9.1 Business goal: "0" cost of blockchain deployment
The goal of DDN is to build the next-generation value Internet from the bottom of the Internet, so DDN has been working from the start to reduce the deployment of blockchains and use-cost. And the simplification of DDN single chain deployment, the exchanges between chains, and the expansion capability of the sidechains, laid a good foundation for the rapid expansion of business.

DDN can provide solutions for massive application scenarios. At present, DDN has signed with Ebookchain, Limschain, Artwork Management System and other product partners. It has been comprehensively deployed in the entertainment industry, such as text, film and television, artwork, etc., and has been launched in the fields of Internet of Things, health care, finance, supply chain and so on. The large-scale ecosystem has begun to take shape.
 
### 9.2 Application Prospect

#### 9.2.1 Intellectual Property Protection(IPR)

Copyright protection for digital media and assets such as texts, pictures, videos, software works has been a worldwide challenge. Hard to confirm the right, piracy flooding, difficult to obtain evidence and many other problems are besetting the industry. The advantages of "blockchains" are transparency, tamper-proof, irreversibility, etc. DDN has uniquely created copyright agreement and copyright history record. It can provide creators, publishing organizations and so on with "one-click registration" quick right confirmation service, "Intellectual Retrieval" copyright evidence services, insurance claims and other copyright litigation services.

#### 9.2.2 Big Data Management
DDN is a distributed ledger and is a natural big data management platform. In the current world, all artificial intelligence, innovation, and value are all from data and information. Where data and information are, values and innovations are born. DDN is the next generation Internet that will reconstruct big data and become the portal for all future data. DDN collects, collates and analyses big data, provides convenience, lowers cost, and improves efficiency.

#### 9.2.3 Internet of Things
DDN is a platform with best value interconnection and process control. When it is applied to the Internet of Things, it will open infinite possibilities. DDN can be used to track the history of the use of devices, coordinate the processing of transactions between devices, and even be like neural networks. Its running state is based on the DDN smart contract control equipment, and then evolves into intelligentized network. DDN adapt to the large-scale Internet of Things, control and manage many physical equipment, develop a powerful equipment management system for all kinds of production enterprises, provide a complete solution for photovoltaic power generation and other accurate poverty reduction projects.

#### 9.2.4 Healthcare
DDN can realize the distributed electronic medical record management system, which can be preserved permanently and cannot be tampered with. Based on protecting privacy, we can achieve cross-agency, cross-regional access to medical information, and comprehensive medical information tracking, improvement of medical quality, decrease of medical costs, improvement of patients' convenience to seek medical treatment, improvement of doctor-patient relationship, and raising the level of medical scientific research. DDN network can also be used in government supervision, clinical trials, drug circulation, health big data mining and other medical applications.

#### 9.2.5 Government Administration
The blockchain is distributed and decentralized, which can effectively solve the problems of corruption in centralized management, and even can manage things that you can't manage through human resources, thus expand the strength of government control. DDN can provide identity authentication, data storage, anti-counterfeiting and traceability, privacy protection and other functions, and realize the tax supervision system, truly record and master the tax situation of each taxpaying object; and realize the personal identity authentication system shared by the whole people, truly record citizenship information and share among departments and enterprises, reduce costs, improve efficiency, enhance mutual trust, and so on, can achieve accurate poverty alleviation.

#### 9.2.6 Financial Insurance
Blockchain is an inherent settlement system. DDN can provide blockchain digital bill service for commercial banks, enterprises, large commercial organizations and so on. It can give play to the blockchain's advantages of not tampering, traceability and real time clearing in bill business, reduce the risk of errors in bill clearing and trust cost, track the flow of funds, and strengthen financial regulation.

#### 9.2.7 Enterprise Management
Blockchain data cannot be tampered with and is traceability, it has unparalleled advantages in the enterprise supply chain management, human resources management, financial management and other aspects, DDN can customize its own enterprise data link for large, medium and small enterprises, and achieve cross-chain data interaction between different enterprises and across industries in the same industry, so that the enterprise management more efficient, lower cost.

## 10. Technology Incubation

### 10.1 Incubation Mode
DDN will adopt the model of technology incubation to further accelerate the global layout. Any entity that needs blockchain applications can get technical support and services from DDN if it has high quality resources.

### 10.2 Typical Cases
Ebookchain is the most typical application of DDN network. Its mission is to "enrich the people with knowledge" and the goal is to strengthen the personal data depository, and on the basis of the protection of personal privacy, allow users to freely combine knowledge, creativity and data, distribute them freely and realize them directly, realize "write and sell"; Based on the entertainment industry, to achieve the aggregation of knowledge creation, knowledge payment, digital publishing and other economic ecology.

LimsChain is an information platform based on DDN and based on information management of third-party testing laboratory.

LimsChain dedicated to provide systematic solution for sampling, inspection, report, quality control, the management of whole process, improve the efficiency of the testing organization, reduce the operating costs, so that the inspection process and data of the inspection organization can achieve fairness, justice, trust, traceability.

#### 10.2.3 Art Management System
Art Management and Trading System is an integrated information management platform based on DDN, it can achieve security, traceability and transaction of art works. Through the DDN network, the system stores, collates and distributes the information of the works created by artists, and uses original chemical or physical anti-counterfeiting technology to track and prevent counterfeiting, thus ensures the authenticity and security of online transactions, improves the number and frequency of transactions, lay a good foundation for the collection, management and circulation of art works.


## 11. Roadmap

### 11.1 Phase One 
Keep upgrading the codes of DDN to better its performance and stability. 

### 11.2 Phase Two

Upgrade the core chain of DDN to connect with other chains so as to build a worldwide distributed data network. 

### 11.3 Phase Three
To design all forms of DDN-based business models and make them available to people worldwide. To realize the three “de-s” goals of decentralization, deorganization and demanagement. 

### 11.4 Community Autonomy 

The global community of DDN will perform the ideals of three “de-s” by looking for developers, operation, managers and translators from all over the world to develop the DDN-based BBSchain following the official Green paper of DDN community management.

Divided by functions, the DDN global community such four sectors as node management, technical development, operation management and marketing. As is shown in the diagram:

## References

* [The Ebookchain whitepaper](http://www.ebookchain.org/ebookchain.pdf)
* [Tim Berners-Lee](https://baike.baidu.com/item/蒂姆·伯纳斯·李/8868412?fr=aladdin)
* [The world’s first website](http://info.cern.ch)
* [The birth of the web](https://home.cern/topics/birth-web)
* [The official website of NPM](https://www.npmjs.com/)
* [Bitcoin whitepaper](https://bitcoin.org/bitcoin.pdf)
* [Bitshares DPoS](http://wiki.bitshares.org/index.php/BitShares)
* [The concept of organization](https://baike.baidu.com/item/组织/10200?fr=aladdin)

