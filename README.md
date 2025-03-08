
#Uninformed Search Algorithms
1. **Depth First Search (DFS)**  
DFS adalah algoritma pencarian yang menjelajahi graf atau pohon secara mendalam sebelum berpindah ke cabang lain. DFS menggunakan struktur data **stack** (baik secara eksplisit atau melalui rekursi). Algoritma ini cocok untuk eksplorasi mendalam tetapi bisa terjebak dalam siklus jika tidak dikendalikan.  

2. **Breadth First Search (BFS)**  
BFS adalah algoritma pencarian yang menjelajahi semua simpul pada satu tingkat sebelum berpindah ke tingkat berikutnya. BFS menggunakan **queue** sehingga menjamin jalur terpendek dalam graf tak berbobot. Algoritma ini cocok untuk pencarian solusi optimal tetapi memerlukan lebih banyak memori dibanding DFS.  

3. **Uniform Cost Search (UCS)**  
UCS adalah varian BFS yang mempertimbangkan bobot atau biaya lintasan. UCS menggunakan **priority queue** untuk selalu mengeksplorasi simpul dengan biaya terendah terlebih dahulu. UCS menjamin menemukan jalur dengan biaya minimum tetapi kurang efisien pada graf besar.

#Informed Search Algorithms
1. **Greedy Search**  
Greedy Search adalah algoritma pencarian yang selalu memilih langkah dengan estimasi terbaik berdasarkan **heuristic function (h(n))** tanpa mempertimbangkan biaya sebelumnya. Meskipun cepat, algoritma ini tidak menjamin solusi optimal karena bisa terjebak dalam **local optimum**.  

2. **A* Tree Search**  
A* Tree Search menggunakan fungsi evaluasi **f(n) = g(n) + h(n)**, di mana **g(n)** adalah biaya dari awal ke node saat ini dan **h(n)** adalah estimasi biaya ke tujuan. Dalam versi **tree search**, algoritma tidak menyimpan riwayat node yang telah dikunjungi, sehingga bisa mengunjungi node yang sama berulang kali.  

3. **A* Graph Search**  
A* Graph Search mirip dengan A* Tree Search tetapi menggunakan **closed list** untuk menyimpan node yang sudah dikunjungi, sehingga menghindari eksplorasi ulang. Ini menjadikannya lebih efisien dan optimal dibanding A* Tree Search, terutama dalam graf dengan banyak jalur menuju node yang sama.
