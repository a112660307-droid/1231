<!doctype html>
<html lang="zh-TW">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>個人履歷｜Portfolio</title>

  <!-- Bootstrap -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/css/bootstrap.min.css" rel="stylesheet"
    integrity="sha384-sRIl4kxILFvY47J16cr9ZwB07vP4J8+LH7aKQnuqkuIAvNWLzeN8tE5YBujZqJLB" crossorigin="anonymous">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/js/bootstrap.bundle.min.js"
    integrity="sha384-FKyoEForCGlyvwx9Hj09JcYn3nv7wiPVlz7YYwJrWVcXK/BmnVDxM+D2scQbITxI" crossorigin="anonymous"></script>

  <style>
    /* 視覺：柔和背景 + 霧面卡片 + 漸層標題 */
    body {
      background: radial-gradient(1200px 500px at 10% 0%, rgba(13,110,253,.18), transparent 60%),
                  radial-gradient(900px 500px at 90% 10%, rgba(25,135,84,.16), transparent 55%),
                  #f6f7fb;
    }
    .glass {
      background: rgba(255,255,255,.78);
      border: 1px solid rgba(255,255,255,.65);
      backdrop-filter: blur(8px);
      -webkit-backdrop-filter: blur(8px);
    }
    .hero-badge {
      border: 1px solid rgba(0,0,0,.08);
      background: rgba(255,255,255,.75);
    }
    .section-title {
      letter-spacing: .02em;
    }
    .icon-dot {
      width: .55rem;
      height: .55rem;
      border-radius: 999px;
      display: inline-block;
      margin-right: .5rem;
      background: currentColor;
      opacity: .75;
    }
    .skill-pill {
      border: 1px solid rgba(0,0,0,.08);
      background: rgba(255,255,255,.85);
    }
    .timeline {
      position: relative;
      padding-left: 1.25rem;
    }
    .timeline:before {
      content: "";
      position: absolute;
      left: .35rem;
      top: .25rem;
      bottom: .25rem;
      width: 2px;
      background: rgba(0,0,0,.08);
    }
    .timeline-item {
      position: relative;
      padding: .6rem 0 .6rem 0;
    }
    .timeline-item:before {
      content: "";
      position: absolute;
      left: -.95rem;
      top: 1.1rem;
      width: .7rem;
      height: .7rem;
      border-radius: 999px;
      background: #0d6efd;
      box-shadow: 0 0 0 4px rgba(13,110,253,.15);
    }
  </style>
</head>

<body>
  <!-- NAVBAR（簡潔高級感） -->
  <nav class="navbar navbar-expand-lg sticky-top glass shadow-sm">
    <div class="container py-1">
      <!-- 【可替換：你的名字 / Logo】 -->
      <a class="navbar-brand fw-bold" href="#">
        <!-- 你也可以放小圖示：<img src="images/logo.png" width="24" class="me-2"> -->
        【你的名字｜Portfolio】
      </a>

      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#nav"
        aria-controls="nav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse" id="nav">
        <ul class="navbar-nav ms-auto gap-1">
          <!-- 這些是頁內錨點，不需要其他頁也可以做出「多區塊」效果 -->
          <li class="nav-item"><a class="nav-link" href="#about">關於我</a></li>
          <li class="nav-item"><a class="nav-link" href="#skills">專長技能</a></li>
          <li class="nav-item"><a class="nav-link" href="#experience">經歷</a></li>
          <li class="nav-item"><a class="nav-link" href="#projects">作品</a></li>
          <li class="nav-item"><a class="nav-link" href="#contact">聯絡</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- HERO（照片 + 一句定位 + 行動按鈕） -->
  <header class="py-5">
    <div class="container">
      <div class="row g-4 align-items-center">
        <div class="col-lg-4 text-center">
          <!-- 【可替換：大頭照】放到 images/profile.jpg -->
          <img src="images/profile.jpg" alt="個人照片" class="img-fluid rounded-circle shadow"
            style="width: 220px; height: 220px; object-fit: cover;">
        </div>

        <div class="col-lg-8">
          <div class="glass rounded-4 shadow-sm p-4 p-md-5">
            <!-- 【可替換：姓名 / 一句定位】 -->
            <span class="badge hero-badge text-dark px-3 py-2 rounded-pill mb-3">
              【可替換：一句標語，例如：內容企劃｜行銷研究｜簡報與網頁基礎】
            </span>
            <h1 class="display-6 fw-bold mb-2">【你的姓名】</h1>

            <!-- 【可替換：自我介紹 2–3 句】 -->
            <p class="text-secondary mb-4">
              【可替換：2–3 句自我介紹。建議：你在學什麼、你擅長什麼、你想找什麼方向/實習。】
            </p>

            <div class="d-flex flex-wrap gap-2">
              <!-- 先做履歷頁：按鈕先導向頁內區塊；之後你要做新頁再改連結即可 -->
              <a class="btn btn-primary px-4" href="#projects">看作品區</a>
              <a class="btn btn-outline-dark px-4" href="#contact">聯絡我</a>

              <!-- 【預留：未來大學生活頁】之後做 college.html 再把 href 改成 college.html -->
              <a class="btn btn-outline-secondary px-4 disabled" aria-disabled="true" href="#">
                大學生活（之後新增）
              </a>
            </div>

            <hr class="my-4">

            <!-- 【可替換：基本資料】 -->
            <div class="row g-3">
              <div class="col-md-6">
                <div class="d-flex align-items-start gap-2">
                  <span class="icon-dot text-primary mt-1"></span>
                  <div>
                    <div class="fw-semibold">就讀</div>
                    <div class="text-secondary">【可替換：學校｜科系｜年級】</div>
                  </div>
                </div>
              </div>
              <div class="col-md-6">
                <div class="d-flex align-items-start gap-2">
                  <span class="icon-dot text-success mt-1"></span>
                  <div>
                    <div class="fw-semibold">目標</div>
                    <div class="text-secondary">【可替換：想走的方向，例如：行銷企劃/內容企劃/品牌研究】</div>
                  </div>
                </div>
              </div>
            </div>

          </div>
        </div>
      </div>
    </div>
  </header>

  <main class="pb-5">
    <div class="container">
      <div class="row g-4">

        <!-- LEFT：主要內容 -->
        <div class="col-lg-8">

          <!-- ABOUT -->
          <section id="about" class="glass rounded-4 shadow-sm p-4 p-md-5 mb-4">
            <h2 class="h4 fw-bold section-title mb-3">關於我</h2>
            <!-- 【可替換：關於我內容】 -->
            <p class="text-secondary mb-0">
              【可替換：建議寫 4–6 行。可以包含：你擅長的事、做過的專題、你最重視的特質（負責/細心/溝通）。】
            </p>
          </section>

          <!-- SKILLS -->
          <section id="skills" class="glass rounded-4 shadow-sm p-4 p-md-5 mb-4">
            <h2 class="h4 fw-bold section-title mb-3">專長技能</h2>

            <!-- 【可替換：技能標籤】 -->
            <div class="d-flex flex-wrap gap-2 mb-3">
              <span class="badge skill-pill text-dark rounded-pill px-3 py-2">【可替換：簡報設計】</span>
              <span class="badge skill-pill text-dark rounded-pill px-3 py-2">【可替換：口頭報告】</span>
              <span class="badge skill-pill text-dark rounded-pill px-3 py-2">【可替換：問卷設計】</span>
              <span class="badge skill-pill text-dark rounded-pill px-3 py-2">【可替換：資料整理】</span>
              <span class="badge skill-pill text-dark rounded-pill px-3 py-2">【可替換：HTML/Bootstrap】</span>
              <span class="badge skill-pill text-dark rounded-pill px-3 py-2">【可替換：社群內容】</span>
            </div>

            <!-- 【可替換：技能敘述】 -->
            <div class="row g-3">
              <div class="col-md-6">
                <div class="border rounded-4 p-3 bg-white">
                  <div class="fw-semibold mb-1">研究 / 分析</div>
                  <div class="text-secondary small">
                    【可替換：例如：研究架構、文獻整理、問卷設計、量表、資料解讀】
                  </div>
                </div>
              </div>
              <div class="col-md-6">
                <div class="border rounded-4 p-3 bg-white">
                  <div class="fw-semibold mb-1">企劃 / 表達</div>
                  <div class="text-secondary small">
                    【可替換：例如：簡報結構、口語表達、腳本撰寫、社群內容發想】
                  </div>
                </div>
              </div>
              <div class="col-md-6">
                <div class="border rounded-4 p-3 bg-white">
                  <div class="fw-semibold mb-1">數位工具</div>
                  <div class="text-secondary small">
                    【可替換：例如：Canva、PowerPoint、Google Workspace、iMovie、AI 工具】
                  </div>
                </div>
              </div>
              <div class="col-md-6">
                <div class="border rounded-4 p-3 bg-white">
                  <div class="fw-semibold mb-1">網頁基礎</div>
                  <div class="text-secondary small">
                    【可替換：例如：HTML、Bootstrap、GitHub Pages 部署】
                  </div>
                </div>
              </div>
            </div>
          </section>

          <!-- EXPERIENCE -->
          <section id="experience" class="glass rounded-4 shadow-sm p-4 p-md-5 mb-4">
            <h2 class="h4 fw-bold section-title mb-3">經歷</h2>

            <!-- 時間軸：你只要替換文字即可 -->
            <div class="timeline">
              <div class="timeline-item">
                <div class="d-flex justify-content-between flex-wrap">
                  <div class="fw-semibold">【可替換：經歷/角色名稱】</div>
                  <div class="text-secondary small">【可替換：年份/期間】</div>
                </div>
                <ul class="text-secondary mb-0 mt-2">
                  <li>【可替換：做了什麼（具體一點）】</li>
                  <li>【可替換：產出/成果（例如：完成簡報/問卷/影片/活動）】</li>
                </ul>
              </div>

              <div class="timeline-item">
                <div class="d-flex justify-content-between flex-wrap">
                  <div class="fw-semibold">【可替換：經歷/角色名稱】</div>
                  <div class="text-secondary small">【可替換：年份/期間】</div>
                </div>
                <ul class="text-secondary mb-0 mt-2">
                  <li>【可替換：做了什麼】</li>
                  <li>【可替換：合作/溝通/統整的內容】</li>
                </ul>
              </div>
            </div>
          </section>

          <!-- PROJECTS -->
          <section id="projects" class="glass rounded-4 shadow-sm p-4 p-md-5">
            <div class="d-flex align-items-center justify-content-between flex-wrap gap-2 mb-3">
              <h2 class="h4 fw-bold section-title mb-0">作品 / 專題</h2>
              <span class="text-secondary small">【可替換：可放一句總結，例如：以研究與企劃為主】</span>
            </div>

            <div class="row g-3">
              <!-- 作品卡 1 -->
              <div class="col-md-6">
                <div class="card border-0 shadow-sm rounded-4 h-100">
                  <div class="card-body p-4">
                    <div class="fw-bold mb-1">【可替換：作品/專題名稱】</div>
                    <div class="text-secondary small mb-3">【可替換：一句副標，例如：研究｜問卷｜簡報】</div>
                    <ul class="text-secondary mb-0">
                      <li>【可替換：你負責的內容】</li>
                      <li>【可替換：成果或亮點】</li>
                    </ul>
                    <!-- 之後你有連結再打開 -->
                    <a class="btn btn-outline-primary btn-sm mt-3 disabled" href="#" aria-disabled="true">
                      作品連結（之後新增）
                    </a>
                  </div>
                </div>
              </div>

              <!-- 作品卡 2 -->
              <div class="col-md-6">
                <div class="card border-0 shadow-sm rounded-4 h-100">
                  <div class="card-body p-4">
                    <div class="fw-bold mb-1">【可替換：作品/專題名稱】</div>
                    <div class="text-secondary small mb-3">【可替換：一句副標】</div>
                    <ul class="text-secondary mb-0">
                      <li>【可替換：你負責的內容】</li>
                      <li>【可替換：成果或亮點】</li>
                    </ul>
                    <a class="btn btn-outline-primary btn-sm mt-3 disabled" href="#" aria-disabled="true">
                      作品連結（之後新增）
                    </a>
                  </div>
                </div>
              </div>
            </div>

          </section>
        </div>

        <!-- RIGHT：側欄（聯絡/快速資訊） -->
        <div class="col-lg-4">

          <section id="contact" class="glass rounded-4 shadow-sm p-4 mb-4">
            <h2 class="h5 fw-bold mb-3">聯絡方式</h2>

            <!-- 【可替換：聯絡資訊】 -->
            <div class="mb-2">
              <div class="text-secondary small">Email</div>
              <div class="fw-semibold">【可替換：你的 Email】</div>
            </div>

            <div class="mb-2">
              <div class="text-secondary small">GitHub</div>
              <div class="fw-semibold">【可替換：你的 GitHub 帳號或連結文字】</div>
            </div>

            <div class="mb-0">
              <div class="text-secondary small">社群</div>
              <div class="fw-semibold">【可替換：IG / FB / LinkedIn】</div>
            </div>

            <hr class="my-3">

            <!-- 小提醒：之後新增頁面 -->
            <div class="text-secondary small">
              提示：等你做完「大學生活」頁面後，把上面 HERO 的「大學生活（之後新增）」按鈕改成
              <span class="fw-semibold">college.html</span> 就能跳轉。
            </div>
          </section>

          <section class="glass rounded-4 shadow-sm p-4">
            <h2 class="h5 fw-bold mb-3">快速摘要</h2>

            <!-- 【可替換：3–5 點亮點】 -->
            <ul class="text-secondary mb-0">
              <li>【可替換：亮點 1】</li>
              <li>【可替換：亮點 2】</li>
              <li>【可替換：亮點 3】</li>
              <li>【可替換：亮點 4】</li>
            </ul>
          </section>

        </div>
      </div>
    </div>
  </main>

  <footer class="py-4">
    <div class="container text-center text-secondary small">
      © <span id="year"></span> 【可替換：你的名字】｜All rights reserved.
    </div>
  </footer>

  <script>
    document.getElementById("year").textContent = new Date().getFullYear();
  </script>
</body>
</html>
