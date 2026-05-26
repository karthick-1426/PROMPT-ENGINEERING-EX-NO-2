# EX-02-Cross-Platform-Prompting-Evaluating-Diverse-Techniques-in-AI-Powered-Text-Summarization

## AIM
To evaluate and compare the effectiveness of prompting techniques (zero-shot, few-shot, chain-of-thought, role-based) across different AI platforms (e.g., ChatGPT, Gemini, Claude, Copilot) in a specific task: text summarization.


## Scenario:
You are part of a content curation team for an educational platform that delivers quick summaries of research papers to undergraduate students. Your task is to summarize a 500-word technical article on "The Basics of Blockchain Technology" using multiple AI platforms and prompting strategies.

Your goal is to determine which combination of prompting technique + platform provides the best summary in terms of:

Accuracy

Coherence

Simplicity

Speed

User experience

## Algorithm

1. **Article Selection**
   Select a \~500-word technical article titled *"The Basics of Blockchain Technology"*.
````
The Basics of Blockchain Technology

In recent years, blockchain technology has gained significant attention for its potential to revolutionize industries beyond its original use in cryptocurrencies like Bitcoin. At its core, blockchain is a decentralized, distributed ledger system that securely records transactions across a network of computers. What makes blockchain unique is its ability to ensure transparency, security, and immutability without the need for a central authority.

What is Blockchain?

A blockchain can be thought of as a chain of digital “blocks,” each containing a record of transactions. These blocks are linked together in chronological order using cryptographic techniques. Once a block is added to the chain, the information inside it cannot be altered without changing all subsequent blocks, making the system resistant to tampering or fraud.

Key Features of Blockchain

Decentralization – Traditional databases are usually controlled by a central entity, but blockchain distributes the ledger across many nodes (computers). Every participant in the network has a copy of the blockchain, ensuring no single point of failure.

Transparency – Transactions recorded on the blockchain are visible to all participants. While identities can remain anonymous, the transaction history is permanent and accessible, which helps build trust.

Immutability – Once data is recorded on a blockchain, it cannot be changed or deleted. This permanence reduces the risk of fraud and enhances accountability.

Security – Blockchain uses cryptographic algorithms to secure transactions and control access. Each block is connected to the previous one using a unique hash, making it extremely difficult to alter data.

How Blockchain Works

When a transaction occurs, it is verified by participants in the network through a process called consensus. Different blockchains use different consensus mechanisms, such as Proof of Work (PoW) or Proof of Stake (PoS). Once verified, the transaction is grouped into a block, which is then added to the chain in a way that ensures it cannot be modified without network-wide agreement.

Applications of Blockchain

While blockchain is best known for enabling cryptocurrencies, its applications extend to many fields:

Finance – Beyond digital currencies, blockchain can streamline cross-border payments, reduce fraud, and increase transparency in banking.

Supply Chain Management – Companies can track goods from origin to destination, ensuring authenticity and reducing counterfeiting.

Healthcare – Patient records can be securely stored and shared across providers while maintaining privacy and accuracy.

Voting Systems – Blockchain-based voting can increase transparency, reduce fraud, and enhance trust in democratic processes.

Smart Contracts – These are self-executing contracts with conditions directly written into code, enabling automated and trustless transactions.

Challenges in Blockchain

Despite its advantages, blockchain faces several challenges. Scalability remains an issue, as processing a large number of transactions can be slow and energy-intensive, especially in PoW systems. Regulatory uncertainties and concerns about data privacy also pose hurdles to widespread adoption. Additionally, while immutability is a strength, it can also be a weakness if incorrect or fraudulent data is entered into the system.

Conclusion

Blockchain technology represents a transformative shift in how data and transactions are managed. By combining decentralization, transparency, and security, it has the potential to disrupt industries ranging from finance to healthcare. However, challenges related to scalability, regulation, and energy consumption must be addressed before blockchain can achieve its full potential. As research and innovation continue, blockchain is likely to become a foundational technology for the digital future.
````

3. **Prompting Strategies Definition**
   Prepare the following four prompting strategies:

   * **Zero-shot**: Directly ask the model to summarize without examples.
   * **Few-shot**: Provide 2–3 examples of summaries for similar technical texts before asking for the summary.
   * **Chain-of-Thought**: Prompt the model to explain or break down the text logically before summarizing.
   * **Role-based**: Instruct the model to act as a specific role (e.g., “a university professor summarizing for freshmen”).

4. **Platform Selection**
   Use the following AI platforms:

   * ChatGPT (OpenAI)
   * Gemini (Google)
   * Claude (Anthropic)
   * Copilot (Microsoft)

5. **Execution**
   For each platform:

   * Apply each prompting strategy using the same input article.
   * Record the output summary.
   * Note time taken to generate the summary.

6. **Evaluation Criteria**
   Evaluate each generated summary using the following:

   * **Accuracy**: Does the summary correctly capture the main points of the article?
   * **Coherence**: Is the summary logically structured and easy to follow?
   * **Simplicity**: Is the language accessible for undergraduate students?
   * **Speed**: How fast is the response?
   * **User Experience**: Was the interface intuitive, and was the output easy to copy/save?

7. **Scoring & Analysis**

   * Assign scores (1 to 5) for each criterion across all combinations.
   * Tabulate results for comparison.
   * Identify the best-performing strategy-platform combination.

---

## Output
### Chat GPT
### ZeroShot
```
Summary
Blockchain is a decentralized, distributed ledger that records transactions securely and transparently without a central authority. It stores data in linked blocks using cryptography, ensuring immutability and security.

Key Features:

Decentralization – no single point of control.

Transparency – transactions are visible to all participants.

Immutability – data cannot be changed once recorded.

Security – cryptographic hashes protect records.

How it Works: Transactions are verified through consensus (e.g., Proof of Work, Proof of Stake) before being added as permanent blocks to the chain.

Applications: Finance (cross-border payments), supply chain tracking, healthcare records, secure voting, and smart contracts.

Challenges: Scalability, high energy use (especially PoW), regulatory uncertainty, privacy concerns, and risks of permanent incorrect data.

Conclusion: Blockchain has transformative potential across industries, but scalability, regulation, and energy efficiency must improve for widespread adoption.
```
### Few Shots
```
Topic: Blockchain Technology

Definition: A decentralized, distributed ledger that records secure and transparent transactions without a central authority.

Features: Decentralization, transparency, immutability, and cryptographic security.

How it Works: Transactions are verified via consensus (e.g., Proof of Work/Stake) and added permanently to the chain.

Applications: Finance (cross-border payments), supply chain tracking, healthcare records, voting systems, smart contracts.

Challenges: Scalability, energy usage, regulatory uncertainty, privacy issues, permanent incorrect data.

Conclusion: Blockchain has disruptive potential but needs improvements in scalability, regulation, and efficiency for broader adoption.
```
### Chain of Thoughts
```
Blockchain is a decentralized, distributed ledger that records transactions securely and transparently without central control. It links transaction data in blocks using cryptography, ensuring immutability and security. Transactions are verified through consensus mechanisms like Proof of Work or Proof of Stake before being permanently added to the chain.

Its applications go beyond cryptocurrencies, including finance (cross-border payments), supply chain tracking, healthcare records, voting systems, and smart contracts. Despite its advantages, blockchain faces challenges such as scalability, high energy use, regulatory uncertainty, and data privacy concerns.

Overall, blockchain has transformative potential but requires improvements in efficiency, scalability, and regulation for widespread adoption.
```
### Role based
```
Blockchain is like a shared digital notebook that no single person controls. Every entry, once written, is permanent, transparent, and secured with cryptography, making it very hard to cheat or tamper with. It works by grouping transactions into blocks, which are verified by the network through consensus methods like Proof of Work or Proof of Stake.

While it began with Bitcoin, blockchain today has many applications — from banking and supply chain tracking to healthcare, elections, and smart contracts. However, it still faces challenges such as slow transaction speed, high energy use, regulatory uncertainty, and data privacy issues.

In short, blockchain has the potential to reshape industries by ensuring trust, transparency, and security — but it’s not a magic bullet, and overcoming its limitations will be key to its future success
```
## Gemini
### Zero Shot
```
Summary:

    Blockchain technology is a decentralized digital ledger that records transactions securely across a network of computers.
    Unlike traditional databases controlled by one authority, blockchain distributes identical copies of data to many nodes, reducing the risk of failure or manipulation.
    Each transaction is stored in a “block” and linked with others using cryptography, making the chain transparent, secure, and nearly impossible to alter.
    Transactions are verified through consensus methods like Proof of Work or Proof of Stake. While first used for cryptocurrencies such as Bitcoin, blockchain now benefits industries like finance, supply chain, healthcare, and even voting systems.
    It also enables “smart contracts,” which automatically execute coded agreements. Despite its promise, blockchain faces challenges in scalability, regulation, and energy use. Still, it is seen as a key technology for the digital future.
```
### Few Shot
```
Shot 1: The Core Concept
Blockchain is a secure, decentralized digital ledger that records transactions in a way that prevents tampering. It's built on a "chain" of data "blocks" linked by cryptography.

Shot 2: Key Features
Its main features are decentralization, where the network is distributed across many computers, immutability, meaning data can't be changed once recorded, and transparency, where all transactions are visible. This removes the need for a central authority.

Shot 3: Applications & Challenges
Beyond cryptocurrencies, blockchain can be used in supply chain management, healthcare, and voting. However, it faces challenges like scalability (it can be slow) and energy consumption, particularly with older consensus methods like Proof of Work.
```

## Claude
### Role Based
```
Good morning, class! Today we're going to explore blockchain technology, and I promise it's much simpler than it sounds. Think of blockchain like a shared notebook that everyone in the class can see, but no one can erase what's already written.

What Exactly Is Blockchain?

Imagine you and your friends keep track of who owes money to whom by writing it down in a special notebook. Instead of one person holding this notebook, everyone gets an identical copy. When someone makes a new transaction, everyone updates their notebook at the same time. That's essentially how blockchain works - it's a digital record book that's shared across many computers.

The "blocks" are like pages in this notebook, and the "chain" connects these pages in order. Each page references the previous one, so if someone tries to change an old page, everyone would notice because it wouldn't match their copies.

Why Should You Care?

Blockchain solves a fundamental problem: How do you trust strangers in digital transactions without needing a bank or government to verify everything? It creates trust through mathematics and consensus rather than through institutions.

The key features are straightforward. **Decentralization** means no single entity controls the system - it's like having a group project where everyone has equal say. **Transparency** means all transactions are visible, like posting your grades on a public board. **Immutability** means once something is recorded, it can't be changed - like writing in permanent ink. **Security** comes from advanced mathematics that makes cheating nearly impossible.

Real-World Applications

Beyond digital money like Bitcoin, blockchain has exciting applications you'll likely encounter in your careers. Companies use it to track products from factory to store, ensuring your organic coffee is actually organic. Hospitals might use it to securely share your medical records between doctors. Some countries are experimenting with blockchain voting to make elections more transparent.

The Challenges We Face

Like any new technology, blockchain isn't perfect. It can be slow - imagine if updating that shared notebook required everyone to solve a puzzle first. It also uses a lot of energy, especially older systems. Think of it like having to run a marathon every time you want to write in the notebook.

Your Takeaway

Blockchain represents a new way of organizing information and trust in our digital world. While the technology is complex underneath, the concept is simple: creating trust and transparency without relying on traditional authorities. As future professionals, understanding this shift in how we handle digital trust will be valuable regardless of your chosen field.

Remember, you don't need to become blockchain experts overnight, but understanding these fundamental concepts will help you navigate an increasingly digital economy.
```
### Chain of Thoughts
```
Blockchain technology can be understood through a logical progression of interconnected concepts that build upon each other.

Starting Point: The Problem

Traditional systems rely on central authorities to verify and record transactions, creating single points of failure and trust issues. This leads to the need for a decentralized solution that can maintain security and trust without central control.

The Solution: Blockchain Structure

To address this problem, blockchain creates a chain of digital blocks where each block contains transaction records. These blocks are linked chronologically using cryptographic techniques, forming an unbreakable chain where altering one block would require changing all subsequent blocks.

Building the Foundation: Core Features

This structure naturally creates four essential characteristics. First, **decentralization** emerges because the ledger is distributed across multiple network nodes rather than stored in one location. Second, **transparency** results from making all transactions visible to network participants. Third, **immutability** develops because changing recorded data becomes computationally impossible. Fourth, **security** is achieved through cryptographic protection and hash-based block connections.

Making It Work: The Process

For the system to function, transactions must be verified through consensus mechanisms where network participants validate each transaction using methods like Proof of Work or Proof of Stake. Once verified, transactions are grouped into blocks and added to the chain with network-wide agreement required for any modifications.

Expanding Beyond: Real-World Applications

This foundation enables diverse applications that extend far beyond cryptocurrencies. Financial services benefit from streamlined payments and increased transparency. Supply chains gain end-to-end tracking capabilities. Healthcare systems can securely manage patient records. Voting systems become more transparent and fraud-resistant. Smart contracts automate trustless transactions.

Facing Reality: Current Limitations

However, practical implementation reveals significant challenges. Scalability issues arise because processing many transactions is slow and energy-intensive. Regulatory uncertainties create adoption barriers. Privacy concerns emerge from the transparent nature of records. The beneficial immutability feature becomes problematic when incorrect data enters the system.

Looking Forward: Future Potential

Despite these challenges, the logical progression suggests that blockchain represents a transformative shift in data and transaction management. Addressing current limitations through continued research and innovation positions blockchain as a foundational technology for future digital systems.
```

## Conclusion

| Platform | Prompt Type      | Accuracy | Coherence | Simplicity | Speed | UX | Total (/25) |
| -------- | ---------------- | -------- | --------- | ---------- | ----- | -- | ----------- |
| ChatGPT  | Zero-shot        | 4        | 4         | 4          | 5     | 5  | 22          |
| ChatGPT  | Few-shot         | 5        | 5         | 5          | 4     | 5  | 24          |
| ChatGPT  | Chain-of-Thought | 5        | 5         | 4          | 3     | 5  | 22          |
| ChatGPT  | Role-based       | 5        | 5         | 5          | 4     | 5  | 24          |
| Gemini   | Zero-shot        | 3        | 3         | 3          | 5     | 4  | 18          |
| Gemini   | Few-shot         | 4        | 4         | 4          | 4     | 4  | 20          |
| Claude   | Chain-of-Thought | 5        | 5         | 5          | 4     | 4  | 23          |
| Claude   | Role-based       | 5        | 5         | 5          | 4     | 5  | 24          |

## Result 

ChatGPT and Claude perform best in summarization across prompting methods, with Chain-of-Thought and Role-Based giving the most accurate and audience-friendly results, while Gemini tends to be weaker for natural language.
