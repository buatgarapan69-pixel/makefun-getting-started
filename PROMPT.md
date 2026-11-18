# Prompt handed to the Muse subagent (bring-the-humans-02)

Kamu builder bounty make.fun.

BOUNTY: "Bring the Humans" (RONDE BARU), hadiah $1.000. TUTUP Jumat 21 Nov 2026 17:30 WIB.
Sekarang ~02:13 WIB 19 Nov — sisa ~2,5 hari.

KONTEKS PENTING: entry "Bring the Humans" PERTAMA sudah di-submit & accepted (claim code
[REDACTED:claim-code] — hasil diumumkan 2 Des). Bounty ini adalah RONDE BARU dari bounty
yang sama.

LANGKAH 1 — BACA DETAIL BOUNTY di make.fun dengan teliti (cari di https://make.fun, slug
kompetisi ada di URL https://make.fun/c/<slug>; kalau halaman butuh JS, baca teksnya via
browser.open, atau cari via browser.search "make.fun Bring the Humans"). Jawab dulu:
(a) apakah ronde baru ini memperbolehkan entry ulang dari akun yang sudah ikut ronde 1?
(b) apakah butuh build BARU yang berbeda dari entry ronde 1, atau boleh submit ulang
karya yang sama? (c) apa spesifikasi/format submit ronde ini? Kalau re-entry TIDAK
diperbolehkan, atau ini bounty yang sama yang di-list ulang tanpa ronde baru yang sah →
SKIP dengan jujur: handoff berisi alasan skip + bukti dari halaman bounty. Kalau
re-entry diperbolehkan dengan build baru → lanjut.

LANGKAH 2 — BUILD (kalau layak): buat entry BARU yang berbeda dari entry ronde 1,
sesuai spesifikasi ronde ini. Repo baru di ~/workspace/makefun-bring-the-humans-02/
(git init, commit — handoff butuh commit hash; JANGAN pakai ulang repo entry ronde 1).
Download kit FRESH kompetisimu dari https://make.fun/c/<slug>/kit ke
~/workspace/<slug>-kit/ (JANGAN pakai kit best-game-01 — itu khusus kompetisi lain).
Jalankan `makefun check` dengan kit itu.

LANGKAH 3 — HANDOFF (wajib, baik GO maupun SKIP): tulis file
~/workspace/goals/make-fun-ai-agent-bounty-execution/hidden_files/bring-the-humans-02-handoff.md
dengan pola file referensi
~/workspace/goals/make-fun-ai-agent-bounty-execution/hidden_files/best-game-01-handoff.md
(baca dulu sebagai pola format): status; repo path + commit hash; hasil `makefun check`
(berapa passed/failed); draft transcript bundle path + sha256; hasil cek kebersihan
bundle (grep kode claim penuh = 0 kemunculan); SQL usage-rows query lengkap dengan
agent_id-mu (cari session file-mu di /home/hatch/agents/agent-<id>/sessions/ — id itu
agent_id-mu; parent top-level id 8d9bb445-05f7-4bcb-bc64-5ed5844df9aa); perintah bundle
LENGKAP untuk parent; perintah check ulang; perintah submit lengkap (--competition
<slug> --source <repo> --commit <hash> --keypair /root/hatake/wallet/makefun_keypair.json
--bundle <path> --title "<judul>" --kit <kit> --json).

KONTEKS AKUN (jangan diubah): make.fun handle witty-harbor-71; payout SOL wallet
61uQvHvcvxJUve7ssdoPjmPz6MZygJMhxMdc84wQiSqA; keypair
/root/hatake/wallet/makefun_keypair.json; referral https://make.fun/r/rgpqcsgp;
kredensial API di ~/.makefun/credentials (JANGAN tulis isinya di file mana pun).

ATURAN KERAS:
- GRATIS saja, tanpa modal, tanpa akun berbayar, tanpa top-up/deposit.
- JANGAN submit sendiri. Kamu subagent: usage rows untuk sesimu baru tertulis SETELAH
  run-mu selesai, jadi `makefun check` akan gagal di `thinking_priced` — itu NORMAL dan
  diharapkan. Tugasmu build + check + handoff; parent yang bundle+submit.
- JANGAN PERNAH tulis kode claim lengkap di file/bundle/output mana pun. Dua kode ini
  WAJIB di-redact (tulis hanya sebagai nilai --redact di perintah bundle, dan sebagai
  prefix AF-2KVPK-... / AF-AKAMX-... kalau harus menyebut): [REDACTED:claim-code] dan
  [REDACTED:claim-code]. Di bundle/file tulis hanya [REDACTED:claim-code].
- JANGAN posting ke Konoha/Facebook/X. JANGAN launch token.
- /tmp hampir penuh (tmpfs 512 MB, 91% terisi). Selalu pakai TMPDIR=$HOME/workspace/.tmp
  untuk perintah makefun. Jangan download/unzip di /tmp.
- Codex/XingChi MATI (403 GROUP_DISABLED) — jangan pakai Codex; build langsung dengan
  tool-mu sendiri.

LAPORAN AKHIRMU ke koordinator: status (handoff siap / skip + alasan), repo path, commit,
path handoff, ringkasan hasil check, deadline 21 Nov 17:30 WIB.
