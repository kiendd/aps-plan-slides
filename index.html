<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Kế hoạch Phối hợp FPT × APS · Đưa Trợ lý AI vào App Chứng khoán</title>
  <!--
    Kế hoạch phối hợp hoàn thiện & đưa Trợ lý AI vào App APS.
    Tài liệu thảo luận và đề xuất hợp tác chiến lược giữa FPT và APEC/APS.
    Điều hướng: ← → / Space, Menu, Phím N mở ghi chú, F toàn màn hình.
  -->
  <style>
    :root {
      --bg: #090d16;
      --surface: #111827;
      --surface-card: #162032;
      --surface-card-hover: #1c2940;
      --border: #23324d;
      --border-light: #334769;
      --text: #f3f4f6;
      --text-muted: #94a3b8;
      --text-dim: #64748b;
      --accent: #38bdf8;
      --primary: #2563eb;
      --success: #10b981;
      --warning: #f59e0b;
      --danger: #ef4444;
      --purple: #a855f7;
    }
    * { box-sizing: border-box; margin: 0; padding: 0; }
    body {
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
      background: var(--bg); color: var(--text);
      overflow: hidden; height: 100vh; width: 100vw;
    }
    #progress-bar {
      position: fixed; top: 0; left: 0; height: 4px; width: 0%; z-index: 100;
      background: linear-gradient(90deg, #2563eb, #38bdf8, #10b981);
      transition: width 0.3s ease;
    }
    .deck { position: relative; height: 100vh; width: 100vw; }
    .slide {
      position: absolute; inset: 0; margin: 0 auto; max-width: 1400px;
      padding: 36px 56px 76px; display: flex; flex-direction: column;
      opacity: 0; visibility: hidden; transform: translateY(16px);
      transition: opacity .35s ease, transform .35s ease, visibility .35s ease;
      overflow-y: auto;
    }
    .slide.active { opacity: 1; visibility: visible; transform: none; }

    /* Header */
    .badges { display: flex; gap: 8px; margin-bottom: 12px; flex-wrap: wrap; }
    .badge {
      display: inline-flex; align-items: center; gap: 6px; font-size: 12px; font-weight: 600;
      text-transform: uppercase; letter-spacing: 1px; padding: 4px 12px; border-radius: 999px;
      color: var(--accent); background: rgba(56,189,248,.1); border: 1px solid rgba(56,189,248,.25);
    }
    .badge.phase { color: #34d399; background: rgba(16,185,129,.1); border-color: rgba(16,185,129,.3); }
    .slide-title { font-size: 32px; font-weight: 700; color: #fff; letter-spacing: -.5px; line-height: 1.25; }
    .slide-subtitle { font-size: 16px; color: var(--text-muted); margin-top: 6px; line-height: 1.5; max-width: 1100px; }
    .slide-header { margin-bottom: 22px; }

    /* Grids & Cards */
    .grid-2 { display: grid; grid-template-columns: 1fr 1fr; gap: 20px; flex: 1; min-height: 0; }
    .grid-3 { display: grid; grid-template-columns: repeat(3, 1fr); gap: 18px; flex: 1; min-height: 0; }
    .card {
      background: var(--surface-card); border: 1px solid var(--border); border-radius: 14px;
      padding: 24px 26px; display: flex; flex-direction: column; gap: 14px;
    }
    .card h3 { font-size: 18.5px; color: #fff; display: flex; gap: 8px; align-items: center; font-weight: 700; margin-bottom: 2px; }
    .card h4 { font-size: 15px; color: var(--accent); }
    ul { list-style: none; margin: 0; padding: 0; }
    .card p { font-size: 14px; color: var(--text-muted); line-height: 1.6; }
    .card ul { list-style: none; display: flex; flex-direction: column; gap: 12px; margin: 0; padding: 0; }
    .card ul li { position: relative; padding-left: 18px; font-size: 14px; line-height: 1.6; color: var(--text); }
    .card ul li .dot { position: absolute; left: 0; top: 0; color: var(--accent); font-weight: bold; }

    .tag-green { color: #34d399; background: rgba(16,185,129,.12); border: 1px solid rgba(16,185,129,.3); padding: 2px 8px; border-radius: 6px; font-size: 11.5px; font-weight: 600; width: fit-content; }
    .tag-blue { color: #38bdf8; background: rgba(56,189,248,.12); border: 1px solid rgba(56,189,248,.3); padding: 2px 8px; border-radius: 6px; font-size: 11.5px; font-weight: 600; width: fit-content; }
    .tag-purple { color: #c084fc; background: rgba(168,85,247,.12); border: 1px solid rgba(168,85,247,.3); padding: 2px 8px; border-radius: 6px; font-size: 11.5px; font-weight: 600; width: fit-content; }

    /* 2x2 Grid */
    .grid-2x2 { display: grid; grid-template-columns: 1fr 1fr; gap: 16px; flex: 1; min-height: 0; }

    /* Architecture / Flow boxes */
    .arch-flow { display: flex; flex-direction: column; gap: 14px; width: 100%; }
    .arch-step { background: var(--surface-card); border: 1px solid var(--border); border-radius: 12px; padding: 16px 20px; display: grid; grid-template-columns: 180px 1fr; gap: 20px; align-items: center; }
    .arch-step b { font-size: 14.5px; color: #fff; }
    .arch-step p { font-size: 13.5px; color: var(--text-muted); line-height: 1.5; }

    /* Title Slide */
    .title-slide { justify-content: center; gap: 20px; }
    .title-slide h1 { font-size: 48px; letter-spacing: -1px; line-height: 1.15; }
    .title-slide h1 span { background: linear-gradient(90deg, #38bdf8, #10b981); -webkit-background-clip: text; background-clip: text; color: transparent; }
    .title-slide .lead { font-size: 18px; color: var(--text-muted); max-width: 950px; line-height: 1.55; }
    .pillars { display: grid; grid-template-columns: repeat(6, 1fr); gap: 10px; margin-top: 10px; width: 100%; }
    .pillar-item { background: var(--surface-card); border: 1px solid var(--border); border-radius: 12px; padding: 12px 14px; }
    .pillar-item .num { font-size: 11.5px; font-weight: 700; color: var(--accent); text-transform: uppercase; margin-bottom: 3px; }
    .pillar-item b { font-size: 13.5px; color: #fff; display: block; margin-bottom: 3px; line-height: 1.3; }
    .pillar-item span { font-size: 11.5px; color: var(--text-muted); line-height: 1.4; display: block; }

    /* Timeline & Comparison Table */
    table.timeline-table { width: 100%; border-collapse: collapse; font-size: 13.5px; text-align: left; }
    table.timeline-table th { background: rgba(255,255,255,.05); color: var(--text-muted); padding: 12px 16px; border-bottom: 1px solid var(--border); font-weight: 600; }
    table.timeline-table td { padding: 13px 16px; border-bottom: 1px solid var(--border); line-height: 1.5; color: var(--text); vertical-align: top; }
    table.timeline-table tr:last-child td { border-bottom: none; }
    /* Controls */
    .controls {
      position: fixed; bottom: 0; left: 0; right: 0; height: 52px; z-index: 100;
      background: rgba(11,15,25,.92); backdrop-filter: blur(10px); border-top: 1px solid var(--border);
      display: flex; align-items: center; justify-content: space-between; padding: 0 28px;
    }
    .controls > div { display: flex; align-items: center; gap: 12px; }
    .btn {
      background: var(--surface-card); border: 1px solid var(--border); color: var(--text);
      padding: 6px 14px; border-radius: 8px; font-size: 13px; cursor: pointer;
    }
    .btn:hover { background: var(--surface-card-hover); border-color: var(--border-light); }
    .btn-primary { background: var(--primary); border-color: #3b82f6; color: #fff; font-weight: 600; }
    .counter { font-size: 13px; font-weight: 600; color: var(--text-muted); }
    #notes-panel {
      position: fixed; bottom: 52px; right: 28px; width: 480px; max-height: 300px; z-index: 99;
      background: #0f172a; border: 1px solid var(--border-light); border-radius: 12px; padding: 16px 20px;
      box-shadow: 0 10px 25px rgba(0,0,0,.5); display: none; flex-direction: column; gap: 8px; overflow-y: auto;
    }
    #notes-panel.open { display: flex; }
    #notes-panel h4 { font-size: 12px; color: var(--accent); text-transform: uppercase; letter-spacing: .5px; }
    #notes-content { font-size: 13.5px; color: var(--text-muted); line-height: 1.55; }

    /* Mobile Responsive (<= 900px) */
    @media (max-width: 900px) {
      .slide { padding: 16px 14px 68px; overflow-y: auto; -webkit-overflow-scrolling: touch; }
      .slide-title { font-size: 22px; line-height: 1.25; }
      .slide-subtitle { font-size: 13.5px; line-height: 1.45; }
      .slide-header { margin-bottom: 14px; }
      .title-slide { justify-content: flex-start; padding-top: 24px; gap: 14px; }
      .title-slide h1 { font-size: 28px; }
      .title-slide .lead { font-size: 14px; }
      .grid-2, .grid-3, .grid-2x2 { display: flex; flex-direction: column; gap: 14px; }
      .card:has(table.timeline-table) { overflow-x: auto !important; -webkit-overflow-scrolling: touch; }
      table.timeline-table { min-width: 600px; }
      .controls { height: 48px; padding: 0 10px; }
      .controls > div { gap: 6px; }
      .btn { padding: 5px 8px; font-size: 11.5px; }
      #btn-notes, #btn-fs { display: none; }
      #notes-panel { left: 10px; right: 10px; width: auto; bottom: 50px; }
    }
  </style>
</head>
<body>
  <div id="progress-bar"></div>
  <div class="deck" id="deck"></div>

  <div class="controls">
    <div>
      <button class="btn" onclick="go(current - 1)" title="Mũi tên trái">◀ Trước</button>
      <button class="btn" onclick="go(current + 1)" title="Mũi tên phải / Space">Tiếp ▶</button>
      <span class="counter" id="counter"></span>
    </div>
    <div>
      <button class="btn" onclick="go(1)" title="Về slide menu">☰ Menu</button>
      <button class="btn" id="btn-notes" onclick="toggleNotes()" title="Phím N">📝 Ghi chú</button>
      <button class="btn" id="btn-fs" onclick="toggleFullScreen()" title="Phím F">⛶ Toàn màn hình</button>
    </div>
  </div>
  <div id="notes-panel"><h4>Gợi ý thuyết trình</h4><div id="notes-content"></div></div>

  <script>
    const deck = document.getElementById("deck");
    const pad = (n) => String(n).padStart(2, "0");

    function addSlide(html, notes) {
      const el = document.createElement("section");
      el.className = "slide";
      el.innerHTML = html;
      el.dataset.notes = notes ?? "";
      deck.appendChild(el);
      return el;
    }

    // SLIDE 1: TRANG BÌA
    addSlide(`
      <div class="badges">
        <span class="badge">FPT × APEC Securities</span>
        <span class="badge phase">Giai đoạn 2 · Triển khai Thực tế</span>
      </div>
      <h1>Kế hoạch Phối hợp FPT × APS<br><span>Đưa Trợ lý AI vào App Chứng khoán</span></h1>
      <p class="lead">Đề xuất lộ trình và các đầu việc phối hợp chiến lược nhằm nâng cấp chất lượng phân tích nghiệp vụ, đấu nối hệ thống kỹ thuật và tích hợp Trợ lý AI trực tiếp vào ứng dụng giao dịch của APS.</p>
      <div class="pillars">
        <div class="pillar-item" style="border-top: 3px solid var(--accent)">
          <div class="num" style="color: var(--accent)">FPT · Việc 01</div>
          <b>So sánh Đa Model LLM</b>
          <span>Đo lường chọn model chính xác & văn phong hay nhất</span>
        </div>
        <div class="pillar-item" style="border-top: 3px solid var(--accent)">
          <div class="num" style="color: var(--accent)">FPT · Việc 02</div>
          <b>Tích hợp Kỹ thuật App</b>
          <span>REST API, Webhook Notification & Auth Token</span>
        </div>
        <div class="pillar-item" style="border-top: 3px solid var(--purple)">
          <div class="num" style="color: #c084fc">APS · Việc 03</div>
          <b>Đồng hành BA & Phân tích</b>
          <span>Nâng cao chất lượng câu trả lời & độ sâu phân tích</span>
        </div>
        <div class="pillar-item" style="border-top: 3px solid var(--purple)">
          <div class="num" style="color: #c084fc">APS · Việc 04</div>
          <b>Chuẩn hóa Nghiệp vụ</b>
          <span>Ranh giới tư vấn, so sánh & chính sách push</span>
        </div>
        <div class="pillar-item" style="border-top: 3px solid var(--purple)">
          <div class="num" style="color: #c084fc">APS · Việc 05</div>
          <b>Quy trình Môi giới</b>
          <span>Tiếp nhận & định tuyến cơ hội chăm sóc khách</span>
        </div>
        <div class="pillar-item" style="border-top: 3px solid var(--purple)">
          <div class="num" style="color: #c084fc">APS · Việc 06</div>
          <b>Mở rộng Kho tri thức</b>
          <span>Margin, Trái phiếu Abond, Asavings & BCTC</span>
        </div>
      </div>
    `, "Mở đầu: Sau khi nghiệm thu thành công bản PoC, đây là kế hoạch hành động 6 việc phối hợp rõ ràng theo 2 nhóm: 2 việc FPT chủ trì công nghệ & 4 việc APS chủ trì nghiệp vụ.").classList.add("title-slide");

    // SLIDE 2: MỤC TIÊU CHUYỂN DỊCH
    addSlide(`
      <div class="slide-header">
        <div class="badges"><span class="badge">Tầm nhìn & Mục tiêu</span></div>
        <h2 class="slide-title">Bức tranh Chuyển dịch từ PoC lên Sản phẩm Thực tế</h2>
        <p class="slide-subtitle">Chuyển mình từ một bot thử nghiệm độc lập trên Telegram sang một Trợ lý AI tài chính nhúng sâu vào hành trình giao dịch của nhà đầu tư APS.</p>
      </div>
      <div class="card" style="padding:0; overflow:hidden;">
        <table class="timeline-table">
          <thead>
            <tr>
              <th style="width: 22%">Hạng mục chuyển đổi</th>
              <th style="width: 39%"><span style="color:#f87171">⏳ Hiện trạng Bản Thử nghiệm (PoC)</span></th>
              <th style="width: 39%"><span style="color:#34d399">🚀 Mục tiêu Sản phẩm Thực tế (Live App)</span></th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td><strong>1. Môi trường & Giao diện</strong></td>
              <td>Chạy độc lập trên Telegram bot cá nhân; người dùng cần có tài khoản Telegram riêng.</td>
              <td><strong>Tích hợp trực tiếp vào Mobile App APS (iOS/Android)</strong>; kênh Telegram duy trì dưới dạng tùy chọn (Optional - do APS quyết định).</td>
            </tr>
            <tr>
              <td><strong>2. Tài khoản & Danh mục</strong></td>
              <td>Dữ liệu danh mục giả lập từ 3 Mẫu khách (Thận trọng, Cân bằng, Tích cực).</td>
              <td><strong>Kết nối API Core Trading của APS</strong>: truy vấn danh mục thực tế, lãi/lỗ thời gian thực và sức mua margin.</td>
            </tr>
            <tr>
              <td><strong>3. Dữ liệu giá & Cảnh báo</strong></td>
              <td>Dữ liệu giá snapshot trễ 5 phút; cảnh báo gửi qua tin nhắn bot Telegram.</td>
              <td><strong>Giá streaming realtime từ sở (HOSE/HNX)</strong>; đẩy Push Notification trực tiếp vào điện thoại khách hàng.</td>
            </tr>
            <tr>
              <td><strong>4. Cơ chế Môi giới & Tư vấn</strong></td>
              <td>Bắn thông báo vào Group Telegram nội bộ để nhân sự trực tiếp nhận thủ công.</td>
              <td><strong>Định tuyến tự động cho Broker quản lý tài khoản</strong> qua hệ thống CRM / App Careby nội bộ của APS.</td>
            </tr>
            <tr>
              <td><strong>5. Kho tri thức & Sản phẩm</strong></td>
              <td>Dữ liệu FAQ công khai trên website apec.com.vn và văn bản quy phạm pháp luật cơ bản.</td>
              <td><strong>Chuyên sâu về biểu phí margin, sản phẩm tài chính APEC</strong> (Abond, Asavings, CW) & Báo cáo phân tích định kỳ.</td>
            </tr>
          </tbody>
        </table>
      </div>
    `, "Nhấn mạnh với lãnh đạo APS: PoC đã chứng minh năng lực lõi (xử lý tiếng Việt, không bịa số, kiểm duyệt an toàn). Giai đoạn 2 là gắn động cơ AI này vào cỗ máy kinh doanh của APS để tạo đột phá cạnh tranh.");
    // SLIDE 3: MA TRẬN 6 ĐẦU VIỆC PHỐI HỢP
    addSlide(`
      <div class="slide-header">
        <div class="badges"><span class="badge">Phân công Phối hợp</span></div>
        <h2 class="slide-title">Ma trận Phân nhiệm FPT × APS (RACI Matrix)</h2>
        <p class="slide-subtitle">Rõ ràng trách nhiệm giữa hai bên cho 6 đầu việc trọng tâm để đảm bảo tiến độ triển khai nhanh và chuẩn xác nhất.</p>
      </div>
      <div class="card" style="padding:0; overflow:hidden;">
        <table class="timeline-table">
          <thead>
            <tr>
              <th style="width:28%">Nội dung công việc</th>
              <th style="width:40%">Trách nhiệm chính của FPT</th>
              <th style="width:32%">Trách nhiệm phối hợp của APS</th>
            </tr>
          </thead>
          <tbody>
            <tr style="background: rgba(56,189,248,.05);">
              <td colspan="3" style="color: var(--accent); font-weight: 700; padding: 8px 14px; text-transform: uppercase; font-size: 11.5px; letter-spacing: 0.5px;">
                ⚡ Khối I: FPT chủ trì (Công nghệ AI, Đánh giá Mô hình & Hạ tầng Kết nối)
              </td>
            </tr>
            <tr>
              <td><strong>Việc 01: So sánh Đa Model LLM</strong></td>
              <td>Thực hiện benchmark đối đầu các model nguồn mở host bởi FPT Smart Cloud (Qwen, Saola, Llama,...), đo lường độ chính xác & văn phong.</td>
              <td>Cùng tham gia thẩm định chất lượng hành văn tiếng Việt, phê duyệt lựa chọn model tối ưu.</td>
            </tr>
            <tr>
              <td><strong>Việc 02: Tích hợp Kỹ thuật App</strong></td>
              <td>Cung cấp REST API chat đồng bộ, Webhook push sự kiện & module xác thực User Token.</td>
              <td>Nhúng khung chat vào App APS, mở API xác thực JWT và mở API đọc danh mục thực tế.</td>
            </tr>
            <tr style="background: rgba(168,85,247,.05);">
              <td colspan="3" style="color: #c084fc; font-weight: 700; padding: 8px 14px; text-transform: uppercase; font-size: 11.5px; letter-spacing: 0.5px;">
                🏛️ Khối II: APS chủ trì (Nghiệp vụ Chứng khoán, Pháp chế, Khách hàng & Vận hành)
              </td>
            </tr>
            <tr>
              <td><strong>Việc 03: Đồng hành BA & Phân tích</strong></td>
              <td>Thiết kế prompt, cấu trúc đầu ra, hiệu chỉnh mô hình & thuật toán trích xuất insight tài chính.</td>
              <td>Cử BA & Chuyên viên phân tích đồng hành xây dựng logic phân tích Vĩ mô / Thế giới tác động đến TTCK Việt Nam, thẩm định câu trả lời & bộ câu hỏi mẫu.</td>
            </tr>
            <tr>
              <td><strong>Việc 04: Chuẩn hóa Quy tắc Nghiệp vụ</strong></td>
              <td>Hiện thực hóa cơ chế Đèn giao thông (phân luồng 3 nhánh: 🟢 Xanh tra cứu dữ kiện, 🟡 Vàng phân tích có kiểm duyệt, 🔴 Đỏ chặn tư vấn mua/bán), 3 hướng so sánh cổ phiếu và chính sách chặn spam.</td>
              <td>Khối Pháp chế & Nghiệp vụ chốt ranh giới tư vấn, lựa chọn tiêu chí so sánh và duyệt ngưỡng cảnh báo.</td>
            </tr>
            <tr>
              <td><strong>Việc 05: Quy trình Môi giới</strong></td>
              <td>Xây dựng module chuyển tiếp lead, webhook đẩy sự kiện tư vấn & giao diện xác nhận với khách.</td>
              <td>Nghiên cứu & đề xuất quy trình tiếp nhận (CRM nội bộ, Careby hay phân bổ Broker quản lý).</td>
            </tr>
            <tr>
              <td><strong>Việc 06: Mở rộng Kho tri thức</strong></td>
              <td>Tự động hóa xử lý tri thức chuyên ngành, tối ưu công cụ tìm kiếm ngữ nghĩa và trích dẫn chuẩn nguồn tài liệu.</td>
              <td>Cung cấp tài liệu sản phẩm đặc thù (Abond, Asavings, CW) và báo cáo phân tích định kỳ.</td>
            </tr>
          </tbody>
        </table>
      </div>
    `, "Điểm cốt lõi: FPT đóng vai trò công nghệ và sản phẩm AI; APS đóng vai trò chủ trì nghiệp vụ, dữ liệu nguồn và trải nghiệm khách hàng.");
    // SLIDE 4: VIỆC 01 (FPT CHỦ TRÌ) - SO SÁNH ĐA MODEL LLM
    addSlide(`
      <div class="slide-header">
        <div class="badges">
          <span class="badge" style="color: var(--accent); border-color: rgba(56,189,248,.35); background: rgba(56,189,248,.12)">FPT chủ trì</span>
          <span class="badge phase">Việc 01 · Công nghệ & Đánh giá</span>
        </div>
        <h2 class="slide-title">So sánh Đa Model LLM: Tìm Độ chính xác & Văn phong Tối ưu</h2>
        <p class="slide-subtitle">FPT chủ trì thử nghiệm đối đầu (Benchmark) giữa các dòng mô hình AI tiên tiến nhất hiện nay nhằm chọn ra mô hình có dữ kiện chuẩn xác nhất, văn phong tài chính sắc sảo nhất và chi phí vận hành tối ưu.</p>
      </div>
      <div class="grid-3">
        <div class="card">
          <div class="tag-green">Độ tin cậy cốt lõi</div>
          <h3>1. Độ chính xác Dữ kiện (Grounding)</h3>
          <ul>
            <li><span class="dot">•</span> <strong>Không bịa số (0% Hallucination):</strong> Model phải bám sát tuyệt đối dữ kiện tài chính được cung cấp, không tự tiện suy đoán hoặc làm tròn sai lệch con số.</li>
            <li><span class="dot">•</span> <strong>Tuân thủ Guardrails:</strong> Thử nghiệm khả năng vượt qua bộ lọc số lạ và bộ lọc cụm từ cấm độc lập của hệ thống.</li>
            <li><span class="dot">•</span> <strong>Các model thử nghiệm:</strong> Các mô hình mã nguồn mở được host bởi FPT Smart Cloud như Qwen, Saola, Llama,...</li>
          </ul>
        </div>
        <div class="card">
          <div class="tag-purple">Chất lượng diễn đạt</div>
          <h3>2. Văn phong Tài chính Sắc sảo</h3>
          <ul>
            <li><span class="dot">•</span> <strong>Hành văn tiếng Việt tự nhiên:</strong> Diễn đạt gãy gọn, mạch lạc, giàu tính phân tích; loại bỏ hoàn toàn cảm giác dịch máy khô cứng (Google Translate style).</li>
            <li><span class="dot">•</span> <strong>Bóc tách nguyên nhân sâu sắc:</strong> Biết xâu chuỗi thông tin giữa biến động giá và tin tức vĩ mô, đem lại trải nghiệm như đang trao đổi với chuyên viên phân tích kỳ cựu.</li>
            <li><span class="dot">•</span> <strong>Khảo sát mù (Blind Test):</strong> Đội ngũ BA/Môi giới APS trực tiếp bình chọn văn phong ưng ý nhất.</li>
          </ul>
        </div>
        <div class="card">
          <div class="tag-blue">Kinh tế & Hiệu năng</div>
          <h3>3. Tốc độ & Chi phí Quy mô</h3>
          <ul>
            <li><span class="dot">•</span> <strong>Phản hồi tức thì với tra cứu dữ liệu:</strong> Độ trễ &lt; 1,5 giây cho các truy vấn trực tiếp (giá thị trường, chỉ số cơ bản, FAQ định sẵn bằng code).</li>
            <li><span class="dot">•</span> <strong>Thời gian phản hồi phân tích (LLM):</strong> Độ trễ toàn trình 2,5 – 4,0 giây cho các câu hỏi tổng hợp, phân tích chuyên sâu (bao gồm RAG, tổng hợp ngữ cảnh và kiểm duyệt Guardrails).</li>
            <li><span class="dot">•</span> <strong>Tối ưu chi phí Token:</strong> Đánh giá chi phí vận hành trên mỗi lượt hỏi đáp, giúp APS mở rộng phục vụ hàng trăm ngàn nhà đầu tư với chi phí hiệu quả nhất.</li>
            <li><span class="dot">•</span> <strong>Hạ tầng FPT Smart Cloud:</strong> Vận hành hoàn toàn trên hạ tầng FPT Smart Cloud, bảo đảm an toàn dữ liệu và quyền tự chủ công nghệ.</li>
          </ul>
        </div>
      </div>
    `, "Nhấn mạnh: Hệ thống sử dụng các mô hình mã nguồn mở host bởi FPT Smart Cloud (Qwen, Saola, Llama,...), vừa đảm bảo an toàn bảo mật dữ liệu, vừa mang lại chất giọng tài chính sắc sảo và chi phí vận hành tối ưu.");

    // SLIDE 5: VIỆC 02 (FPT CHỦ TRÌ) - TÍCH HỢP KỸ THUẬT & HẠ TẦNG APP
    addSlide(`
      <div class="slide-header">
        <div class="badges">
          <span class="badge" style="color: var(--accent); border-color: rgba(56,189,248,.35); background: rgba(56,189,248,.12)">FPT chủ trì</span>
          <span class="badge phase">Việc 02 · Kiến trúc Kỹ thuật</span>
        </div>
        <h2 class="slide-title">Phương án Tích hợp App: REST API + Webhook + Token Auth</h2>
        <p class="slide-subtitle">Thiết kế module hóa tối ưu, giúp đội ngũ Mobile App của APS đấu nối nhanh chóng, bảo mật thông tin tài khoản tuyệt đối và linh hoạt lựa chọn kênh triển khai.</p>
      </div>
      <div class="grid-2x2">
        <div class="card" style="border-left: 4px solid var(--accent);">
          <div class="tag-blue">Giao tiếp Hỏi đáp 2 chiều</div>
          <h3>1. REST API Chat</h3>
          <p>Mobile App APS gọi endpoint <code>POST /api/v1/chat/message</code> kèm JWT Token.</p>
          <ul>
            <li><span class="dot">•</span> <strong>Phản hồi trọn gói (Standard HTTP):</strong> Trả lời hoàn chỉnh trong một payload, đơn giản hóa tối đa tích hợp phía client Mobile App và bot chat.</li>
            <li><span class="dot">•</span> <strong>Cấu trúc JSON chuẩn hóa:</strong> Trả về các khối rõ ràng (tiêu đề, dữ kiện gạch đầu dòng, trích dẫn nguồn và gợi ý nút bấm).</li>
          </ul>
        </div>
        <div class="card" style="border-left: 4px solid var(--success);">
          <div class="tag-green">Tin đẩy chủ động</div>
          <h3>2. Webhook ➡️ Push Notification</h3>
          <p>Khi Bot Engine phát hiện biến động giá hoặc có Bản tin mới, hệ thống bắn payload qua Webhook của APS.</p>
          <ul>
            <li><span class="dot">•</span> <strong>Đẩy thông báo App (FCM / APNs):</strong> Server APS tiếp nhận sự kiện và gửi Push Notification trực tiếp vào thiết bị của khách hàng.</li>
            <li><span class="dot">•</span> <strong>Lọc theo danh mục thực:</strong> Chỉ gửi cho nhà đầu tư đang nắm giữ mã hoặc đã đăng ký quan tâm.</li>
          </ul>
        </div>
        <div class="card" style="border-left: 4px solid var(--purple);">
          <div class="tag-purple">Bảo mật & Phân quyền</div>
          <h3>3. Xác thực User Token (SSO)</h3>
          <p>Nhận diện khách hàng qua cơ chế Token do App APS cấp sau khi người dùng đăng nhập.</p>
          <ul>
            <li><span class="dot">•</span> <strong>Không lưu mật khẩu:</strong> Bot Gateway giải mã JWT Token qua Auth Service của APS để lấy định danh <code>account_no</code>.</li>
            <li><span class="dot">•</span> <strong>Truy vấn Core an toàn:</strong> Bot gọi internal API của APS để đọc danh mục thực tế của tài khoản trong phiên chat.</li>
          </ul>
        </div>
        <div class="card" style="border-left: 4px solid #f59e0b;">
          <div style="color: #fbbf24; background: rgba(245,158,11,.12); border: 1px solid rgba(245,158,11,.3); padding: 2px 8px; border-radius: 6px; font-size: 11.5px; font-weight: 600; width: fit-content;">Tùy chọn · Chờ APS quyết định</div>
          <h3>4. Kênh Telegram (Optional)</h3>
          <p>Phương án mở rộng tùy chọn nếu APS muốn tiếp cận khách hàng đa kênh hoặc độc quyền hoàn toàn trên App.</p>
          <ul>
            <li><span class="dot">•</span> <strong>Nếu duy trì Telegram:</strong> Khách quét mã QR trên App APS để liên kết với bot Telegram, đồng bộ cảnh báo và danh mục.</li>
            <li><span class="dot">•</span> <strong>Nếu ưu tiên "Độc quyền App":</strong> Đóng kênh Telegram bên ngoài, dồn toàn bộ lưu lượng và trải nghiệm giữ chân khách hàng vào App APS.</li>
          </ul>
        </div>
      </div>
    `, "Nhấn mạnh: Việc duy trì kênh Telegram là hoàn toàn tùy chọn (Optional) phụ thuộc vào chiến lược của APS — nếu APS muốn giữ chân khách hàng độc quyền trên Mobile App thì sẵn sàng đóng kênh ngoài.");

    // SLIDE 6: VIỆC 03 (APS CHỦ TRÌ) - ĐỒNG HÀNH BA & PHÂN TÍCH
    addSlide(`
      <div class="slide-header">
        <div class="badges">
          <span class="badge" style="color: #c084fc; border-color: rgba(168,85,247,.35); background: rgba(168,85,247,.12)">APS chủ trì</span>
          <span class="badge phase">Việc 03 · Đột phá Nghiệp vụ</span>
        </div>
        <h2 class="slide-title">Đồng hành BA & Chuyên gia Phân tích Chứng khoán APS</h2>
        <p class="slide-subtitle">Đề xuất mời đội ngũ BA và Chuyên viên nghiên cứu phân tích của APS trực tiếp tham gia nâng tầm chất lượng câu trả lời từ mức 'tra cứu thông tin' lên tầm 'tư vấn chuyên sâu sắc sảo', đặc biệt là năng lực bóc tách tác động Vĩ mô & Thế giới đến thị trường Việt Nam.</p>
      </div>
      <div class="grid-3">
        <div class="card">
          <div class="tag-purple">Insight tài chính sâu</div>
          <h3>1. Nâng cấp Câu trả lời & Vĩ mô</h3>
          <ul>
            <li><span class="dot">•</span> <strong>Phân tích Vĩ mô & Thế giới tác động TTCK VN:</strong> Nhờ chuyên gia APS cố vấn khung logic liên kết các sự kiện quốc tế (lãi suất Fed, tỷ giá USD/VND, giá dầu, địa chính trị, dòng vốn ngoại) với các nhóm ngành và cổ phiếu cụ thể tại Việt Nam.</li>
            <li><span class="dot">•</span> <strong>Giải thích biến động sâu:</strong> Không chỉ nêu tăng/giảm thuần túy; bóc tách nguyên nhân từ thanh khoản, khối ngoại bán ròng, chuỗi giá trị ngành và bối cảnh vĩ mô.</li>
            <li><span class="dot">•</span> <strong>Văn phong chuyên gia:</strong> Chuẩn hóa thuật ngữ tài chính sắc bén (định giá P/E forward, kháng cự/hỗ trợ, chu kỳ kinh tế, biên lợi nhuận ròng).</li>
          </ul>
        </div>
        <div class="card">
          <div class="tag-blue">Đồng hành thiết kế</div>
          <h3>2. Phối hợp Prompting</h3>
          <ul>
            <li><span class="dot">•</span> <strong>BA APS cùng viết kịch bản:</strong> Cùng đội ngũ FPT tinh chỉnh System Prompt cho các tác vụ phân tích ngành, đánh giá cổ phiếu và tóm tắt tin tức doanh nghiệp.</li>
            <li><span class="dot">•</span> <strong>Bẫy thuật ngữ & Biệt danh:</strong> Bổ sung các tiếng lóng thị trường, cách gọi thân mật của môi giới để bot hiểu tự nhiên nhất.</li>
          </ul>
        </div>
        <div class="card">
          <div class="tag-green">Thước đo chất lượng</div>
          <h3>3. Bộ Benchmark APS</h3>
          <ul>
            <li><span class="dot">•</span> <strong>Bộ câu hỏi chuẩn ngành:</strong> APS biên soạn 50–100 câu hỏi hóc búa thực tế mà khách hàng thường hỏi môi giới để đưa vào bộ kiểm thử tự động (Eval suite).</li>
            <li><span class="dot">•</span> <strong>Chấm điểm nghiệm thu:</strong> Chuyên gia APS trực tiếp đánh giá độ hữu ích và chuẩn xác của câu trả lời trước khi go-live.</li>
          </ul>
        </div>
      </div>
    `, "Nhấn mạnh: AI chỉ thông minh khi được nuôi dưỡng bằng tri thức của các chuyên gia thực thụ. Đặc biệt, việc bóc tách biến động thị trường Việt Nam dưới lăng kính Vĩ mô và Thế giới cần chuyên gia phân tích APS đồng hành đóng gói phương pháp luận và kiểm định.");

    // SLIDE 7: VIỆC 04 (APS CHỦ TRÌ) - CHUẨN HÓA QUY TẮC NGHIỆP VỤ & TƯ VẤN
    addSlide(`
      <div class="slide-header">
        <div class="badges">
          <span class="badge" style="color: #c084fc; border-color: rgba(168,85,247,.35); background: rgba(168,85,247,.12)">APS chủ trì</span>
          <span class="badge phase">Việc 04 · Tuân thủ & An toàn</span>
        </div>
        <h2 class="slide-title">Chuẩn hóa Ranh giới Tư vấn, So sánh & Chính sách Push</h2>
        <p class="slide-subtitle">Rà soát chặt chẽ các ranh giới nghiệp vụ cùng khối Pháp chế & Giám sát tuân thủ của APS trước khi đưa sản phẩm ra đại chúng.</p>
      </div>
      <div class="grid-3">
        <div class="card">
          <div class="tag-green">🟢 Xanh · 🟡 Vàng · 🔴 Đỏ</div>
          <h3>Ranh giới Tư vấn (Đèn giao thông)</h3>
          <p><strong>Cơ chế Đèn giao thông</strong> phân loại câu hỏi thành 3 luồng: 🟢 <em>Nhánh Xanh</em> (tra cứu dữ kiện thuần), 🟡 <em>Nhánh Vàng</em> (giải thích biến động, có bộ lọc số lạ), và 🔴 <em>Nhánh Đỏ</em> (xin khuyến nghị mua/bán). Hiện bot cấm 100% tự ý tư vấn ở Nhánh Đỏ. Đề xuất APS quyết định chính sách:</p>
          <ul>
            <li><span class="dot">•</span> <strong>Lựa chọn A (An toàn tuyệt đối):</strong> Giữ nguyên từ chối tư vấn độc lập ở Nhánh Đỏ; AI chỉ cung cấp dữ kiện thuần và chuyển hướng sang Môi giới người thật.</li>
            <li><span class="dot">•</span> <strong>Lựa chọn B (Dẫn nguồn APS Research):</strong> Cho phép bot trích dẫn nguyên văn khuyến nghị chính thức (Target price, Khả quan/Trung lập) nếu mã đó có Báo cáo phân tích do APS phát hành.</li>
          </ul>
        </div>
        <div class="card">
          <div class="tag-blue">3 Hướng so sánh mã</div>
          <h3>Nội dung So sánh (Nhánh vàng)</h3>
          <p>Hiện so sánh 2 mã theo giá và 5 chỉ số (P/E, P/B, EPS, BVPS, ROE). Đề xuất APS chọn hướng làm tiếp:</p>
          <ul>
            <li><span class="dot">•</span> <strong>Hướng 1 (Định giá APS):</strong> Đối chiếu định giá P/E forward và góc nhìn chuyên gia APS.</li>
            <li><span class="dot">•</span> <strong>Hướng 2 (Chính sách đòn bẩy Margin):</strong> So sánh tỷ lệ ký quỹ margin, hạn mức và lãi suất ưu đãi của 2 mã tại APS.</li>
            <li><span class="dot">•</span> <strong>Hướng 3 (Dòng tiền & Kỹ thuật):</strong> Đối chiếu khối ngoại và thanh khoản bình quân.</li>
          </ul>
        </div>
        <div class="card">
          <div class="tag-purple">Chống làm phiền</div>
          <h3>Chính sách Thông báo đẩy</h3>
          <p>Chuyển giao các ngưỡng cảnh báo hiện có sang chính sách vận hành trong App:</p>
          <ul>
            <li><span class="dot">•</span> <strong>Cá nhân hóa theo danh mục thực:</strong> Tự động kích hoạt cảnh báo biến động cho các mã có trong tài khoản APS của khách.</li>
            <li><span class="dot">•</span> <strong>Lịch quyền & Cổ tức:</strong> Báo trước ngày GDKHQ và lịch chi trả cổ tức các mã khách nắm giữ.</li>
            <li><span class="dot">•</span> <strong>Thẩm định ngưỡng:</strong> Khối Nghiệp vụ APS chốt trần số tin/ngày và khung giờ yên tĩnh trên App.</li>
          </ul>
        </div>
      </div>
    `, "Làm rõ với Pháp chế APS: Cơ chế Đèn giao thông (🟢 Xanh: tra cứu dữ kiện - 🟡 Vàng: phân tích có kiểm duyệt Guardrails - 🔴 Đỏ: chặn tư vấn mua bán vi phạm pháp lý). FPT cung cấp sẵn các chốt chặn này, APS là người nắm quyền quyết định điều chỉnh ranh giới ở Nhánh Đỏ cho phù hợp với định vị.");

    // SLIDE 8: VIỆC 05 (APS CHỦ TRÌ) - ĐẤU NỐI MÔI GIỚI THẬT
    addSlide(`
      <div class="slide-header">
        <div class="badges">
          <span class="badge" style="color: #c084fc; border-color: rgba(168,85,247,.35); background: rgba(168,85,247,.12)">APS chủ trì</span>
          <span class="badge phase">Việc 05 · Kinh doanh & Môi giới</span>
        </div>
        <h2 class="slide-title">Quy trình Chuyển tiếp Khách hàng cho Đội ngũ Broker APS</h2>
        <p class="slide-subtitle">Biến trợ lý AI thành công cụ tạo lead bán hàng đắc lực, tự động phát hiện nhu cầu tư vấn để chuyển giao cho chuyên viên môi giới tiếp quản.</p>
      </div>
      <div class="grid-2">
        <div class="card">
          <div class="tag-blue">Giai đoạn Chuyển tiếp (Pilot)</div>
          <h3>Kế thừa Cơ chế Group Thông báo</h3>
          <p>Tiếp tục duy trì giải pháp đã kiểm chứng ở bản PoC để có thể vận hành thử nghiệm ngay lập tức:</p>
          <ul>
            <li><span class="dot">•</span> <strong>Bước 1:</strong> Khách bấm "Gặp môi giới" trên App hoặc Telegram ➡️ Bot tự động tổng hợp câu hỏi, mã cổ phiếu và thông tin liên hệ.</li>
            <li><span class="dot">•</span> <strong>Bước 2:</strong> Bắn thông báo tức thì vào Group Telegram điều phối nội bộ của Khối Môi giới APS.</li>
            <li><span class="dot">•</span> <strong>Bước 3:</strong> Trưởng nhóm hoặc chuyên viên trực ca tiếp nhận thủ công và liên hệ hỗ trợ khách hàng ngay.</li>
          </ul>
        </div>
        <div class="card">
          <div class="tag-green">Đề xuất Định hướng Lâu dài</div>
          <h3>Đề nghị APS Nghiên cứu & Đề xuất</h3>
          <p>Phối hợp cùng APS xây dựng quy trình định tuyến tự động phù hợp với mô hình vận hành của công ty:</p>
          <ul>
            <li><span class="dot">•</span> <strong>Phương án 1 (Gắn theo Broker quản lý):</strong> Định tuyến tự động về hệ thống CRM / App Careby nội bộ của chính Môi viên đang chăm sóc tài khoản đó.</li>
            <li><span class="dot">•</span> <strong>Phương án 2 (Hàng đợi Tổng đài CSKH):</strong> Đối với khách hàng vãng lai chưa có môi giới riêng, đẩy vào hàng đợi của Telesales / CSKH APEC để chăm sóc và gắn Broker mới.</li>
            <li><span class="dot">•</span> <strong>Cam kết phản hồi (SLA):</strong> Bot hiển thị thông tin Broker (Tên, SĐT/Zalo) và gửi tin báo xác nhận chuyên viên đang liên hệ.</li>
          </ul>
        </div>
      </div>
      <div class="card" style="background: rgba(16,185,129,.06); border-color: rgba(16,185,129,.3); padding: 14px 18px; margin-top: 14px;">
        <h4 style="color:#34d399; margin-bottom:2px;">💡 Mục tiêu cốt lõi:</h4>
        <p style="color:var(--text); font-size:13.5px; margin:0;">AI không thay thế môi giới, mà trở thành phễu lọc nhu cầu tự động 24/7 và chuyển giao tận tay đội ngũ Broker APS các cơ hội giao dịch nóng nhất của nhà đầu tư.</p>
      </div>
    `, "Gửi thông điệp quan trọng tới Giám đốc Khối Môi giới APS: Bot sinh ra để phục vụ môi giới, giúp môi giới lọc trước nhu cầu của khách và trao tận tay môi giới những cơ hội giao dịch nóng nhất.");

    // SLIDE 9: VIỆC 06 (APS CHỦ TRÌ) - MỞ RỘNG KHO TRI THỨC APEC
    addSlide(`
      <div class="slide-header">
        <div class="badges">
          <span class="badge" style="color: #c084fc; border-color: rgba(168,85,247,.35); background: rgba(168,85,247,.12)">APS chủ trì</span>
          <span class="badge phase">Việc 06 · Cơ sở Tri thức</span>
        </div>
        <h2 class="slide-title">Chuẩn hóa & Mở rộng Kho Tri thức Sản phẩm APEC</h2>
        <p class="slide-subtitle">Mở rộng cơ sở dữ liệu tri thức nghiệp vụ từ các thông tin chung sang toàn bộ hệ sinh thái sản phẩm tài chính chuyên biệt của APEC.</p>
      </div>
      <div class="grid-2">
        <div class="card">
          <div class="tag-blue">Hiện trạng Dữ liệu (Đã có)</div>
          <h3>Kho Tài liệu Hiện tại</h3>
          <p>Hệ thống trợ lý AI đã được số hóa hoàn chỉnh và đối soát chính xác với:</p>
          <ul>
            <li><span class="dot">•</span> <strong>Cơ sở tri thức chuẩn hóa:</strong> Toàn bộ kho tài liệu nghiệp vụ, hướng dẫn và quy định của APS đã được xử lý và kiểm soát thông tin an toàn.</li>
            <li><span class="dot">•</span> <strong>Dữ liệu cổng thông tin <code>apec.com.vn</code>:</strong> Trung tâm hỗ trợ, Câu hỏi thường gặp FAQ, Kiến thức chung, Hướng dẫn giao dịch cổ phiếu / phái sinh.</li>
            <li><span class="dot">•</span> <strong>Bộ văn bản quy phạm pháp luật:</strong> Luật Chứng khoán, Nghị định 155/2020/NĐ-CP (trích dẫn chuẩn xác theo từng Điều, khoản).</li>
          </ul>
        </div>
        <div class="card">
          <div class="tag-green">Đề xuất Bổ sung từ APS</div>
          <h3>Dữ liệu Chuyên sâu Cần mở rộng</h3>
          <p>Đề xuất APS cử đầu mối cung cấp các bộ tài liệu nghiệp vụ nội bộ:</p>
          <ul>
            <li><span class="dot">•</span> <strong>Chính sách Margin & Biểu phí:</strong> Bảng lãi suất margin các gói T+, phí giao dịch phái sinh, danh mục chứng khoán được phép ký quỹ cập nhật.</li>
            <li><span class="dot">•</span> <strong>Sản phẩm tài chính APEC:</strong> Bộ tài liệu chính thức về Trái phiếu doanh nghiệp (Abond), Tích lũy tối ưu tiền nhàn rỗi (Asavings), Chứng quyền có bảo đảm (CW) và Hợp đồng hợp tác đầu tư.</li>
            <li><span class="dot">•</span> <strong>Báo cáo Nghiên cứu Phân tích (APS Research):</strong> Nạp các bản tin chiến lược tháng/quý, báo cáo định giá doanh nghiệp để bot trích dẫn khi khách hỏi phân tích sâu.</li>
          </ul>
        </div>
      </div>
      <div class="card" style="background: rgba(56,189,248,.06); border-color: rgba(56,189,248,.3); padding: 14px 18px; margin-top: 14px;">
        <h4 style="color:var(--accent); margin-bottom:2px;">⚡ Năng lực Xử lý Tri thức Sẵn sàng:</h4>
        <p style="color:var(--text); font-size:13.5px; margin:0;">Hệ thống lõi của FPT đã hoàn thiện 100% khả năng tiếp nhận và kiểm định dữ liệu an toàn. APS chỉ cần cung cấp tài liệu nghiệp vụ (PDF/Word), dữ liệu mới sẽ được tích hợp và sẵn sàng vận hành trong vòng 24 giờ.</p>
      </div>
    `, "Khẳng định: Năng lực xử lý tri thức tài chính của FPT đã hoàn thiện 100%. Khi APS bổ sung tài liệu các sản phẩm sinh lời cốt lõi như Trái phiếu Abond, Tích lũy tiền gửi Asavings, Chứng quyền CW..., trợ lý AI sẽ lập tức hỗ trợ bán chéo và giải đáp chi tiết điều khoản cho khách hàng.");

    // SLIDE 10: KẾ HOẠCH TRIỂN KHAI & HÀNH ĐỘNG
    addSlide(`
      <div class="slide-header">
        <div class="badges"><span class="badge">Lộ trình Thực thi</span></div>
        <h2 class="slide-title">Kế hoạch Hành động 4–6 Tuần & Quyết định Cần chốt</h2>
        <p class="slide-subtitle">Lộ trình triển khai tinh gọn, chia theo từng chặng rõ ràng nhằm đưa sản phẩm lên ứng dụng APS trong thời gian sớm nhất.</p>
      </div>
      <div class="card" style="padding:0; overflow:hidden; margin-bottom:16px;">
        <table class="timeline-table">
          <thead>
            <tr>
              <th style="width:20%">Giai đoạn</th>
              <th style="width:45%">Trọng tâm công việc</th>
              <th style="width:35%">Kết quả bàn giao (Deliverables)</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td><strong>Tuần 1 – 2<br><span style="color:var(--accent)">Chuẩn bị & Đánh giá</span></strong></td>
              <td>• FPT thực hiện benchmark so sánh các model LLM (độ chính xác & văn phong).<br>• BA & Chuyên gia APS rà soát câu trả lời, thiết kế prompt.<br>• Pháp chế chốt ranh giới tư vấn & tiêu chí so sánh mã.<br>• Thống nhất tài liệu API Core Trading & cơ chế Auth JWT.</td>
              <td>• Báo cáo đánh giá so sánh model LLM.<br>• Bộ Prompt & Quy tắc nghiệp vụ được duyệt.<br>• Tài liệu đặc tả API integration FPT-APS.</td>
            </tr>
            <tr>
              <td><strong>Tuần 3 – 4<br><span style="color:#c084fc">Tích hợp Kỹ thuật</span></strong></td>
              <td>• FPT dựng REST API & Webhook Notification.<br>• APS mở API đọc danh mục & nhúng khung chat vào App.<br>• Nạp tài liệu Margin, Abond, Asavings vào Kho tri thức.</td>
              <td>• Bản build App nội bộ có tính năng Chatbot.<br>• Kết nối thử nghiệm tài khoản chứng khoán thật.</td>
            </tr>
            <tr>
              <td><strong>Tuần 5 – 6<br><span style="color:#34d399">Pilot & Go-Live</span></strong></td>
              <td>• Đánh giá chất lượng trên Bộ câu hỏi Benchmark của APS.<br>• Vận hành luồng tiếp nhận Môi giới (Group Telegram hoặc CRM).<br>• Mở Pilot thử nghiệm cho 500 khách hàng thân thiết của APS.</td>
              <td>• Báo cáo đánh giá chất lượng đạt chuẩn.<br>• Phát hành chính thức trên App Store & Google Play.</td>
            </tr>
          </tbody>
        </table>
      </div>
      <div class="card" style="background: rgba(37,99,235,.08); border-color: rgba(56,189,248,.35);">
        <h4 style="color: #fff; margin-bottom: 2px;">⚡ 4 Quyết định Ban Lãnh đạo APS cần bấm nút khởi động:</h4>
        <p style="color: var(--text); font-size: 13.5px; line-height: 1.6;">
          1. <strong>Cử đầu mối BA & Chuyên gia Phân tích</strong> tham gia hoàn thiện câu trả lời và xây bộ câu hỏi kiểm thử chuẩn.<br>
          2. <strong>Phối hợp cùng FPT đánh giá văn phong</strong> & thẩm định kết quả so sánh các mô hình LLM thử nghiệm.<br>
          3. <strong>Giao Khối Kỹ thuật APS</strong> phối hợp với FPT mở API tài khoản thật và tiếp nhận REST API/Webhook.<br>
          4. <strong>Giao Khối Môi giới APS</strong> nghiên cứu đề xuất quy trình tiếp nhận và phân bổ lead khách hàng từ bot.
        </p>
      </div>
    `, "Kết luận: Kế hoạch 6 tuần hoàn toàn khả thi nếu hai bên chỉ định đầu mối rõ ràng. Đề xuất Lãnh đạo bấm nút khởi động 4 nhóm đầu mối ngay trong tuần tới.");

    // Điều hướng
    const slides = [...deck.querySelectorAll(".slide")];
    const counter = document.getElementById("counter");
    const progress = document.getElementById("progress-bar");
    const notesPanel = document.getElementById("notes-panel");
    const notesContent = document.getElementById("notes-content");
    let current = Math.min(Math.max(parseInt(location.hash.slice(1), 10) - 1 || 0, 0), slides.length - 1);

    function go(i) {
      if (i < 0 || i >= slides.length) return;
      current = i;
      slides.forEach((s, k) => {
        const active = k === i;
        s.classList.toggle("active", active);
        if (active) s.scrollTop = 0;
      });
      counter.textContent = `Slide ${pad(i + 1)} / ${pad(slides.length)}`;
      progress.style.width = `${(i / (slides.length - 1)) * 100}%`;
      notesContent.textContent = slides[i].dataset.notes || "Không có ghi chú cho slide này.";
      history.replaceState(null, "", `#${i + 1}`);
    }
    const toggleNotes = () => notesPanel.classList.toggle("open");
    function toggleFullScreen() {
      if (!document.fullscreenElement) document.documentElement.requestFullscreen().catch(() => {});
      else document.exitFullscreen().catch(() => {});
    }
    document.addEventListener("keydown", (e) => {
      const keys = {
        ArrowRight: () => go(current + 1), " ": () => go(current + 1), PageDown: () => go(current + 1),
        ArrowLeft: () => go(current - 1), PageUp: () => go(current - 1),
        Home: () => go(0), End: () => go(slides.length - 1),
        n: toggleNotes, N: toggleNotes, f: toggleFullScreen, F: toggleFullScreen,
      };
      if (keys[e.key]) { e.preventDefault(); keys[e.key](); }
    });
    go(current);
  </script>
</body>
</html>
