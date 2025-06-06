# Gujarati-to-Marathi-Machine-Translation-
Gujarati-to-Marathi Neural  Machine Translation via  English Pivot and NLLB-200  Fine-Tuning &lt;br>

Machine translation between low‐resource Indic languages is difficult because of scarce direct 
parallel data and script differences. This project builds a Gujarati to Marathi translator by 
combining a pivot‐based corpus construction (via English) with transfer‐learning–based 
fine‐tuning of a multilingual transformer. Instead of relying on limited or noisy Guj–Mr parallel 
texts, we use the publicly available WMT24 English–Gujarati and English–Marathi splits. By 
aligning on identical English sentences, we effectively make a medium‐sized Guj–Mr corpus. 
This approach rids our need of annotating new data. We then fine‐tune a 600 million–parameter 
distilled variant of the NLLB‐200 (No Language Left Behind) Seq2Seq model, which is 
pretrained on 200+ languages, including Gujarati (Gujr–Gujr script) and Marathi (Mar–Deva 
script). The resulting system demonstrates high lexical fidelity (for named entities) and 
grammatical adequacy (judged qualitatively).  
This project applies the following concepts/techniques: Subword Tokenization (SentencePiece), 
Transformer Encoder–Decoder with Attention, Multilingual Transfer Learning, 
Sequence‐to‐Sequence Training & Teacher Forcing, Pivot‐Based Data Augmentation, Data 
Collation & Efficient GPU Batching, Forced Language Tokens & Beam Search, Tokenization 
Strategies & Unicode Handling, Qualitative Error Analysis. 
