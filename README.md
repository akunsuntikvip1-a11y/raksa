<!doctype html>
<html lang="id">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>LENGKAP BUKU SMP/MTS | SAM/SMK yoxx 🐰</title>
  <style>
    :root{
      --bg1: linear-gradient(135deg,#0f172a,#2a2a72);
      --accent: linear-gradient(90deg,#ff7a18,#af002d,#319197);
      --card-bg: rgba(255,255,255,0.06);
      --glass: rgba(255,255,255,0.03);
    }
    html,body{height:100%;margin:0;font-family:Inter,ui-sans-serif,system-ui,Segoe UI,Roboto,"Helvetica Neue",Arial}
    body{background:var(--bg1);color:#e6eef8;display:flex;align-items:center;justify-content:center;padding:20px}

    /* landscape container */
    .wrap{width:100%;max-width:1400px;height:80vh;display:grid;grid-template-columns:1fr 420px;gap:22px;align-items:stretch}

    .left{padding:28px;border-radius:18px;background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));box-shadow:0 8px 30px rgba(2,6,23,0.6);transform:skewX(-6deg)}
    .right{padding:22px;border-radius:18px;background:var(--card-bg);backdrop-filter:blur(6px);box-shadow:inset 0 0 0 1px rgba(255,255,255,0.02);transform:skewX(-6deg)}

    header{display:flex;justify-content:space-between;align-items:center}
    h1{margin:0;font-size:20px;letter-spacing:0.6px}
    .by{font-size:13px;opacity:0.9}

    .keywords{margin-top:20px;display:flex;gap:14px}
    .key{padding:14px 18px;border-radius:12px;background:linear-gradient(90deg, rgba(255,255,255,0.03), rgba(255,255,255,0.01));cursor:pointer;user-select:none;flex:1;text-align:center;transition:transform .14s ease, box-shadow .14s}
    .key:hover{transform:translateY(-6px);box-shadow:0 8px 24px rgba(0,0,0,0.35)}
    .key.active{background:var(--accent);color:#091021;font-weight:700}

    .controls{margin-top:22px;display:grid;grid-template-columns:1fr 1fr;gap:14px}
    select,input[type=number]{width:100%;padding:12px;border-radius:10px;border:0;background:var(--glass);color:inherit}

    .subjects{margin-top:18px;display:grid;grid-template-columns:repeat(2,1fr);gap:12px}
    .subject{padding:10px;border-radius:10px;background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));cursor:pointer;transform:skewX(6deg);user-select:none}

    .searchRow{margin-top:18px;display:flex;gap:10px}
    .btn{padding:12px 16px;border-radius:10px;border:0;cursor:pointer}
    .btn.primary{background:linear-gradient(90deg,#ff7a18,#af002d);color:white;font-weight:700}
    .btn.ghost{background:transparent;border:1px solid rgba(255,255,255,0.06);color:inherit}

    .help{margin-top:14px;font-size:13px;opacity:0.8}

    /* right panel */
    .right h2{margin:0 0 12px 0}
    .panel{padding:12px;border-radius:10px;background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));}
    .settings{display:flex;gap:8px;align-items:center}
    .gear{cursor:pointer;padding:8px;border-radius:8px}

    footer{position:fixed;left:18px;bottom:12px;font-weight:600}
    footer a{color:rgb(255,120,100);text-decoration:underline}

    /* small responsive */
    @media (max-width:880px){.wrap{grid-template-columns:1fr;height:auto}.left{transform:none}.right{transform:none}}
  </style>
</head>
<body>
  <div class="wrap">
    <main class="left">
      <header>
        <div>
          <h1>LENGKAP BUKU SMP/MTS | SAM/SMK yoxx 🐰</h1>
          <div class="by">by : yoga 🐰</div>
        </div>
        <div class="gear" title="Pengaturan" id="openSettings">⚙️</div>
      </header>

      <section class="keywords" aria-hidden>
        <div class="key" data-mode="materi">materi "jenis kelas" "tahun ajaran"</div>
        <div class="key" data-mode="rangkuman">🔥 rangkuman "jenis kelas" "tahun ajaran"</div>
      </section>

      <div class="controls">
        <div>
          <label style="font-size:13px;opacity:0.9">Pilih Mata Pelajaran</label>
          <select id="subjectSelect">
            <option value="MTK">1 — Matematika [Mtk]</option>
            <option value="BSD">2 — Bahasa Sunda [b Sunda]</option>
            <option value="BIND">3 — Bahasa Indonesia [b indo]</option>
            <option value="BING">4 — Bahasa Inggris [b inggris]</option>
            <option value="PA">5 — Pendidikan Agama [isi manual]</option>
            <option value="IPA">6 — Ilmu Pengetahuan Alam [IPA]</option>
            <option value="IPS">7 — Ilmu Pengetahuan Sosial [IPS]</option>
            <option value="TIK">8 — Teknik Informatika [TIK]</option>
            <option value="PJOK">9 — Pendidikan Jasmani, Olahraga & Kesehatan [PJOK]</option>
            <option value="SB">10 — Seni Budaya</option>
            <option value="PKN">11 — Pendidikan Kewarganegaraan [PKN]</option>
          </select>
        </div>
        <div>
          <label style="font-size:13px;opacity:0.9">Pilih Kelas</label>
          <select id="classSelect">
            <option value="1">1</option>
            <option value="2">2</option>
            <option value="3">3</option>
            <option value="4">4</option>
            <option value="5">5</option>
            <option value="6">6</option>
            <option value="7">7</option>
            <option value="8">8</option>
            <option value="9">9</option>
            <option value="10">10</option>
            <option value="11">11</option>
            <option value="12">12</option>
          </select>
        </div>
      </div>

      <div style="margin-top:12px;display:flex;gap:12px;align-items:center">
        <div style="flex:1">
          <label style="font-size:13px;opacity:0.9">Tahun Ajaran (masukan manual)</label>
          <input id="yearInput" type="text" placeholder="contoh: 2024/2025" />
        </div>
        <div style="width:160px">
          <label style="font-size:13px;opacity:0.9">Mode Pencarian</label>
          <select id="modeSelect">
            <option value="materi">materi</option>
            <option value="rangkuman">rangkuman</option>
          </select>
        </div>
      </div>

      <div id="agamaWrap" style="display:none;margin-top:12px">
        <label style="font-size:13px;opacity:0.9">Isi Nama Agama (untuk Pendidikan Agama)</label>
        <input id="agamaInput" type="text" placeholder="Contoh: Islam / Kristen / Katolik / Hindu / Buddha / Konghucu" />
      </div>

      <div class="subjects" style="margin-top:18px">
        <!-- quick subject tiles (mirrored to select) -->
        <div class="subject" data-val="MTK">Matematika [Mtk]</div>
        <div class="subject" data-val="BSD">Bahasa Sunda [b Sunda]</div>
        <div class="subject" data-val="BIND">Bahasa Indonesia [b indo]</div>
        <div class="subject" data-val="BING">Bahasa Inggris [b inggris]</div>
        <div class="subject" data-val="PA">Pendidikan Agama [isi manual]</div>
        <div class="subject" data-val="IPA">Ilmu Pengetahuan Alam [IPA]</div>
        <div class="subject" data-val="IPS">Ilmu Pengetahuan Sosial [IPS]</div>
        <div class="subject" data-val="TIK">Teknik Informatika [TIK]</div>
        <div class="subject" data-val="PJOK">PJOK</div>
        <div class="subject" data-val="SB">Seni Budaya</div>
        <div class="subject" data-val="PKN">PKN</div>
      </div>

      <div class="searchRow">
        <button class="btn primary" id="searchBtn">Cari di Google</button>
        <button class="btn ghost" id="clearBtn">Clear</button>
      </div>

      <div class="help">Langkah: 1) Pilih kata kunci (materi / rangkuman). 2) Pilih mata pelajaran. 3) Pilih kelas. 4) Masukkan tahun ajaran. 5) Klik <strong>Cari di Google</strong>.</div>

    </main>

    <aside class="right">
      <h2>Pengaturan & Info</h2>
      <div class="panel">
        <div style="display:flex;justify-content:space-between;align-items:center">
          <div>
            <div style="font-size:14px;font-weight:700">Pengaturan Pemutar & Report</div>
            <div style="font-size:13px;opacity:0.85;margin-top:6px">Klik gear di kiri atas untuk buka opsi lagu dan report.</div>
          </div>
          <div style="font-size:12px;opacity:0.85">Versi 1.0</div>
        </div>

        <hr style="margin:12px 0;border:none;border-top:1px solid rgba(255,255,255,0.03)" />

        <div style="font-size:13px;">Daftar Mata Pelajaran (singkatan dalam tanda kurung)</div>
        <ul style="opacity:0.9;margin-top:8px">
          <li>Matematika [Mtk]</li>
          <li>Bahasa Sunda [b Sunda]</li>
          <li>Bahasa Indonesia [b indo]</li>
          <li>Bahasa Inggris [b inggris]</li>
          <li>Pendidikan Agama [isi manual]</li>
          <li>IPA, IPS, TIK, PJOK, Seni Budaya, PKN</li>
        </ul>

      </div>

      <div style="height:12px"></div>

      <div class="panel">
        <div style="font-size:13px;font-weight:700">Petunjuk Cepat</div>
        <ol style="margin-top:8px;opacity:0.9">
          <li>Pilih mode (materi / rangkuman).</li>
          <li>Pilih mata pelajaran atau klik cepat di daftar.</li>
          <li>Isi kelas dan tahun ajaran.</li>
          <li>Klik Cari untuk membuka hasil pencarian Google di tab baru.</li>
        </ol>
      </div>

    </aside>
  </div>

  <!-- bottom-left support link -->
  <footer>Yuk support yox : <a href="https://saweria.co/yoxxsuport" target="_blank" rel="noopener">klik ini</a></footer>

  <!-- settings modal (hidden) -->
  <div id="settingsModal" style="position:fixed;left:50%;top:50%;transform:translate(-50%,-50%) scale(0.9);min-width:320px;background:rgba(4,8,23,0.96);padding:18px;border-radius:12px;box-shadow:0 30px 80px rgba(2,6,23,0.8);display:none;z-index:120">
    <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:10px">
      <div style="font-weight:800">Pengaturan Lagu & Report</div>
      <div style="cursor:pointer" id="closeSettings">✖️</div>
    </div>
    <div style="margin-top:8px">
      <div style="font-size:13px;margin-bottom:8px">Daftar lagu (klik untuk putar):</div>
      <div style="display:flex;gap:8px;flex-direction:column">
        <button class="btn ghost" data-src="http://b.top4top.io/m_3488zlv381.mp3">Lagu default (klik untuk putar)</button>
        <!-- tambahkan placeholder lagu lain jika perlu -->
      </div>
      <div style="margin-top:12px;font-size:13px">Report / Halaman lain: <a href="https://lynk.id/yoxxreal/page/yoxx" target="_blank" rel="noopener">https://lynk.id/yoxxreal/page/yoxx</a></div>
    </div>
  </div>

  <audio id="player" src="" preload="none"></audio>

  <script>
    // Elements
    const keys = document.querySelectorAll('.key');
    const modeSelect = document.getElementById('modeSelect');
    const subjectSelect = document.getElementById('subjectSelect');
    const classSelect = document.getElementById('classSelect');
    const yearInput = document.getElementById('yearInput');
    const searchBtn = document.getElementById('searchBtn');
    const clearBtn = document.getElementById('clearBtn');
    const subjectTiles = document.querySelectorAll('.subject');
    const agamaWrap = document.getElementById('agamaWrap');
    const agamaInput = document.getElementById('agamaInput');

    // settings modal
    const openSettings = document.getElementById('openSettings');
    const settingsModal = document.getElementById('settingsModal');
    const closeSettings = document.getElementById('closeSettings');
    const player = document.getElementById('player');

    // default active
    let activeMode = 'materi';
    document.querySelector('.key[data-mode="materi"]').classList.add('active');

    keys.forEach(k=>k.addEventListener('click',()=>{
      keys.forEach(x=>x.classList.remove('active'));
      k.classList.add('active');
      activeMode = k.dataset.mode;
      modeSelect.value = activeMode;
    }));

    // subject tiles quick select
    subjectTiles.forEach(tile=>{
      tile.addEventListener('click',()=>{
        const v = tile.dataset.val;
        subjectSelect.value = v;
        if(v === 'PA') { agamaWrap.style.display = 'block'; } else { agamaWrap.style.display = 'none'; }
      });
    });

    subjectSelect.addEventListener('change', ()=>{
      if(subjectSelect.value === 'PA') agamaWrap.style.display = 'block'; else agamaWrap.style.display = 'none';
    });

    clearBtn.addEventListener('click', ()=>{
      yearInput.value=''; agamaInput.value='';
      subjectSelect.selectedIndex = 0; classSelect.selectedIndex = 0; modeSelect.value='materi';
      keys.forEach(x=>x.classList.remove('active'));
      document.querySelector('.key[data-mode="materi"]').classList.add('active');
      agamaWrap.style.display='none';
    });

    function buildQuery(){
      const mode = modeSelect.value; // materi or rangkuman
      let subjectText = subjectSelect.options[subjectSelect.selectedIndex].text;
      // if Pendidikan Agama, use agamaInput if filled
      if(subjectSelect.value === 'PA' && agamaInput.value.trim() !== ''){
        subjectText = 'Pendidikan Agama ' + agamaInput.value.trim();
      }
      const classText = classSelect.value;
      const year = yearInput.value.trim();

      // clean subjectText to remove numeric prefix
      subjectText = subjectText.replace(/^\d+\s+—\s+/,'');

      let q = '';
      if(mode === 'materi'){
        q = `${subjectText} kelas ${classText} ${year} materi`;
      } else {
        q = `rangkuman ${subjectText} kelas ${classText} ${year}`;
      }
      return encodeURIComponent(q.trim());
    }

    searchBtn.addEventListener('click', ()=>{
      const q = buildQuery();
      // open google search in new tab (will open in user's default browser, likely Chrome on Android if set)
      const url = `https://www.google.com/search?q=${q}`;
      window.open(url,'_blank');
    });

    // settings modal behavior: clicking gear opens modal and plays default song
    openSettings.addEventListener('click', ()=>{
      settingsModal.style.display = 'block';
      settingsModal.style.transform = 'translate(-50%,-50%) scale(1)';
      // auto play default song immediately as requested
      const defaultSong = 'http://b.top4top.io/m_3488zlv381.mp3';
      player.src = defaultSong;
      player.play().catch(()=>{
        // some browsers block autoplay; in that case set src and show play button
      });
    });
    closeSettings.addEventListener('click', ()=>{
      settingsModal.style.display = 'none';
      player.pause(); player.currentTime = 0; player.src='';
    });

    // clicking song buttons in modal
    document.querySelectorAll('#settingsModal button[data-src]').forEach(btn=>{
      btn.addEventListener('click', ()=>{
        const src = btn.dataset.src;
        if(player.src !== src){ player.src = src; }
        player.play().catch(()=>{});
      });
    });

    // small UX: pressing Enter in year input triggers search
    yearInput.addEventListener('keydown', (e)=>{ if(e.key === 'Enter') searchBtn.click(); });

  </script>
</body>
</html>
