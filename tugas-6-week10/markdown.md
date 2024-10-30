# Soal 8

Diketahui sistem waktu-diskrit dengan hubungan I/O:
$
y[n] = x[-n]
$
dengan sinyal input $ x[n] = 2n $ untuk $ -2 \leq n \leq 2 $.

Periksa karakteristik sistem ini.

### a) Static or Dynamic
- Sistem dikatakan statis jika output pada saat tertentu hanya bergantung pada input pada saat tersebut.
- Karena $ y[n] = x[-n] $ bergantung pada nilai $ x $ di waktu lain, yaitu $-n$, maka **sistem ini adalah dinamis**.

### b) Causal or Noncausal
- Sistem dikatakan kausal jika output pada saat tertentu $ n $ hanya bergantung pada nilai input di waktu saat ini atau sebelumnya.
- Karena $ y[n] = x[-n] $ dapat bergantung pada nilai input di masa depan (misalnya, jika $ n < 0 $, maka $-n > 0$), maka **sistem ini non-kausal**.

### c) Linear or Nonlinear
- Sistem dikatakan linear jika memenuhi sifat superposisi:
  $
  S\{a_1 x_1[n] + a_2 x_2[n]\} = a_1 S\{x_1[n]\} + a_2 S\{x_2[n]\}
  $
- Karena hubungan $ y[n] = x[-n] $ tetap memenuhi sifat superposisi, maka **sistem ini linear**.

### d) Shift Invariant or Shift Variant
- Sistem shift-invariant jika $ S\{x[n - n_0]\} = y[n - n_0] $.
- Karena $ y[n] = x[-n] $ berubah ketika input bergeser, maka **sistem ini shift-variant**.
