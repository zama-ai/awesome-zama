# Supporting Guide to Zama AI GitHub Organization

The guide as a central hub, and sequences content across repos for assimilation: start with "why FHE matters," move to "core tools," then "applications," and end with "advanced engagement." Each section includes:

- **Overview**: What it covers and its importance.
- **Key Repos/Files**: Clickable GitHub links to repos, MD files, or PDFs.
- **Learning Path**: Step-by-step reading/building order with cognitive tips (e.g., connect ideas via examples).
- **Transitions**: How it leads to the next section.

By the end, you'll conceptualize Zama's ecosystem, engage with FHEVM standards/contracts, and be ready to contribute or build. For updates, check repo commits or [Zama's docs site](https://docs.zama.ai/) (linked from repos).

## 1. High-Level Overview (FHE Fundamentals and Zama's Ecosystem)
Grasp FHE's power for privacy in AI/blockchain without math overload. Ideal for beginners/non-devs to build intuition; devs, note how it enables encrypted ops. Covers Zama's vision via curated resources.

### Key Concepts Covered
- FHE basics: Encrypt data, compute on ciphertexts, decrypt results—perfect for confidential AI/ML and smart contracts.
- Zama's stack: From low-level crypto (TFHE) to high-level apps (FHEVM).
- Use cases: Encrypted ML predictions, private blockchain txs.

### Key Repos/Files
- [`awesome-zama/README.md`](https://github.com/zama-ai/awesome-zama/blob/main/README.md): Curated hub with sections on libraries, papers, and tutorials.
- [`fhevm/fhevm-whitepaper.pdf`](https://github.com/zama-ai/fhevm/blob/main/fhevm-whitepaper.pdf): Intro to FHEVM for confidential EVM contracts.
- [`fhevm-solidity/fhevm-whitepaper.pdf`](https://github.com/zama-ai/fhevm-solidity/blob/main/fhevm-whitepaper.pdf): Original FHEVM paper (Sep 2023).
- [`fhevm-solidity/fhevm-whitepaper-v2.pdf`](https://github.com/zama-ai/fhevm-solidity/blob/main/fhevm-whitepaper-v2.pdf): V2 updates (Dec 2024).
- [`tfhe-rs-handbook/tfhe-rs-handbook.pdf`](https://github.com/zama-ai/tfhe-rs-handbook/blob/main/tfhe-rs-handbook.pdf): Practical TFHE guide (Feb 2025).

### Learning Path
1. Start with [`awesome-zama/README.md`](https://github.com/zama-ai/awesome-zama/blob/main/README.md) for a bird's-eye view—scan "Libraries and Solutions" for Zama's tools.
2. Read [`fhevm/fhevm-whitepaper.pdf`](https://github.com/zama-ai/fhevm/blob/main/fhevm-whitepaper.pdf) (or litepaper at [docs.zama.ai/protocol/zama-protocol-litepaper](https://docs.zama.ai/protocol/zama-protocol-litepaper)) to understand FHE in blockchain (focus on diagrams for non-devs).
3. Dive into [`tfhe-rs-handbook/tfhe-rs-handbook.pdf`](https://github.com/zama-ai/tfhe-rs-handbook/blob/main/tfhe-rs-handbook.pdf) for FHE mechanics—non-devs skim Ch. 1-2; devs note bootstrapping.
4. Explore demos in README (e.g., [Encrypted DNA testing](https://huggingface.co/spaces/zama-fhe/encrypted_dna)) to see FHE in action.

**Tips**: Visualize FHE as "computing in a locked box." Connect to real-world: How does it fix data leaks in AI models? Revisit for reinforcement.

**Transition**: With FHE intuition, explore core libraries to see the "building blocks" under the hood.

## 2. Core FHE Libraries (Low-Level Crypto Tools)
These repos provide the cryptographic primitives. Start here for dev foundations; non-devs skim READMEs for concepts like "programmable bootstrapping."

### 2.1 TFHE-rs (Boolean/Integer Ops on Encrypted Data)
Overview: Pure Rust TFHE implementation—Zama's fast, flexible FHE scheme for encrypted arithmetic.

#### Key Files
- [`tfhe-rs/README.md`](https://github.com/zama-ai/tfhe-rs/blob/main/README.md): Installation, features (e.g., GPU support).
- External: [docs.zama.ai/tfhe-rs](https://docs.zama.ai/tfhe-rs) (tutorials linked from README).

#### Learning Path
1. Read README for setup (`cargo add tfhe`).
2. Follow [TFHE-rs tutorials](https://docs.zama.ai/tfhe-rs/tutorials) (e.g., array ops video in awesome-zama).
3. Experiment: Run basic encrypted addition example.

**Tips**: Devs, test on GPU for speed gains; non-devs, note how it enables "invisible" computations.

### 2.2 Concrete (Python-to-FHE Compiler)
Overview: Compiles Python code to FHE circuits—bridges high-level programming to crypto.

#### Key Files
- [`concrete/README.md`](https://github.com/zama-ai/concrete/blob/main/README.md): Quickstart, examples.
- See [docs.zama.ai/concrete](https://docs.zama.ai/concrete) for full guides.

#### Learning Path
1. Install via README (pip install concrete-compiler).
2. Compile a simple Python func (e.g., add two numbers encrypted).
3. Explore Concrete releases in awesome-zama for updates.

**Tips**: Think of it as "Python magic" for privacy—build a toy app to assimilate.

### 2.3 Threshold-FHE (MPC for FHE Keys)
Overview: Threshold protocols for distributed key gen/decryption—enhances security for multi-party FHE.

#### Key Files
- [`threshold-fhe/docs/threshold-benchmark.md`](https://github.com/zama-ai/threshold-fhe/blob/main/docs/threshold-benchmark.md): Benchmarks and requirements.
- [`threshold-fhe/README.md`](https://github.com/zama-ai/threshold-fhe/blob/main/README.md): Setup for distributed decryption example.

#### Learning Path
1. Read README for overview (e.g., threshold key gen).
2. Run [`examples/distributed_decryption.rs`](https://github.com/zama-ai/threshold-fhe/blob/main/examples/distributed_decryption.rs) example.
3. Check benchmarks MD for perf tips.

**Tips**: Non-devs: It's like "shared locks" for team privacy. Devs: Integrate with TFHE-rs.

**Transition**: Core libs ready? Apply them to apps like ML (Concrete ML) or blockchain (FHEVM).

## 3. Applications (Building with FHE)
Apply libs to real domains. Sequence: ML first (simpler), then blockchain (FHEVM focus).

### 3.1 Concrete ML (Privacy-Preserving ML)
Overview: FHE-enabled ML framework—train/deploy models on encrypted data, compatible with scikit-learn/PyTorch.

#### Key Files
- [`concrete-ml/README.md`](https://github.com/zama-ai/concrete-ml/blob/main/README.md): Installation, quickstart.
- [`concrete-ml/docs/built-in-models/linear.md`](https://github.com/zama-ai/concrete-ml/blob/main/docs/built-in-models/linear.md): Linear models API (e.g., logistic regression on encrypted data).
- [`concrete-ml/docs/built-in-models/tree.md`](https://github.com/zama-ai/concrete-ml/blob/main/docs/built-in-models/tree.md): Tree models (scikit/XGBoost equivs).
- [`concrete-ml/docs/built-in-models/neural-networks.md`](https://github.com/zama-ai/concrete-ml/blob/main/docs/built-in-models/neural-networks.md): PyTorch-to-FHE conversion.
- Use-case examples: [`use_case_examples/titanic/KaggleTitanic.ipynb`](https://github.com/zama-ai/concrete-ml/blob/main/use_case_examples/titanic/KaggleTitanic.ipynb) (encrypted Titanic prediction).

#### Learning Path
1. Setup via README (pip install concrete-ml).
2. Read linear/tree MDs for built-ins—run scikit-like examples.
3. Convert a NN via neural-networks MD.
4. Try demos (e.g., [Encrypted sentiment analysis](https://huggingface.co/spaces/zama-fhe/encrypted_sentiment_analysis) from awesome-zama).

**Tips**: Non-devs: See how FHE protects health/finance data. Devs: Quantize models for efficiency.

### 3.2 FHEVM (Confidential Smart Contracts)
Overview: EVM-compatible FHE layer for encrypted blockchain ops—core of Zama's protocol. Enables private txs/DeFi.

#### Key Files
- [`fhevm/README.md`](https://github.com/zama-ai/fhevm/blob/main/README.md): Monorepo overview, setup.
- [`fhevm/fhevm-whitepaper.pdf`](https://github.com/zama-ai/fhevm/blob/main/fhevm-whitepaper.pdf): Protocol details.
- In [`fhevm-solidity`](https://github.com/zama-ai/fhevm-solidity): [`fhevm-whitepaper-v2.pdf`](https://github.com/zama-ai/fhevm-solidity/blob/main/fhevm-whitepaper-v2.pdf) (V2 features).
- [`fhevm-hardhat-template/README.md`](https://github.com/zama-ai/fhevm-hardhat-template/blob/main/README.md): Dev env setup, tests.
- Subdirs: `fhevm/gateway-contracts/` (entry points), `fhevm/host-contracts/` (FHE logic), `fhevm/test-suite/` (examples).

#### Learning Path
1. Read README and whitepaper for concepts (e.g., ciphertext handles in Solidity).
2. Setup Hardhat template: Follow [`fhevm-hardhat-template` guide](https://github.com/zama-ai/fhevm-hardhat-template) for local net.
3. Build: Upgrade a basic contract (see [Quickstart tutorial](https://docs.zama.ai/protocol/solidity-guides/getting-started/quick-start-tutorial)).
4. Test: Run suite examples; explore V2 paper for advanced (e.g., CMUX operator tutorial video in awesome-zama).
5. Engage: [Hello FHEVM bounty](https://www.zama.ai/post/zama-bounty-program-season-10-create-a-hello-fhevm-tutorial) for dApp build.

**Tips**: Non-devs: FHEVM = "secret voting in Ethereum." Devs: Use encrypted types like `uint256 encrypted`—practice incremental upgrades.

**Transition**: Apps mastered? Join the community via bounties for hands-on contribution.

## 4. Community and Advanced Resources (Engagement & Research)
For deepening knowledge and contributing. Includes papers, talks, and incentives.

### Key Repos/Files
- [`bounty-program/README.md`](https://github.com/zama-ai/bounty-program/blob/main/README.md): €500k+ rewards for FHE tasks (e.g., FHEVM tutorials).
- Awesome-zama sections: Whitepapers (sorted by date), Research papers (e.g., peer-reviewed on TFHE advances), Talks (videos/posters).
- Demos: Encrypted use cases (e.g., [credit card approval](https://huggingface.co/spaces/zama-fhe/credit_card_approval_prediction)).

### Learning Path
1. Browse bounties README for open challenges—pick one aligned with your skills.
2. Scan awesome-zama "Research papers" for latest (e.g., FHEVM V2).
3. Watch talks (e.g., [fhEVM tutorial video](https://www.youtube.com/watch?v=1FtbyHZwNX4)).

**Tips**: Bounties build portfolio; non-devs, start with announcement blogs in awesome-zama.

## Additional Repo Navigation Tips
- **Root Across Repos**: Always check `README.md` for quickstarts; use GitHub search for "FHEVM" across org.
- **Building Locally**: Follow per-repo installs (e.g., Rust for TFHE-rs, Python for Concrete).
- **Contributing**: Fork, PR to fix docs/bugs; join [community.zama.ai](https://community.zama.ai/) for support.
- **Search Tip**: GitHub org search for keywords (e.g., "tutorial") to find buried MDs.
- **External Complements**: Repos link to [docs.zama.ai](https://docs.zama.ai/) for polished guides (e.g., FHEVM Solidity overview).

This guide builds knowledge sequentially: concepts → tools → apps → community. Revisit for projects like an FHEVM dApp. For mainnet updates, check [Zama blog](https://www.zama.ai/post).


Happy encrypting!
