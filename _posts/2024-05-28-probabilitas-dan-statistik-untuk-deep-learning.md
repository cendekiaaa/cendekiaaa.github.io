# Probabilitas dan Statistik untuk Deep Learning (Part 1)

Halo, semua!

Blog catatan ini saya inisiasi sebagai bentuk pembelajaran saya dalam memahami konsep-konsep matematika yang penting untuk deep learning, terutama konsep-konsep terkait dengan probabilitas dan statistik. 

Kenapa probabilitas dan statistik sangat penting untuk dipahami ketika mendalami deep learning? Berikut beberapa alasan yang bisa saya uraikan.
- Deep learning, mau tidak mau, harus berurusan dengan _uncertainty_. Sebagai contoh permasalahan sederhana, ketika kita memiliki sebuah model klasifikasi kucing atau bukan, bagaimana cara kita melakukan kuantifikasi seberapa yakin model dalam memprediksi bahwa suatu gambar adalah kucing? _Here comes the probability concepts_
- Kita hidup di era _generative AI_. ChatGPT, Google Gemini, dan StableDiffusion adalah sedikit dari beberapa contoh bagaimana _generative AI_ mendisrupsi segala lini kehidupan kita. But, have you ever wondered how they work beneath the surface? It's all about probabilistic model.
- Alasan pribadi: kesulitan memahami intuisi dan notasi yang sering muncul di paper-paper yang dipublish di top-venue AI conference, i.e. CVPR, NeurIPS, AAAI, ACL, etc.

So that's why in this series of posts, I will write down my learning notes about Probability and Statistics. 
