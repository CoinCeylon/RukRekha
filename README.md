# RukRekha 🌳  – Immutable Tree Planting Verification on Cardano

**RukRekha** (*රුක් රේඛා*, meaning "Tree Line" or "Tree Record" in Sinhala) is a decentralized application (dApp) designed to transparently verify tree planting efforts using the Cardano blockchain. It leverages smart contracts, simulated IoT data, and NFT technology to ensure every planted tree leaves a permanent digital mark.

---

## ✨ Key Features

- ✅ **Blockchain-verified tree planting logs**
- 🔐 **Smart contract validator using Aiken** (authorized wallet-only submissions)
- 📡 **Simulated IoT integration** for environmental data (e.g., soil moisture, temp)
- 🏅 **NFT eco-badge minting** for donors and contributors
- 📊 **Public dashboard** to view and verify tree planting activity

---

## 🚀 Live Demo (Testnet)

> Coming soon — hosted on GitHub Pages or Cardano testnet

---

## 🧩 Tech Stack

| Layer | Tools |
|-------|-------|
| Frontend | HTML, CSS, Bootstrap, JavaScript |
| Blockchain | [Cardano Testnet](https://testnet.cardano.org), [Mesh SDK](https://meshjs.dev), [Blockfrost API](https://blockfrost.io) |
| Smart Contracts | [Aiken](https://aiken-lang.org) (Plutus V2 Validator) |
| NFT | On-chain assets minted via Mesh SDK |
| IoT | Simulated via JavaScript (can connect to ESP32 in future) |

[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/Thyagee/RukRekha/blob/main/LICENSE)

---


https://youtu.be/286Io5gN35w


RukRekha: Decentralized Tree Adoption & Carbon Offset Tracking
📜 Executive Summary
The RukRekha project was envisioned as a groundbreaking platform designed to enhance transparency, engagement, and accountability in tree planting and carbon offset initiatives. Our idea was to harness the power of blockchain technology, non-fungible tokens (NFTs), QR-based verification, and community-driven participation to create a robust, traceable, and user-friendly solution for both individuals and organizations. Although development was constrained by environmental setup issues, our team successfully implemented the foundational components, signup, login, wallet connection, and basic user interface designs. This document details the initial concept, intended features, technical design, processes, limitations identified, and proposed future enhancements, demonstrating the thought and planning invested in the idea.
🎯 Project Vision & Objectives
Vision
To establish a decentralized, transparent, and verifiable ecosystem for tree adoption and carbon offsetting, enabling stakeholders to contribute meaningfully to environmental sustainability while confidently tracking the impact of their efforts.
Objectives
● Foster trust by recording immutable planting data on a public blockchain.
● Incentivize engagement through NFT-based digital identity and recognition.
● Provide accessible verification tools using smartphones and QR codes.
● Support community oversight with transparent dashboards and feedback mechanisms.
● Ensure scalability, affordability, and ease-of-use for widespread adoption.
🌟 Planned Feature Set
1️
⃣ Blockchain-Based Data Submission
● Organizations record tree planting details (location, species, date, planter info) via web forms.
● Submitted data is hashed and permanently stored on the Cardano blockchain using Mesh SDK and Blockfrost API.
● Ensures data integrity and publicly auditable records.
2️
⃣ NFT Tree Adoption & Digital Identity
● Donors adopt trees by funding planting efforts.
● Upon adoption, an NFT is minted via an Aiken smart contract, containing:
○ Donor name
○ GPS location of the tree
○ Tree species
○ Planting date
● NFTs are stored securely in the donor’s Cardano-compatible wallet (e.g., Eternl), serving as proof of contribution and a digital badge.
3️
⃣ Camera-Based Growth Verification
● Planters submit periodic growth verification photos through a web form.
● Photos are automatically timestamped and geotagged, with metadata stored securely on Firebase cloud storage.
● Photos create a growth timeline, enhancing transparency and engagement.
4️
⃣ QR Code Tagging & Public Dashboard
● Unique QR codes are generated for each planted tree.
● QR codes are printed (weatherproof) and physically attached to trees.
● When scanned by any smartphone, the QR links to a public dashboard page displaying:
○ Full planting history
○ NFT metadata and donor details
○ Photo timeline showing growth
○ Verification of carbon-offset claims
🔑 Quick Implementation Recommendations
● Use free or low-cost tools like Firebase’s free tier and open-source QR code generators.
● Employ simple web technologies and standard smartphone capabilities to minimize barriers to use.
● Design user-friendly interfaces with clear instructions for non-technical users.
👥 Stakeholders & Actors
Actor
Role & Responsibilities
🌿 Organization/Planter
Plants trees, submits planting and growth data, attaches QR codes.
💳 Donor/User (Adopter)
Funds tree planting, receives NFT, monitors progress via dashboard.
📸 Verifier/Public
Scans QR codes, verifies claims, submits feedback/photos.
🧰 System Admin
Maintains platform, manages blockchain backend, resolves disputes.
🔄 Planned Processes
🌱 Planter Workflow
1. Sign up and log in to the platform.
2. Submit planting activity data (species, quantity, date, GPS location) with an initial photo.
3. Data is recorded on blockchain; QR code is generated and printed.
4. Attach QR code to tree; upload periodic photos for growth verification.
🌲 Donor Workflow
1. Browse available planting opportunities.
2. Adopt trees and fund planting efforts through wallet transaction.
3. Receive NFT as proof of adoption.
4. Monitor tree status and history via dashboard or by scanning QR code.
🔍 Verifier/Public Workflow
1. Scan QR code attached to tree using any smartphone.
2. View full planting history, photos, and donor information.
3. Submit feedback or additional verification photos if necessary.
⚙️
System Admin Workflow
1. Set up and maintain blockchain smart contracts, Firebase, and QR generation tools.
2. Monitor system performance and resolve technical or user issues.
3. Audit data for transparency and generate reports for stakeholders.
4. Manage dispute resolution in case of data disputes or fraud.
📑 Why This Approach Was Designed
● ✅ Low Cost & Feasibility: Relied on free/low-cost cloud services and open-source tools.
● ✅ Scalable & Transparent: Blockchain ensures data cannot be tampered with.
● ✅ User-Friendly: QR codes and clear dashboards make it easy for anyone to verify.
● ✅ Engaging & Motivating: NFTs serve as digital certificates and foster donor loyalty.
🚧 Current Status & Achievements
Despite environmental and setup challenges, the team completed:
● User signup and login functionalities.
● Wallet connection integration with Eternl.
● Initial user interface designs for the main workflows.
We were unable to implement the full feature set within the project timeframe, but this document reflects our original scope and technical ambition.
🔍 Identified Limitations & Future Enhancements
From the outset, we analyzed potential challenges and devised mitigation strategies, detailed in our planning documents:
Key Challenges
● NFT spamming & excessive costs
● Fake or incorrect data submissions
● Identity fraud and wallet abuse
● QR tag loss or damage
● Blockchain scalability and transaction fees
● Privacy and data security concerns
● Poor user onboarding or UI complexity
● Downtime of blockchain APIs
● Automated bot abuse
● Disputes over data authenticity
Proposed Enhancements
● Wallet-based rate limiting to prevent spam.
● Community-based moderation and AI-assisted photo verification.
● KYC or reputation systems to discourage fraud.
● Use of durable NFC tags alongside QR codes.
● Hybrid on/off-chain storage for scalability.
● Batch NFT minting and fee optimization.
● Clear, user-friendly UI with tutorials.
● API failover mechanisms and local data buffering.
● CAPTCHA and rate limiting to prevent bot abuse.
● Transparent dispute resolution policies and audit trails.
🌱 Conclusion & Next Steps
The RukRekha project represents a novel and realistic approach to solving challenges in tree planting verification and engagement. Our team demonstrated foresight, thorough planning, and technical creativity in conceptualizing the platform. Although we were unable to fully implement it, the groundwork we laid and the challenges we identified will provide a strong foundation for any future development or collaboration.
We welcome any opportunity to present our progress, share insights, and collaborate further to bring this impactful idea to full realization.
Prepared by the CodeGenesis Team
2025.07.07
## 📂 Folder Structure