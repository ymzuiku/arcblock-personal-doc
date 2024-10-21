# What is Blocklet Server?

## What is a Blocklet?

A Blocklet is what we call an application in our company. It can theoretically be any kind of application, though most are currently built with Node.js. These applications run on the Blocklet Server platform.

To make it easier to understand, think of some of our company’s products: Pages-Kit and AIGNE are both Blocklets. Essentially, all our products, except for Blocklet Server and DID, are Blocklets.

Blocklet Server is the platform where Blocklets run. It manages the lifecycle of each Blocklet and ensures they function properly.

## Basic Architecture of Blocklet Server

Blocklet Server is built with Node.js, and many of our Blocklets are also developed using Node.js.

Inside Blocklet Server, there are two main components:

Blocklet Server: The core platform.
Blocklet Service: A layer that provides Blocklets with essential features like login, data storage, and message notifications.

Here is a simple architecture diagram (we don't need to go into details right now):

https://team.arcblock.io/comment/docs/c158aee4-accd-42f4-9ced-6a23f28c00e0/en/L0P8cWeYx15c1GB_4Tnk_TFv#a6045171-3e58-4717-84bf-2d08a2684a58

## The user structure of blocklet server.

A complete Blocklet Server has three types of users:

- **Platform Provider**: The one who runs the Blocklet Server environment and allows others to buy and deploy Blocklets. For example, arcblock.io is a platform provider. Anyone can also set up their own platform using Blocklet Server.
- **Blocklet Owner**: These users buy space on the platform to deploy their own Blocklets (In the future, they will be our company’s main customers).
- **Blocklet User**: These are the customers of the Blocklet Owners. They use the Blocklets. (Sometimes, the Blocklet Owner and User can be the same person. For example, someone might deploy discuss-kit for personal use.)

There is one more special type of user:

Blocklet Developers: These users create their own Blocklets and publish them to the [Blocklet Store](https://store.blocklet.dev/) to make money. Right now, we don’t have many serious outside developers. Most Blocklet developers are still our company’s employees.
