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
1.Select a 500-word article on "The Basics of Blockchain Technology."
2.Open Different AI Tools.
3.Apply the Zero-shot prompt and generate the summary.
4.Apply the Few-shot prompt and generate the summary.
5.Apply the Chain-of-Thought prompt and generate the summary.
6.Apply the Role-based prompt and generate the summary.
7.Compare all summaries based on accuracy, coherence, simplicity, speed, and user experience.
8.Record the observations in a comparison table.
9.Identify the prompting technique that produces the best summary.

## AI Tools

CHATGPT:

Prompts Used
1. Zero-shot Prompt

Summarize the following 500-word article on "The Basics of Blockchain Technology" in about 100 words using simple language suitable for undergraduate students.

2. Few-shot Prompt

Example:
Original: Artificial Intelligence enables computers to perform tasks requiring human intelligence...

Summary: AI allows computers to perform human-like tasks such as learning and problem-solving.

Now summarize the following article on "The Basics of Blockchain Technology" in the same style using about 100 words.

3. Chain-of-Thought Prompt

Read the article carefully. First identify the main ideas, then remove unnecessary details, organize the important points logically, and finally write a clear summary in about 100 words suitable for undergraduate students.

4. Role-based Prompt

You are an educational content writer preparing study material for undergraduate students. Summarize the following article on "The Basics of Blockchain Technology" in simple language using about 100 words.

GEMINI:

1. Zero-Shot Prompting
The Prompt: "Summarize the basics of blockchain technology."

Gemini's Output:

Blockchain is a decentralized, distributed ledger technology that securely records transactions across a network of computers (nodes). Instead of relying on a central authority like a bank, it groups data into "blocks" that are chained together chronologically using cryptographic hashes. Once a block is added, it cannot be altered without changing all subsequent blocks and gaining network consensus. This makes blockchain highly secure, transparent, and resistant to fraud, serving as the foundational technology for cryptocurrencies like Bitcoin and enabling applications in supply chain, finance, and beyond.

2. Few-Shot Prompting
The Prompt: "Here is a summary of Machine Learning: 'Machine learning is a branch of AI where computers learn from data without explicit programming. Key components include training data, algorithms, and models.' Using a similar format, summarize the basics of blockchain technology."

Gemini's Output:

Blockchain is a branch of decentralized computing where transactions are securely recorded across a network without a central authority.
Key components include:

Distributed Ledger: The shared database accessible to all network participants.

Cryptographic Hashes: The security mechanism that links data blocks together immutably.

Consensus Mechanisms: The rules (like Proof of Work) the network uses to verify and agree on new transactions.

3. Chain-of-Thought (CoT) Prompting
The Prompt: "First, identify the core definition of a blockchain. Next, explain step-by-step how a transaction is verified and added to the chain. Finally, summarize why this matters for security. Combine this into a short summary."

Gemini's Output:

At its core, a blockchain is a digital, decentralized public ledger. When a user requests a transaction, it is broadcasted to a peer-to-peer network of computers known as nodes. These nodes use complex algorithms to validate the transaction's status. Once verified, the transaction is combined with other recent transactions to create a new "block" of data. This new block is permanently and immutably added to the existing blockchain using cryptographic hashing. This step-by-step process matters because it eliminates single points of failure; altering any data requires rewriting the entire chain and overpowering the network, making the system virtually tamper-proof.

4. Role-Based Prompting
The Prompt: "You are an expert content curator for an undergraduate educational platform. Summarize a 500-word technical article on the basics of blockchain technology. Make it highly engaging, easy to digest for students with no tech background, and emphasize the main takeaways."
Gemini's Output:

Blockchain in a Nutshell: The End of the Middleman

Imagine a shared Google Doc that thousands of people can view and add to, but absolutely no one can erase or secretly edit. That’s the basic idea behind blockchain!

Instead of trusting a central authority (like a bank or a government) to keep track of transactions, blockchain uses a global network of computers to maintain a single, digital ledger.

GROK:

1. Zero-shot
Prompt used:
“Summarize the following 500-word technical article on The Basics of Blockchain Technology for undergraduate students. Keep it accurate, coherent, simple, and concise.”
Summary:
Blockchain is a decentralized digital ledger that records transactions across many computers so no single party controls the data. Information is stored in linked “blocks.” Each block contains transaction data, a timestamp, and a cryptographic hash of the previous block, forming an unbreakable chain. Once added, data cannot be altered without changing every subsequent block, which the network would reject. Consensus mechanisms (such as Proof of Work or Proof of Stake) let participants agree on the valid state of the ledger without a central authority. This design provides transparency, security, and trust for uses like cryptocurrency, supply-chain tracking, and secure record-keeping.
2. Few-shot
Prompt used:
(Provided two short example summaries of other technical topics in simple student-friendly language, then asked for the same style on the blockchain article.)
Summary:
Think of blockchain as a shared notebook that many people keep identical copies of. Every new page (called a block) lists recent transactions, is time-stamped, and is locked with a unique digital fingerprint (hash) that also points to the previous page. Because every copy must match, no one can secretly change an old entry—the whole network would notice. Computers agree on new pages through rules called consensus (like Proof of Work or Proof of Stake). The result is a transparent, tamper-proof record that doesn’t need a bank or other middleman. Students can use this idea to understand cryptocurrencies, digital contracts, and secure data sharing.
3. Chain-of-thought
Prompt used:
“Summarize the article step by step. First identify the core definition, then the key components (blocks, hashing, chain, consensus), then the main benefits and simple real-world uses. Finally write a short coherent paragraph suitable for undergraduates.”
Summary (reasoning + final output):

Core idea → decentralized, shared ledger.
Building blocks → data + timestamp + previous hash → immutable chain.
Agreement method → consensus algorithms.
Benefits → no single point of failure, transparency, security.
Student-friendly uses → crypto, tracking goods, digital certificates.

Final summary:
Blockchain technology creates a shared digital ledger maintained by many computers instead of one central authority. Transactions are grouped into blocks; each block is cryptographically linked to the one before it by a unique hash, making the history almost impossible to alter. Network participants reach agreement through consensus mechanisms such as Proof of Work or Proof of Stake. Because every participant holds a copy and changes require network-wide approval, the system is transparent and resistant to tampering. For undergraduates, this means a practical foundation for understanding cryptocurrencies, secure supply chains, and trusted digital records—without needing a bank or other intermediary.
4. Role-based
Prompt used:
“You are a patient university teaching assistant explaining technical concepts to first-year undergraduates. Summarize the article on The Basics of Blockchain Technology in clear, simple language, avoiding jargon where possible and defining any necessary terms.”
Summary:
Imagine a notebook that hundreds of people all keep identical copies of. Every time someone wants to add a new entry (a transaction), it gets written on a new page called a “block.” That page also gets a special digital lock (a hash) that includes a fingerprint of the previous page, so the pages form an unbreakable chain—hence “blockchain.”
Because everyone has the same notebook, no single person can secretly erase or change an old entry; the others would immediately see the mismatch. The group decides which new pages are valid by following clear rules (called consensus).
The big advantages are that you don’t need a central boss (like a bank), the record is public and permanent, and it’s very hard to cheat. This is why blockchain is used for digital money, tracking products from factory to store, and keeping important certificates safe.
That’s the basic idea in everyday terms.

PERPLEXITY:

A. Zero-shot

Summarize the following 500-word article on “The Basics of Blockchain Technology” in 3–4 clear sentences for undergraduate students. Keep it accurate, simple, and coherent:

B. Few-shot

You will summarize short technical articles for undergraduate students. Here are two examples of good summaries:

Example 1 input: [short sample text]
Example 1 summary: [2–3 sentence summary]

Example 2 input: [short sample text]
Example 2 summary: [2–3 sentence summary]

Now summarize the following article in the same style (3–4 sentences, simple, accurate):


C. Chain-of-thought (hidden reasoning, output only summary)

You are helping undergraduate students understand a technical article. First, think step by step about the key concepts, then produce only a final 3–4 sentence summary that is accurate, simple, and coherent. Do not show your reasoning, only the summary.


D. Role-based

You are an experienced undergraduate teaching assistant in computer science. Your task is to summarize a 500-word technical article on blockchain for first-year students who are new to the topic. Write a 3–4 sentence summary that is accurate, easy to understand, and logically coherent.

## COMPARISON

<img width="923" height="420" alt="Screenshot 2026-07-30 232743" src="https://github.com/user-attachments/assets/9839e359-e1de-401c-ad0e-d950cd336e3c" />

<img width="912" height="707" alt="Screenshot 2026-07-30 232847" src="https://github.com/user-attachments/assets/f334436a-4285-409b-8740-3e74c2365cf9" />



## Result

Across all four platforms, the role-based and chain-of-thought prompts consistently produced the most accurate and coherent summaries, since role-based prompting encouraged simpler analogies (e.g., the "shared notebook" explanation) and CoT prompting forced structured, logically ordered reasoning before the final summary. Zero-shot prompts were the fastest and most concise but occasionally lacked depth. Few-shot prompts were the least consistent, since output quality depended heavily on the quality of the examples provided. Overall, Grok's role-based summary scored highest, balancing accuracy, simplicity, and engagement, making Grok + role-based prompting the best combination for this summarization task.


