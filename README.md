# Tugas-Hari-1-Pekan-3
sanbarcode
<h2>Soal 1: Pemahaman Component Matplotlib</h2>

- Jelaskan apa itu Figure
- Jelaskan apa itu Axis

jawab:
Figure adalah window atau page atau halaman dalam objek visual. kalau kita ngegambar di kertas, maka kertas tersebutlah yang di namakan figure.
Axis adalah suatu area di dalam figure dimana data akan di plot. di dalam Axis juga terdapat berbagai macam komponen lagi seperti x-axis, y-axis, dan lain sebagainya.

<h2>Soal 2: Membuat Component Figure dan Axis</h2>

- Buatlah Figure dan Axis kosong tanpa Data
- Plot data di bawah ini dengan 2 cara, yaitu dengan membuat figure dan axis secara explicit dan Implicit

import numpy as np
import matplotlib.pyplot as plt

x = np.linspace(0, 20, 100)
y = np.cos(x/2)

fig = plt.figure()
ax = fig.add_subplot()
plt.show()

fig = plt.figure()
ax = fig.add_subplot()
ax.plot(x, y)
plt.show()

Exected Output:

![alt text](https://drive.google.com/uc?id=1mq8HMFwz5GlTH_SPAFnXZZ8KnBWBC9d3)

Expected Output:

![alt text](https://drive.google.com/uc?id=156xwVvDgShvIPBefimXg18zfFjz_SQ8X)

<h2>Soal 3: Memasukan multiple data ke dalam satu axis</h2>

- Plot ketiga data berikut ke dalam satu axis, dan gunakan seaborn style
- save data tersebut dengan nama file bebas

x = np.linspace(0, 20, 100)
y = np.cos(x/2)
y2 = np.sin(x)
y3 = np.sin(2*x)

fig, ax = plt.subplots()
ax.plot(x, y)
ax.plot(x, y2)
ax.plot(x, y3)
plt.show()

Expected Output:

![alt text](https://drive.google.com/uc?id=1EnJDnXuJ97NZ9EcKQWRaGCD7-LroZ-Gj)
