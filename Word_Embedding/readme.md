
  # 🧠 Word Embedding Techniques in NLP

  This project demonstrates how text is converted into **dense vector representations** using Keras Embedding Layers — moving beyond sparse representations like One-Hot Encoding and Bag-of-Words. The focus is on understanding how embeddings allow models to capture **semantic meaning**, **context**, and **relationships** between words.

-----

  ## 📌 Project Overview
  Implemented pipeline:
  - One-Hot Encoding → Integer Token Mapping
  - Vocabulary Building
  - Sequence Padding (equal input length)
  - Keras Embedding Layer (trainable vectors)
  - Extracting learned embeddings for interpretation

  These representations form the core of modern NLP architectures like RNNs, LSTMs, GRUs, and Transformers.

-----

  ## 🧠 NLP Embedding Pipeline
  Raw Text → Tokenization → Integer Mapping → Padding → Embedding Layer → Dense Vector Output

-----

  ## 🛠️ Features Implemented
  - One-Hot Encoding
  - Padding sequences
  - Trainable Embedding matrix
  - Embedding extraction for analysis
  - Understanding vector shapes & semantics

-----

  ## 🤖 Core Model Code
  from tensorflow.keras.models import Sequential
  from tensorflow.keras.layers import Embedding

  model = Sequential()
  model.add(Embedding(input_dim=vocab_size, output_dim=10, input_length=sent_length))
  model.compile(optimizer='adam', loss='mse')
  model.summary()

  **Output Shape:** (None, sent_length, 10)

-----

  ## 🧠 Key Concept Highlights
  - Sparse vectors → limited meaning
  - Dense vectors → semantic representation
  - Similar words → closer vector space distance
  - Required for all neural NLP

-----

  ## 📊 Example Output
  Input: "the glass of milk"
  Output Sample:
  [ [0.0398, -0.0071, 0.0258, ...],
    [0.0283,  0.0295, 0.0313, ...],
    [0.0398, -0.0071, 0.0258, ...] ]

  *(Values vary per training — embeddings are learned)*

-----

  ## 🛠️ Tech Stack
  Python · TensorFlow/Keras · NumPy · Google Colab

-----

  ## 🚀 How to Run
  pip install tensorflow numpy
  Run notebook / .py file to view embedding model output and summary.

-----

  ## 🎯 Learning Outcomes
  - Why embeddings matter in NLP
  - Dense vectors vs sparse representations
  - Semantic similarity via vector math
  - Foundation for advanced NLP models

-----

  ## 👩‍💻 Author
  **Shreya Gupta** — Aspiring AI/ML Engineer | NLP Enthusiast

-----

  ## ✨ Closing Note
  *Text becomes data. Data becomes meaning. Embeddings are where NLP begins.* 🚀

