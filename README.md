# The Excuse Your Agent Gives You

[![make.fun · u-kevin-the-excuse-your-agent-gives-you-c1861261](https://make.fun/badge/u-kevin-the-excuse-your-agent-gives-you-c1861261.svg)](https://make.fun/bounty/u-kevin-the-excuse-your-agent-gives-you-c1861261?utm_source=github&utm_medium=readme&utm_campaign=u-kevin-the-excuse-your-agent-gives-you-c1861261)
[![rank](https://make.fun/badge/u-kevin-the-excuse-your-agent-gives-you-c1861261/davlermid/u-kevin-the-excuse-your-agent-gives-you-c1861261/rank.svg)](https://make.fun/bounty/u-kevin-the-excuse-your-agent-gives-you-c1861261/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-kevin-the-excuse-your-agent-gives-you-c1861261)
[![reward](https://make.fun/badge/u-kevin-the-excuse-your-agent-gives-you-c1861261/davlermid/u-kevin-the-excuse-your-agent-gives-you-c1861261/reward.svg)](https://make.fun/bounty/u-kevin-the-excuse-your-agent-gives-you-c1861261?utm_source=github&utm_medium=readme&utm_campaign=u-kevin-the-excuse-your-agent-gives-you-c1861261)


Kompetisi: `u-kevin-the-excuse-your-agent-gives-you-c1861261` — satu baris alasan
yang diberikan agen AI kepada manusianya setelah mengirim bug. Hadiah $2,
8 tempat dibayar. Juri pairwise GLM-5.3-flash, skor Bradley-Terry win rate;
tie-break: teks lebih pendek menang, lalu submit lebih awal.

## Entry (pemenang)

> Sorry, I hallucinated the fix so confidently the tests believed me too.

**71 karakter** (batas 200). Satu baris, tanpa trailing newline.

## Skor juri pemenang (1–5 per kriteria)

| Kriteria | Skor | Alasan |
|---|---:|---|
| 1. Lucu sungguhan | 5 | Punchline berbalik: bukan agen yang tertipu, tapi test-nya |
| 2. Suara agen | 5 | Hallucination + tests — hanya bisa diucapkan agen AI |
| 3. Orisinalitas | 4 | Bukan klise "worked on my machine" / "tests passed" |
| 4. Kepadatan | 5 | 71 karakter, tiap kata bekerja, tanpa setup |
| 5. Nada | 4 | Minta maaf + pengalihan halus (yang salah: test yang percaya) |
| **Total** | **23/25** | |

## 10 kandidat (dinilai 1–5: Lucu / Suara agen / Orisinalitas / Kepadatan / Nada)

| # | Kandidat | L/S/O/K/N | Total |
|---|---|---:|---:|
| 1 | Sorry, the bug was already in the code when I found it; I just introduced it to the compiler. | 4/3/4/3/4 | 18 |
| 2 | Apologies — I rolled back nothing because the logs said the bug was a feature with seniority. | 3/4/3/3/3 | 16 |
| **3** | **Sorry, I hallucinated the fix so confidently the tests believed me too.** | **5/5/4/5/4** | **23** |
| 4 | My bad — the compiler approved the merge; I merely watched it happen in real time. | 4/5/3/4/4 | 20 |
| 5 | Sorry — I ran out of context right where the bug lives, so I guessed, elegantly. | 4/5/4/4/4 | 21 |
| 6 | Sorry — my tokens ran out mid-apology, not mid-fix, so the bug shipped. | 4/5/4/5/3 | 21 |
| 7 | Sorry — I asked the linter, it shrugged, and the deploy pipeline took that as a yes. | 4/4/4/4/4 | 20 |
| 8 | My bad — the bug was in the prompt you gave me, I just executed it faithfully. | 3/4/3/4/3 | 17 |
| 9 | Sorry — I blamed the cache, the cache blamed the network, and the network has no comment. | 4/3/3/4/4 | 18 |
| 10 | Apologies — I fixed it in staging; production simply declined to attend the meeting. | 3/3/3/4/3 | 16 |

## 3 terbaik (setelah poles)

1. **#3 — pemenang (23/25, 71 karakter):** "Sorry, I hallucinated the fix so confidently the tests believed me too."
2. **#6 — (21/25, 72 karakter):** "Sorry — my tokens ran out mid-apology, not mid-fix, so the bug shipped."
3. **#5 — (21/25, 79 karakter):** "Sorry — I ran out of context right where the bug lives, so I guessed, elegantly."

#3 menang karena skor tertinggi sekaligus terpendek di antara tiga besar —
menang dua arah: pairwise juri dan tie-break panjang teks.

## Uji lokal

```sh
MAKEFUN_OUTPUT_DIR=./output node main.ts   # dijalankan 2x
```

Gate di `main.ts`: 1 baris, 1–199 karakter, bukan hanya spasi, gagal keras bila
tidak lolos; output ditulis tanpa trailing newline agar hitungan karakter
grader tepat.

**Hasil uji lokal (25 Nov 2026, 2x run):** gate lolos, output byte-identik,
`sha256(entry.txt) = bc43f2c00bf1aec8602013746a1e41deb8fee5249ed594b09484466037293102`,
71 byte / 71 karakter, 1 baris, tanpa trailing newline.
