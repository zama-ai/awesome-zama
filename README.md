<p align="center">
  <img src="https://github.com/zama-ai/awesome-zama/assets/157474013/3743d435-dbba-4d89-907a-81957e6a4b1a" width="200px">
  <br><br/>
  A curated list by the team at Zama of blog posts, libraries, research papers, and tutorials on <b>Fully Homomorphic Encryption (FHE)</b>.
</p>


## Table of contents

- [Libraries and solutions](#libraries-and-solutions)
- [Demos](#demos)
- [Tutorials](#tutorials)
   - [TFHE-rs](#tfhe-rs)
   - [Concrete](#concrete)
   - [Concrete ML](#concrete-ml)
   - [fhEVM](#fhevm)
- [Blog posts](#blog-posts)
   - [Product releases](#product-releases)
   - [Announcements](#announcements)
   - [Engineering articles](#engineering-articles)
- [Research papers and publications](#research-papers-and-publications)
- [Talks and posters](#contributed-talks-and-posters)
<br></br>

## Libraries and solutions
Zama's FHE libraries and solutions.

- [TFHE-rs](https://github.com/zama-ai/tfhe-rs): A pure Rust implementation of the TFHE scheme for Boolean and integer arithmetics over encrypted data.
- [Concrete](https://github.com/zama-ai/concrete): TFHE compiler that converts python programs into FHE equivalents.
- [Concrete ML](https://github.com/zama-ai/concrete-ml): Privacy-preserving ML framework built on top of Concrete, with bindings to traditional ML frameworks.
- [fhEVM](https://docs.zama.ai/fhevm): A confidential smart contracts protocol for the EVM using homomorphic encryption.
- [Zama Bounty Program and Grant Program](https://github.com/zama-ai/bounty-program): Contribute to Zama's open source libraries and get rewarded. More than €500,000 available in prizes.
<br></br>

## Demos
Demos by Zama sorted by date

- [Encrypted anonymization using FHE](https://huggingface.co/spaces/zama-fhe/encrypted-anonymization)
- [Encrypted credit card approval prediction using FHE](https://huggingface.co/spaces/zama-fhe/credit_card_approval_prediction)
- [Encrypted sentiment analysis using FHE](https://huggingface.co/spaces/zama-fhe/encrypted_sentiment_analysis)
- [Encrypted health prediction using FHE](https://huggingface.co/spaces/zama-fhe/encrypted_health_prediction)
- [Encrypted image filtering using FHE](https://huggingface.co/spaces/zama-fhe/encrypted_image_filtering)
<br></br>

## Tutorials
Tutorials by the Zama team sorted by date

### TFHE-rs
- [[Video tutorial] Implement GPU acceleration on homomorphic computation using TFHE-rs](www.zama.ai/post/video-tutorial-implement-gpu-acceleration-on-homomorphic-computation-using-tfhe-rs) - May 2024
- [[Video tutorial] Implement signed integers using TFHE-rs](https://www.zama.ai/post/video-tutorial-implement-signed-integers-ssing-tfhe-rs) - November 2023
- [Boolean SHA256 using TFHE-rs](https://www.zama.ai/post/boolean-sha256-tfhe-rs) - July 2023
- [Dark market application using TFHE-rs](https://www.zama.ai/post/dark-market-tfhe-rs) - July 2023
- [Regular expression engine with TFHE-rs](https://www.zama.ai/post/regex-engine-tfhe-rs) - June 2023


### Concrete 
- [[Video tutorial]Compile composable functions with Concrete](https://www.zama.ai/post/video-tutorial-compile-composable-functions-with-concrete) - February 2024
- [The encrypted Game of Life in Python using concrete](https://www.zama.ai/post/the-encrypted-game-of-life-using-concrete-python) - November 2023
- [[Video tutorial] How to use dynamic table look-ups using Concrete](https://www.zama.ai/post/video-tutorial-how-to-use-dynamic-table-look-ups-using-concrete) - November 2023
- [[Video tutorial] Dive into Concrete - Zama's Fully Homomorphic Encryption compiler](https://www.zama.ai/post/video-tutorial-dive-into-concrete-zamas-fully-homomorphic-encryption-compiler) - October 2023
- [[Video tutorial] How to get started with Concrete - Zama's Fully Homomorphic Encryption compiler](https://www.zama.ai/post/how-to-started-with-concrete-zama-fully-homomorphic-encryption-compiler) - July 2023
- [Encrypted key-value database using homomorphic encryption](https://www.zama.ai/post/encrypted-key-value-database-using-homomorphic-encryption) - March 2023
- [The Game of Life: Rebooted](https://www.zama.ai/post/the-game-of-life-rebooted-with-concrete-v0-2) - August 2022
- [Encrypted search using fully homomorphic encryption](https://www.zama.ai/post/encrypted-search-using-fully-homomorphic-encryption) - February 2022

### Concrete ML
- [Running privacy-preserving inferences on Hugging Face endpoints](https://huggingface.co/blog/fhe-endpoints) - April 2024
- [Build an end-to-end encrypted Shazam application using Concrete ML](https://www.zama.ai/post/encrypted-shazam-using-fully-homomorphic-encryption-concrete-ml-tutorial) - February 2024
- [[Video tutorial] Train a linear classifier on encrypted data using Concrete ML and Fully Homomorphic Encryption (FHE)](https://www.zama.ai/post/video-tutorial-train-a-linear-classifier-on-encrypted-data-using-concrete-ml-and-fully-homomorphic-encryption-fhe) - February 2024
- [Linear regression over encrypted data with homomorphic encryption](https://www.zama.ai/post/linear-regression-using-linear-svr-and-concrete-ml-homomorphic-encryption) - June 2023
- [Comparison of Concrete ML regressors](https://www.zama.ai/post/comparison-of-concrete-ml-regressors) - June 2023
- [[Video tutorial]How to convert a scikit-learn model into its homomorphic equivalent](https://www.zama.ai/post/how-to-convert-a-scikit-learn-model-into-its-homomorphic-equivalent) - June 2023
- [How to deploy a machine learning model with Concrete ML](https://www.zama.ai/post/how-to-deploy-machine-learning-models-with-concrete-ml) - May 2023
- [Encrypted image filtering using homomorphic encryption](https://www.zama.ai/post/encrypted-image-filtering-using-homomorphic-encryption) - February 2023
- [Sentiment analysis over encrypted data](https://huggingface.co/blog/sentiment-analysis-fhe) - November 2022
- [Titanic competition with privacy-preserving machine learning](https://www.zama.ai/post/titanic-competition-with-privacy-preserving-machine-learning-using-concrete-ml) - August 2022

### fhEVM
- [[Video tutorial] Using asynchronous decryption in Solidity contracts with fhEVM](https://www.zama.ai/post/video-tutorial-using-asynchronous-decryption-in-solidity-contracts-with-fhevm) - April 2024
- [Build an encrypted wordle game onchain using FHE and Zama's fhEVM](https://www.zama.ai/post/build-an-encrypted-wordle-game-onchain-using-fhe-and-zama-fhevm) - February 2024
- [[Video tutorial] Accelerate your code testing and get code coverage using fhEVM mocks](https://www.zama.ai/post/video-tutorial-accelerate-your-code-testing-and-get-code-coverage-using-fhevm-mocks) - January 2024
- [Programmable privacy and onchain compliance using Homomorphic Encryption](https://www.zama.ai/post/programmable-privacy-and-onchain-compliance-using-homomorphic-encryption) - November 2023
- [[Video tutorial] Use the CMUX operator on Zama’s fhEVM](https://www.zama.ai/post/video-tutorial-use-the-cmux-operator-on-zamas-fhevm) - October 2023
- [Confidential DAO voting using Homomorphic Encryption](https://www.zama.ai/post/confidential-dao-voting-using-homomorphic-encryption)
- [[Video tutorial] How to write confidential smart contracts using Zama's fhEVM](https://www.zama.ai/post/video-tutorial-how-to-write-confidential-smart-contracts-using-zamas-fhevm) - October 2023
- [Onchain blind auctions using FHE](https://www.zama.ai/post/on-chain-blind-auctions-using-homomorphic-encryption) - July 2023
- [Confidential ERC-20 tokens using Homomorphic Encryption and the fhEVM](https://www.zama.ai/post/confidential-erc-20-tokens-using-homomorphic-encryption) - June 2023
- [Private smart contract using FHE](https://www.zama.ai/post/private-smart-contracts-using-homomorphic-encryption) - May 2023
<br></br>

## Blog posts
Zama's blog posts sorted by date
### Product releases
- [Zama Product Releases - January 2024](https://www.zama.ai/post/zama-product-releases-january-2024)
- [Zama Product Releases - October 2023](https://www.zama.ai/post/zama-product-releases-october-2023)
- [Zama Product Releases - July 2023](https://www.zama.ai/post/zama-product-releases-july-2023)
- [Zama Product Releases - April 2023](https://www.zama.ai/post/zama-product-announcement-april-2023)
- [Zama product Releases - January 2023](https://www.zama.ai/post/zama-product-announcement-january-2023)
- [Zama Product Releases - October 2022](https://www.zama.ai/post/zama-product-announcement-october-2022)
- [Zama product Releases - July 2022](https://www.zama.ai/post/zama-product-announcement-july-2022)
- [Zama Product Releases - April 2022](https://www.zama.ai/post/zama-product-announcement-april-2022)

### Announcements
- [The Zama FHE Master Plan](https://www.zama.ai/post/zama-fhe-master-plan) - March 2024
- [Introducing the Zama Grant Program and launching the Zama Bounty Program season 5](https://www.zama.ai/post/introducing-the-zama-grant-program-and-launching-the-zama-bounty-program-season-5) - February 2024
- [Zama Bounty Program Season 3](https://www.zama.ai/post/zama-bounty-program-season-3) - May 2023
- [Zama Bounty Program Season 4: New Bounties Available](https://www.zama.ai/post/launching-the-zama-bounty-program-season-4) -  September 2023
- [Zama Bounty Program Season 2](https://www.zama.ai/post/zama-bounty-program-season-2) - February 2023
- [Launching the Zama Bounty Program with over €500,000 in prizes](https://www.zama.ai/post/launching-the-zama-bounty-program) - November 2022
- [How We Monetize Open Source at Zama](https://www.zama.ai/post/open-source) - August 2022
- [How We Hire at Zama](https://www.zama.ai/post/how-we-hire-at-zama) - October 2021

### Engineering articles
- [Training predictive models on encrypted data using Fully Homomorphic Encryption](https://www.zama.ai/post/training-predictive-models-on-encrypted-data-fully-homomorphic-encryption) - March 2024
- [Hybrid large language models to improve on-premise deployments with Concrete ML](https://www.zama.ai/post/hybrid-large-language-models-to-improve-on-premise-deployments-with-concrete-ml) - October 2023
- [The architecture of Concrete, Zama's Fully Homomorphic Encryption compiler leveraging MLIR](https://www.zama.ai/post/the-architecture-of-concrete-zama-fully-homomorphic-encryption-compiler-leveraging-mlir) - October 2023
- [Concrete - Zama's FHE compiler](https://www.zama.ai/post/zama-concrete-fully-homomorphic-encryption-compiler) - May 2023
- [Making chatGPT encrypted end-to-end](https://www.zama.ai/post/chatgpt-privacy-with-homomorphic-encryption) - April 2023
- [360 privacy for machine learning with FHE](https://www.zama.ai/post/360-privacy-for-machine-learning-with-homomorphic-encryption) - December 2022
- [Bootstrapping for dummies](https://www.zama.ai/post/what-is-bootstrapping-homomorphic-encryption) - November 2022
- [FHE and quantum cryptography](https://www.zama.ai/post/fully-homomorphic-encryption-and-post-quantum-cryptography) - October 2022
- [FHE as a puzzle piece](https://www.zama.ai/post/fhe-as-a-puzzle-piece) - January 2023
- [TFHE deep dive part 4](https://www.zama.ai/post/tfhe-deep-dive-part-4) - June 2022
- [TFHE deep dive part 3](https://www.zama.ai/post/tfhe-deep-dive-part-3) - May 2022
- [TFHE deep dive part 2](https://www.zama.ai/post/tfhe-deep-dive-part-2) - May 2022
- [TFHE deep dive part 1](https://www.zama.ai/post/tfhe-deep-dive-part-1) - May 2022
- [Estimating the security of homomorphic encryption schemes](https://www.zama.ai/post/estimating-the-security-of-homomorphic-schemes) - December 2021
- [Homomorphic Encryption 101](https://www.zama.ai/post/homomorphic-encryption-101) - December 2021
- [A homomorphic FPGA implementation of the Intel 4004 — Part 1](https://www.zama.ai/post/homomorphic-fpga-implementation-of-the-intel-4004-part-1) - November 2021
- [People should not care about privacy](https://www.zama.ai/post/people-should-not-care-about-privacy) - August 2021
<br></br>

## Research papers and publications
Research papers and publications by the Zama team sorted by date

- [Crypto dark matter on the torus: Oblivious PRFs from shallow PRFs and TFHE](https://doi.org/10.1007/978-3-031-58751-1_16) - May 2024 - EUROCRYPT 2024
- [TFHE public-key encryption revisited](https://doi.org/10.1007/978-3-031-58868-6_11) - May 2024 - CT-RSA 2024
- Homomorphic evaluation of LWR-based PRFs and application to transciphering [[ePrint version](https://ia.cr/2024/665)] - April 2024 - ePrint Archive
- [Simulation-extractable KZG polynomial commitments and applications to HyperPlonk](https://doi.org/10.1007/978-3-031-57722-2_3) - April 2024 - PKC 2024
- [Vector commitments with proofs of smallness: Short range proofs and more](https://doi.org/10.1007/978-3-031-57722-2_2) [[ePrint version](https://ia.cr/2023/800)] - April 2024 - PKC 2024
- Towards verifiable FHE in practice: Proving correct execution of TFHE's bootstrapping using plonky2 [[ePrint version](https://ia.cr/2024/451)] - March 2024 - ePrint Archive
- [The key lattice framework for concurrent group messaging](https://doi.org/10.1007/978-3-031-54773-7_6) [[ePrint version](https://ia.cr/2022/1531)] - March 2024 - ACNS 2024
- [A new approach to efficient and secure fixed-point computation](https://doi.org/10.1007/978-3-031-54770-6_3) [[ePrint version](https://ia.cr/2024/035)] - March 2024 - ACNS 2024
- Neural network training on encrypted data with TFHE [[arXiv version](https://arxiv.org/abs/2401.16136)] - January 2024 - arXiv<!-- markdown-link-check-disable-next-line -->
- [Computing e-th roots in number fields](https://doi.org/10.1137/1.9781611977929.16) [[arXiv version](https://arxiv.org/abs/2305.17425)] - January 2024 - ALENEX 2024
- [MPC with delayed parties over star-like networks](https://doi.org/10.1007/978-981-99-8721-4_6) [[ePrint version](https://ia.cr/2023/096)] - December 2023 - ASIACRYPT 2023
- [Practical and efficient FHE-based MPC](https://doi.org/10.1007/978-3-031-47818-5_14) [[ePrint version](https://ia.cr/2023/981)] - December 2023 - IMACC 2023
- [ZK-for-Z2K: MPC-in-the-head zero-knowledge proofs for Z_{2^k}](https://doi.org/10.1007/978-3-031-47818-5_8) [[ePrint version](https://ia.cr/2023/1057)] - December 2023 - IMACC 2023
- [Multiparty computation: To secure privacy, do the math](https://dl.acm.org/doi/10.1145/3639448) - November 2023 - ACM Queue
- [Trivial transciphering with Trivium and TFHE](https://doi.org/10.1145/3605759.3625255) [[ePrint version](https://ia.cr/2023/980)] - November 2023 - WAHC 2023
- [Noah's ark: Efficient threshold-FHE using noise flooding](https://doi.org/10.1145/3605759.3625259) [[ePrint version](https://ia.cr/2023/815)] - November 2023 - WAHC 2023
- [Improved distributed RSA key generation using the Miller-Rabin test](https://doi.org/10.1145/3576915.3623163) - November 2023 - CCS 2023
- Updatable privacy-preserving blueprints [[ePrint version](https://ia.cr/2023/1787)] - November 2023 - ePrint Archive
- [SoK: Privacy-enhancing technologies in finance](https://doi.org/10.4230/LIPIcs.AFT.2023.12) [[ePrint version](https://ia.cr/2023/122)] - October 2023 - AFT 2023
- [fhEVM - Confidential EVM Smart Contracts using Fully Homomorphic Encryption](https://github.com/zama-ai/fhevm/blob/main/fhevm-whitepaper.pdf) - September 2023 - White paper
- [On the precision loss in approximate homomorphic encryption](https://doi.org/10.1007/978-3-031-53368-6_16) [[ePrint version](https://ia.cr/2022/162)] - August 2023 - SAC 2023
- [Attribute-based single sign-on: Secure, private, and efficient](https://doi.org/10.56553/popets-2023-0097) [[ePrint version](https://ia.cr/2023/915)] - July 2023 - PoPETs 2023
- [Computing on encrypted data](https://doi.org/10.1109/MSEC.2023.3279517) - July 2023 - IEEE Security & Privacy
- Faster secret keys for (T)FHE [[ePrint version](https://ia.cr/2023/979)] - June 2023 - ePrint Archive
- [Deep neural networks for encrypted inference with TFHE](https://doi.org/10.1007/978-3-031-34671-2_34) [[ePrint version](https://ia.cr/2023/257)] - June 2023 - CSCML 2023<!-- markdown-link-check-disable-next-line -->
- [Parameter optimization & larger precision for (T)FHE](https://doi.org/10.1007/s00145-023-09463-5) [[ePrint version](https://ia.cr/2022/704)] - ‍June 2023 - Journal of Cryptology
- [Topical Collection on Computing on Encrypted Data](https://doi.org/10.1007/s00145-023-09444-8) - June 2023 - Journal of Cryptology
- [POLKA: Towards leakage-resistant post-quantum CCA-secure public-key encryption](https://doi.org/10.1007/978-3-031-31368-4_5) [[ePrint version](https://eprint.iacr.org/2022/873)] - ‍May 2023 - PKC 2023
- [On-line/Off-line DCR-based homomorphic encryption and applications](https://doi.org/10.1007/978-3-031-30872-7_5) [[ePrint version](https://ia.cr/2023/048)] - April 2023 - CT-RSA 2023
- TFHE public-key encryption revisited [[ePrint version](https://ia.cr/2023/603)] - April 2023 - ePrint Archive
- Lightweight asynchronous verifiable secret sharing with optimal resilience [[ePrint version](https://ia.cr/2023/536)] - April 2023 - ePrint Archive
- [Differential fault analysis](https://doi.org/10.1007/978-3-642-27739-9_1707-1) ‍‍‍- March 2023 - Encyclopedia of Cryptography, Security and Privacy
- [Improving convergence and practicality of slide-type reductions](https://doi.org/10.1016/j.ic.2023.105012) [[ePrint version](https://ia.cr/2023/140)] - March 2023 - Information and Computation
- [Privacy-preserving tree-based inference with TFHE](https://link.springer.com/chapter/10.1007/978-3-031-52426-4_10) [[ePrint version](https://ia.cr/2023/258)] - February 2023 - ePrint Archive
- On side-channel and CVO attacks against TFHE and FHEW [[ePrint version](https://ia.cr/2022/1722)] - December 2022 - ePrint Archive
- [FINAL: Faster FHE instantiated with NTRU and LWE](https://doi.org/10.1007/978-3-031-22966-4_7) [[ePrint version](https://ia.cr/2022/074)] - ‍December 2022 - ASIACRYPT 2022
- The key lattice framework for concurrent group messaging [[ePrint version](https://ia.cr/2022/1531)] - November 2022 - ePrint Archive
- [Liberating TFHE: Programmable bootstrapping with general quotient polynomials](https://doi.org/10.1145/3560827.3563376) [[ePrint version](https://ia.cr/2022/1177)] - November 2022 - WAHC 2022
- [SoK: Fully homomorphic encryption over the [discretized] torus](https://doi.org/10.46586/tches.v2022.i4.661-692) [[ePrint version](https://ia.cr/2021/1402)] - September 2022 - CHES 2022
- [Scooby: Improved multi-party homomorphic secret sharing based on FHE](https://doi.org/10.1007/978-3-031-14791-3_24) [[ePrint version](https://ia.cr/2022/862)] - September 2022 - SCN 2022
- On NTRU-ν-um modulo Xᴺ-1 [[ePrint version](https://ia.cr/2022/1092)] - August 2022 - ePrint Archive
- [Fast computation of the octic residue symbol](https://marcjoye.github.io/papers/Joy22octic.pdf) - ‍August 2022 - NutMiC 2022
- Secure branching program evaluation [[ePrint version](https://ia.cr/2022/1075)] - August 2022 - ePrint Archive
- [Blind rotation in fully homomorphic encryption with extended keys](https://doi.org/10.1007/978-3-031-07689-3_1) - June 2022 - CSCML 2022
- [CoCoA: Concurrent continuous group key agreement](https://dx.doi.org/10.1007/978-3-031-07085-3_28) [[ePrint version](https://ia.cr/2022/251)] - May 2022 - Eurocrypt 2022
- Towards globally optimized hybrid homomorphic encryption: Featuring the Elisabeth stream cipher [[ePrint version](https://ia.cr/2022/180)] - February 2022 - ePrint Archive
- [A pairing-free signature scheme from correlation intractable hash function and strong Diffie-Hellman assumption](https://doi.org/10.1007/978-3-030-95312-6_2) [[ePrint version](https://ia.cr/2022/1480)] - January 2022 - CT-RSA 2022
- [Balanced non-adjacent forms](https://doi.org/10.1007/978-3-030-92078-4_19) [[ePrint version](https://ia.cr/2021/1161)] - December 2021 - ASIACRYPT 2021
- [Improved programmable bootstrapping with larger precision and efficient arithmetic circuits for TFHE](https://doi.org/10.1007/978-3-030-92078-4_23) [[ePrint version](https://ia.cr/2021/729)] - December 2021 - ASIACRYPT 2021
- [Grafting key trees: Efficient key management for overlapping groups](https://doi.org/10.1007/978-3-030-90456-2_8) [[ePrint version](https://ia.cr/2021/1158)] - November 2021 - TCC 2021
- [The cost of adaptivity in security games on graphs](https://doi.org/10.1007/978-3-030-90453-1_19) [[ePrint version](https://ia.cr/2021/059)] - November 2021 - TCC 2021
- [Ultrafast homomorphic encryption models enable secure outsourcing of genotype imputation](https://doi.org/10.1016/j.cels.2021.07.010) [[bioRxiv version](https://doi.org/10.1101/2020.07.02.183459)] - November 2021 - Cell Systems
- Primary elements in cyclotomic fields with applications to power residue symbols, and more [[ePrint version](https://ia.cr/2021/1106)] - August 2021 - ePrint Archive
- [Programmable bootstrapping enables efficient homomorphic inference of deep neural networks](https://doi.org/10.1007/978-3-030-78086-9_1) [[ePrint version](https://ia.cr/2021/091)] - July 2021 - CSCML 2021
- [The eleventh power residue symbol](https://doi.org/10.1515/jmc-2020-0077) [[ePrint version](https://ia.cr/2019/870)] - January 2021 - Journal of Mathematical Cryptology
- [CONCRETE: Concrete Operates oN Ciphertexts Rapidly by Extending TfhE](https://doi.org/10.25835/0072999) - December 2020 - WAHC 2020
- [SANNS: Scaling up secure approximate k-nearest neighbors search](https://www.usenix.org/conference/usenixsecurity20/presentation/chen-hao) - August 2020 - USENIX 2020
<br></br>

## Contributed talks and posters
Contributed talks and posters by the Zama team sorted by date
- [Advanced FHE protocols for the blockchain](https://iacr.org/submit/files/slides/2024/rwc/rwc2024/5/slides.pptx) - ‍‍March 2024 - RWC 2024
- [Revisiting oblivious top-k selection with applications to secure k-NN classification](https://github.com/FHE-org/fhe-org.github.io/files/14896282/1635-Geelen.pdf) - ‍‍March 2024 - FHE.org 2024
- [Security guidelines for implementing homomorphic encryption](https://github.com/FHE-org/fhe-org.github.io/files/14896275/1445-Gong.updated.pdf) - ‍‍March 2024 - FHE.org 2024
- [TFHE simplified: A practical guide to integer arithmetic and reliability](https://github.com/FHE-org/fhe-org.github.io/files/14896277/1545-Orfila.pdf) - ‍‍March 2024 - FHE.org 2024
- [Neural network training on encrypted data with TFHE](https://github.com/FHE-org/fhe-org.github.io/files/14896476/Zama.30-Montero.pdf) - ‍‍March 2024 - FHE.org 2024
- [Towards verifiable bootstrapping in practice: Proving correct execution of TFHE’s blind rotation using plonky2](https://github.com/FHE-org/fhe-org.github.io/files/14896490/Zama.13-Walter.pdf) - ‍‍March 2024 - FHE.org 2024
- [Game of life, revisited](https://github.com/FHE-org/fhe-org.github.io/files/14896286/Zama.03-Mames.pdf) - ‍‍March 2024 - FHE.org 2024
- [Homomorphic integer division for TFHE](https://github.com/FHE-org/fhe-org.github.io/files/14896469/Zama.37-Deo.pdf) - ‍‍March 2024 - FHE.org 2024
- [The inhibitor: ReLU and addition-based attention for efficient transformers under fully homomorphic encryption on the torus](https://github.com/FHE-org/fhe-org.github.io/files/14896485/Zama.23-Brannvall.pdf) - ‍‍March 2024 - FHE.org 2024
- [Privacy-preserving tree-based inference with TFHE](https://github.com/zama-ai/awesome-zama/raw/main/data/PPML2023PresentationTrees.pdf) - August 2023 - PPML 2023
- [Recent advances in homomorphic compilation](https://github.com/FHE-org/fhe-org.github.io/raw/main/conferences/conference-2023/media/homomorphic-compilation.pdf) - ‍‍March 2023 - FHE.org 2023
- [On NTRU-ν-um modulo Xᴺ-1](https://eprint.iacr.org/2022/1092) - ‍March 2023 - FHE.org 2023
- [Parameter optimization & larger precision for (T)FHE](https://github.com/FHE-org/fhe-org.github.io/raw/main/conferences/conference-2023/media/DL-ST-slides.pdf) - ‍March 2023 - FHE.org 2023
- [Private smart contracts using homomorphic encryption](https://github.com/FHE-org/fhe-org.github.io/raw/main/conferences/conference-2023/media/private-smart-contracts.pdf) - ‍March 2023 - FHE.org 2023
- [Fully homomorphic encryption for user privacy and model intellectual property protection](https://github.com/FHE-org/fhe-org.github.io/raw/main/conferences/conference-2023/media/user-privacy-model-protection.pdf) - ‍March 2023 - FHE.org 2023
- [Hybrid attacks on LWE and the lattice estimator](https://github.com/FHE-org/fhe-org.github.io/raw/main/conferences/conference-2022/media/hybrid-attacks.pdf) - May 2022 - FHE.org 2022
- [Fast, easy, and accessible FHE with Concrete and specialized accelerators](https://github.com/FHE-org/fhe-org.github.io/raw/main/conferences/conference-2022/media/concrete-and-specialized-accelerators.pdf) - May 2022 - FHE.org 2022
- [Concrete ML: A data-scientist-friendly toolkit for machine learning over encrypted data](https://github.com/FHE-org/fhe-org.github.io/raw/main/conferences/conference-2022/media/concrete-ml.pdf) - May 2022 - FHE.org 2022
- [Performance of hierarchical transforms in homomorphic encryption: A case study on logistic regression inference](https://github.com/FHE-org/fhe-org.github.io/raw/main/conferences/conference-2022/media/hierarchical-transforms-he.pdf) - May 2022 - FHE.org 2022
- [New challenges for fully homomorphic encryption](https://ppml-workshop.github.io/ppml20/pdfs/Chillotti_et_al.pdf) - December 2020 - PPML 2020
<br></br>
