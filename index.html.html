<!DOCTYPE html>
<html lang="th">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>RSL Enhanced — Retail Space Leasing Intelligence (Thailand)</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&amp;family=Noto+Sans+Thai:wght@400;500;600;700;800&amp;display=swap" rel="stylesheet">
<script src="https://cdn.tailwindcss.com"></script>
<link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY=" crossorigin=""/>
<script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js" integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo=" crossorigin=""></script>
<style>
  html,body{font-family:'Inter','Noto Sans Thai',system-ui,sans-serif}
  .tab-active{background:#2563EB;color:#fff}
  .tab-inactive{color:#475569}
  .card{transition:all .2s}
  .card:hover{transform:translateY(-2px);box-shadow:0 10px 25px -5px rgb(0 0 0 / .12)}
  .pill{display:inline-flex;align-items:center;padding:.15rem .55rem;font-size:.7rem;border-radius:9999px;font-weight:600}
  .badge-green{background:#dcfce7;color:#166534}
  .badge-blue{background:#dbeafe;color:#1d4ed8}
  .badge-amber{background:#fef3c7;color:#92400e}
  .badge-red{background:#fee2e2;color:#991b1b}
  .badge-purple{background:#f3e8ff;color:#6b21a8}
  .badge-slate{background:#f1f5f9;color:#334155}
  .scrollbar-thin::-webkit-scrollbar{height:6px;width:6px}
  .scrollbar-thin::-webkit-scrollbar-thumb{background:#cbd5e1;border-radius:3px}
  details>summary{list-style:none;cursor:pointer}
  details>summary::-webkit-details-marker{display:none}
  .leaflet-popup-content{font-family:'Inter','Noto Sans Thai',sans-serif;margin:10px 12px}
  #map{height:calc(100vh - 220px);min-height:520px;border-radius:12px}
  .verify-tip{background:#fffbeb;border-left:3px solid #f59e0b;padding:8px 12px;font-size:.78rem;color:#78350f;border-radius:6px}
  .grid-row dt{color:#64748b;font-size:.78rem}
  .grid-row dd{color:#0f172a;font-weight:600;font-size:.86rem}
  .section-title{font-size:.78rem;text-transform:uppercase;letter-spacing:.05em;color:#64748b;font-weight:700;border-bottom:1px solid #e2e8f0;padding-bottom:6px;margin-bottom:10px}
  .modal-backdrop{position:fixed;inset:0;background:rgba(15,23,42,.55);z-index:60;display:none;align-items:flex-start;justify-content:center;padding:24px;overflow-y:auto}
  .modal-backdrop.open{display:flex}
  .modal{background:#fff;border-radius:16px;max-width:1100px;width:100%;box-shadow:0 25px 50px -12px rgb(0 0 0 / .4);max-height:90vh;overflow-y:auto}
  @media print{.no-print{display:none!important}}
</style>
</head>
<body class="bg-slate-50 text-slate-900 min-h-screen">

<!-- ============ HEADER ============ -->
<header class="sticky top-0 z-50 bg-white/95 backdrop-blur border-b border-slate-200 no-print">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="flex items-center justify-between h-14">
      <div class="flex items-center gap-2">
        <div class="w-8 h-8 rounded-lg bg-blue-600 flex items-center justify-center"><span class="text-white font-bold">R</span></div>
        <div>
          <div class="font-bold leading-none">RSL <span class="text-blue-600">Enhanced</span></div>
          <div class="text-[10px] text-slate-500 leading-none mt-0.5">Retail Space Leasing Intelligence · TH</div>
        </div>
      </div>
      <nav class="hidden md:flex items-center gap-1 text-sm">
        <button data-tab="discover" class="tab-btn px-3 py-1.5 rounded-full font-medium tab-active">Discover</button>
        <button data-tab="properties" class="tab-btn px-3 py-1.5 rounded-full font-medium tab-inactive">พื้นที่เช่า</button>
        <button data-tab="brands" class="tab-btn px-3 py-1.5 rounded-full font-medium tab-inactive">แบรนด์</button>
        <button data-tab="landlords" class="tab-btn px-3 py-1.5 rounded-full font-medium tab-inactive">ห้าง/Landlord</button>
        <button data-tab="map" class="tab-btn px-3 py-1.5 rounded-full font-medium tab-inactive">แผนที่</button>
        <button data-tab="match" class="tab-btn px-3 py-1.5 rounded-full font-medium tab-inactive">Match</button>
        <button data-tab="calc" class="tab-btn px-3 py-1.5 rounded-full font-medium tab-inactive">Calculator</button>
        <button data-tab="pitch" class="tab-btn px-3 py-1.5 rounded-full font-medium tab-inactive">Pitch Center</button>
      </nav>
      <div class="flex items-center gap-2">
        <button onclick="window.print()" class="hidden sm:inline-flex text-xs px-3 py-1.5 rounded-full bg-slate-100 hover:bg-slate-200">Print</button>
        <span class="text-xs text-slate-500 hidden lg:inline">v.1.0 · 2026</span>
      </div>
    </div>
    <nav class="md:hidden flex gap-1 pb-2 overflow-x-auto scrollbar-thin text-xs">
      <button data-tab="discover" class="tab-btn-m px-3 py-1.5 rounded-full whitespace-nowrap tab-active">Discover</button>
      <button data-tab="properties" class="tab-btn-m px-3 py-1.5 rounded-full whitespace-nowrap tab-inactive">พื้นที่</button>
      <button data-tab="brands" class="tab-btn-m px-3 py-1.5 rounded-full whitespace-nowrap tab-inactive">แบรนด์</button>
      <button data-tab="landlords" class="tab-btn-m px-3 py-1.5 rounded-full whitespace-nowrap tab-inactive">Landlord</button>
      <button data-tab="map" class="tab-btn-m px-3 py-1.5 rounded-full whitespace-nowrap tab-inactive">แผนที่</button>
      <button data-tab="match" class="tab-btn-m px-3 py-1.5 rounded-full whitespace-nowrap tab-inactive">Match</button>
      <button data-tab="calc" class="tab-btn-m px-3 py-1.5 rounded-full whitespace-nowrap tab-inactive">Calc</button>
      <button data-tab="pitch" class="tab-btn-m px-3 py-1.5 rounded-full whitespace-nowrap tab-inactive">Pitch</button>
    </nav>
  </div>
</header>

<main class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-6">

<!-- ============ DISCOVER ============ -->
<section data-section="discover" class="section">
  <div class="rounded-2xl bg-gradient-to-br from-blue-600 to-indigo-700 text-white p-6 sm:p-10 shadow-lg">
    <div class="grid md:grid-cols-2 gap-6 items-center">
      <div>
        <p class="text-xs uppercase tracking-widest text-blue-200 font-semibold">RSL · Retail Space Leasing</p>
        <h1 class="text-3xl sm:text-4xl font-extrabold mt-2 leading-tight">Marketplace + Intelligence<br/>สำหรับร้านค้า / ห้าง / นักลงทุน</h1>
        <p class="mt-3 text-blue-100 text-sm sm:text-base">รวมพื้นที่เช่าค้าปลีกทั่วไทย + Brand Directory + แผนที่คู่แข่ง<br/>ลดเวลา site selection จาก 3-6 เดือน → 2-4 สัปดาห์</p>
        <div class="flex flex-wrap gap-2 mt-5">
          <button onclick="switchTab('properties')" class="bg-white text-blue-700 hover:bg-blue-50 px-4 py-2 rounded-full text-sm font-semibold">ค้นหาพื้นที่เช่า</button>
          <button onclick="switchTab('brands')" class="bg-blue-500/40 hover:bg-blue-500/60 px-4 py-2 rounded-full text-sm font-semibold ring-1 ring-white/30">ดู Brand Directory</button>
          <button onclick="switchTab('map')" class="bg-blue-500/40 hover:bg-blue-500/60 px-4 py-2 rounded-full text-sm font-semibold ring-1 ring-white/30">เปิดแผนที่</button>
        </div>
      </div>
      <div class="grid grid-cols-2 gap-3 text-sm">
        <div class="bg-white/10 ring-1 ring-white/20 rounded-xl p-4"><div class="text-2xl font-extrabold" id="kpi-prop">—</div><div class="text-blue-200 text-xs">พื้นที่เช่าในระบบ</div></div>
        <div class="bg-white/10 ring-1 ring-white/20 rounded-xl p-4"><div class="text-2xl font-extrabold" id="kpi-brand">—</div><div class="text-blue-200 text-xs">แบรนด์ในฐานข้อมูล</div></div>
        <div class="bg-white/10 ring-1 ring-white/20 rounded-xl p-4"><div class="text-2xl font-extrabold" id="kpi-mall">—</div><div class="text-blue-200 text-xs">ห้าง / Landlord</div></div>
        <div class="bg-white/10 ring-1 ring-white/20 rounded-xl p-4"><div class="text-2xl font-extrabold" id="kpi-land">—</div><div class="text-blue-200 text-xs">ที่ดิน Retail-grade</div></div>
      </div>
    </div>
  </div>

  <div class="mt-6 grid lg:grid-cols-3 gap-4">
    <div class="bg-white rounded-xl border border-slate-200 p-5">
      <div class="flex items-center gap-3"><div class="w-10 h-10 bg-blue-100 text-blue-700 rounded-lg flex items-center justify-center text-xl">🏬</div><div><div class="font-bold">สำหรับแบรนด์ผู้เช่า</div><div class="text-xs text-slate-500">Tenant pitch</div></div></div>
      <p class="text-sm text-slate-600 mt-3">เปรียบเทียบทำเลโดยใช้ traffic, mall mix, ค่าเช่า/ตร.ม., เงื่อนไข 3+3 ปี เพื่อตัดสินใจขออนุมัติงบ</p>
      <button onclick="switchTab('properties')" class="text-blue-600 hover:underline text-xs font-semibold mt-3">เปิด Marketplace →</button>
    </div>
    <div class="bg-white rounded-xl border border-slate-200 p-5">
      <div class="flex items-center gap-3"><div class="w-10 h-10 bg-emerald-100 text-emerald-700 rounded-lg flex items-center justify-center text-xl">🏢</div><div><div class="font-bold">สำหรับห้าง / Landlord</div><div class="text-xs text-slate-500">Matchmaking</div></div></div>
      <p class="text-sm text-slate-600 mt-3">เปิดดูแบรนด์ที่กำลังหา expansion ในรัศมีของห้าง — match กับช่องว่างเช่าที่มี</p>
      <button onclick="switchTab('brands')" class="text-emerald-600 hover:underline text-xs font-semibold mt-3">ดูแบรนด์ →</button>
    </div>
    <div class="bg-white rounded-xl border border-slate-200 p-5">
      <div class="flex items-center gap-3"><div class="w-10 h-10 bg-purple-100 text-purple-700 rounded-lg flex items-center justify-center text-xl">📊</div><div><div class="font-bold">สำหรับนักลงทุน</div><div class="text-xs text-slate-500">Investor pitch</div></div></div>
      <p class="text-sm text-slate-600 mt-3">ดู TAM/SAM ตลาด retail leasing ไทย, business model, unit economics, traction</p>
      <button onclick="switchTab('pitch')" class="text-purple-600 hover:underline text-xs font-semibold mt-3">ดู Pitch Center →</button>
    </div>
  </div>

  <div class="mt-6">
    <h2 class="text-lg font-bold mb-3">🔥 Featured Spaces</h2>
    <div id="featured-grid" class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-3"></div>
  </div>

  <div class="mt-8 bg-white border border-slate-200 rounded-2xl p-5">
    <div class="flex items-start justify-between flex-wrap gap-3">
      <div>
        <h3 class="font-bold text-lg">📦 Export ข้อมูลทั้งหมด</h3>
        <p class="text-sm text-slate-600 mt-1">ดาวน์โหลด raw data (CSV/JSON) เพื่อนำเข้า database, Excel, หรือ BI tool ของตัวเอง</p>
      </div>
      <button onclick="exportData('all','json')" class="bg-purple-600 hover:bg-purple-700 text-white text-sm px-4 py-2 rounded-lg font-semibold">⬇ Download All (JSON)</button>
    </div>
    <div class="grid sm:grid-cols-2 lg:grid-cols-3 gap-3 mt-4">
      <div class="bg-slate-50 rounded-xl p-3">
        <div class="font-semibold text-sm mb-2">พื้นที่เช่า (Properties)</div>
        <div class="flex gap-2"><button onclick="exportData('properties','csv')" class="text-xs px-3 py-1.5 bg-blue-600 text-white rounded-lg hover:bg-blue-700">CSV</button><button onclick="exportData('properties','json')" class="text-xs px-3 py-1.5 bg-slate-200 text-slate-700 rounded-lg hover:bg-slate-300">JSON</button></div>
      </div>
      <div class="bg-slate-50 rounded-xl p-3">
        <div class="font-semibold text-sm mb-2">แบรนด์ (Brands)</div>
        <div class="flex gap-2"><button onclick="exportData('brands','csv')" class="text-xs px-3 py-1.5 bg-blue-600 text-white rounded-lg hover:bg-blue-700">CSV</button><button onclick="exportData('brands','json')" class="text-xs px-3 py-1.5 bg-slate-200 text-slate-700 rounded-lg hover:bg-slate-300">JSON</button></div>
      </div>
      <div class="bg-slate-50 rounded-xl p-3">
        <div class="font-semibold text-sm mb-2">Landlord / ห้าง</div>
        <div class="flex gap-2"><button onclick="exportData('landlords','csv')" class="text-xs px-3 py-1.5 bg-blue-600 text-white rounded-lg hover:bg-blue-700">CSV</button><button onclick="exportData('landlords','json')" class="text-xs px-3 py-1.5 bg-slate-200 text-slate-700 rounded-lg hover:bg-slate-300">JSON</button></div>
      </div>
      <div class="bg-slate-50 rounded-xl p-3">
        <div class="font-semibold text-sm mb-2">สาขาแบรนด์บนแผนที่</div>
        <div class="flex gap-2"><button onclick="exportData('stores','csv')" class="text-xs px-3 py-1.5 bg-blue-600 text-white rounded-lg hover:bg-blue-700">CSV</button><button onclick="exportData('stores','json')" class="text-xs px-3 py-1.5 bg-slate-200 text-slate-700 rounded-lg hover:bg-slate-300">JSON</button></div>
      </div>
      <div class="bg-slate-50 rounded-xl p-3">
        <div class="font-semibold text-sm mb-2">ห้าง (Mall Locations)</div>
        <div class="flex gap-2"><button onclick="exportData('malls','csv')" class="text-xs px-3 py-1.5 bg-blue-600 text-white rounded-lg hover:bg-blue-700">CSV</button><button onclick="exportData('malls','json')" class="text-xs px-3 py-1.5 bg-slate-200 text-slate-700 rounded-lg hover:bg-slate-300">JSON</button></div>
      </div>
      <div class="bg-slate-50 rounded-xl p-3">
        <div class="font-semibold text-sm mb-2">ที่ดินเปล่า (Land Plots)</div>
        <div class="flex gap-2"><button onclick="exportData('land','csv')" class="text-xs px-3 py-1.5 bg-blue-600 text-white rounded-lg hover:bg-blue-700">CSV</button><button onclick="exportData('land','json')" class="text-xs px-3 py-1.5 bg-slate-200 text-slate-700 rounded-lg hover:bg-slate-300">JSON</button></div>
      </div>
    </div>
  </div>

  <div class="mt-8 verify-tip">
    <strong>หมายเหตุข้อมูล:</strong> ตัวเลขสาขา / ขนาด / occupancy / contact ส่วนใหญ่อ้างอิงจากข้อมูลสาธารณะ (รายงานประจำปี, เว็บบริษัท, ข่าวธุรกิจ) อัปเดต ~2024-2025
    บางส่วนเป็นค่าประมาณการ / template — แนะนำให้ยืนยันก่อนใช้ในการพิชชิ่งจริง ค่าเช่า/CAM/Service เป็นเรทอ้างอิงตลาด ไม่ใช่ออเฟอร์อย่างเป็นทางการ
  </div>
</section>

<!-- ============ PROPERTIES (พื้นที่เช่า) ============ -->
<section data-section="properties" class="section hidden">
  <div class="flex flex-wrap items-end justify-between gap-3 mb-4">
    <div>
      <h2 class="text-2xl font-bold">พื้นที่เช่า · Retail Spaces</h2>
      <p class="text-sm text-slate-500">ห้าง · ตึกแถว · ที่ดินเปล่าสำหรับ retail (ทั่วประเทศไทย)</p>
    </div>
    <div class="flex flex-wrap gap-2">
      <input id="prop-search" placeholder="🔍 ค้นหาทำเล / ห้าง / เขต..." class="border border-slate-200 rounded-lg px-3 py-2 text-sm w-56"/>
      <select id="prop-type" class="border border-slate-200 rounded-lg px-3 py-2 text-sm">
        <option value="">ทุกประเภท</option><option value="mall">ห้าง</option><option value="standalone">ตึกแถว/Standalone</option><option value="kiosk">Kiosk</option><option value="land">ที่ดินเปล่า</option><option value="community">Community Mall</option>
      </select>
      <select id="prop-region" class="border border-slate-200 rounded-lg px-3 py-2 text-sm">
        <option value="">ทุกภูมิภาค</option><option value="bkk">กรุงเทพฯ/ปริมณฑล</option><option value="central">ภาคกลาง</option><option value="north">ภาคเหนือ</option><option value="northeast">อีสาน</option><option value="east">ภาคตะวันออก</option><option value="south">ภาคใต้</option>
      </select>
      <select id="prop-sort" class="border border-slate-200 rounded-lg px-3 py-2 text-sm">
        <option value="match">ตรงที่สุด</option><option value="price_asc">ราคา ต่ำ→สูง</option><option value="price_desc">ราคา สูง→ต่ำ</option><option value="size_asc">ขนาด เล็ก→ใหญ่</option><option value="size_desc">ขนาด ใหญ่→เล็ก</option>
      </select>
    </div>
  </div>
  <div id="prop-count" class="text-xs text-slate-500 mb-3"></div>
  <div id="prop-grid" class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-3"></div>
</section>

<!-- ============ BRANDS ============ -->
<section data-section="brands" class="section hidden">
  <div class="flex flex-wrap items-end justify-between gap-3 mb-4">
    <div>
      <h2 class="text-2xl font-bold">แบรนด์ · Tenant Directory</h2>
      <p class="text-sm text-slate-500">แบรนด์ที่กำลังขยายสาขาในไทย — F&amp;B · Fashion/Beauty · Mass/Specialty · Lifestyle</p>
    </div>
    <div class="flex flex-wrap gap-2">
      <input id="brand-search" placeholder="🔍 ชื่อแบรนด์ / parent..." class="border border-slate-200 rounded-lg px-3 py-2 text-sm w-56"/>
      <select id="brand-cat" class="border border-slate-200 rounded-lg px-3 py-2 text-sm">
        <option value="">ทุกหมวด</option><option>F&amp;B</option><option>Fashion</option><option>Beauty/Health</option><option>Lifestyle/Specialty</option><option>Electronics</option><option>Home/Furniture</option><option>Edutainment</option><option>Mass/Convenience</option>
      </select>
      <select id="brand-status" class="border border-slate-200 rounded-lg px-3 py-2 text-sm">
        <option value="">สถานะการขยาย</option><option value="active">Active scouting</option><option value="selective">Selective</option><option value="paused">Paused</option>
      </select>
      <select id="brand-format" class="border border-slate-200 rounded-lg px-3 py-2 text-sm">
        <option value="">รูปแบบร้าน</option><option>Kiosk</option><option>Inline</option><option>Flagship</option><option>Anchor</option>
      </select>
    </div>
  </div>
  <div id="brand-count" class="text-xs text-slate-500 mb-3"></div>
  <div id="brand-grid" class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-3"></div>
</section>

<!-- ============ LANDLORDS ============ -->
<section data-section="landlords" class="section hidden">
  <div class="flex flex-wrap items-end justify-between gap-3 mb-4">
    <div>
      <h2 class="text-2xl font-bold">ห้าง / Landlord</h2>
      <p class="text-sm text-slate-500">เครือศูนย์การค้าใหญ่ + Community mall + เจ้าของที่ดิน retail</p>
    </div>
    <div class="flex flex-wrap gap-2">
      <input id="ll-search" placeholder="🔍 ห้าง / เครือ / เขต..." class="border border-slate-200 rounded-lg px-3 py-2 text-sm w-56"/>
      <select id="ll-group" class="border border-slate-200 rounded-lg px-3 py-2 text-sm">
        <option value="">ทุกเครือ</option><option>CPN</option><option>Central Group</option><option>The Mall Group</option><option>Siam Piwat</option><option>MBK</option><option>Future Park</option><option>AWC</option><option>SF/IKANO</option><option>Index Living Mall</option><option>Lotus's</option><option>Big C</option><option>Independent</option>
      </select>
      <select id="ll-region" class="border border-slate-200 rounded-lg px-3 py-2 text-sm">
        <option value="">ทุกภาค</option><option value="bkk">กรุงเทพฯ/ปริมณฑล</option><option value="central">ภาคกลาง</option><option value="north">ภาคเหนือ</option><option value="northeast">อีสาน</option><option value="east">ภาคตะวันออก</option><option value="south">ภาคใต้</option>
      </select>
    </div>
  </div>
  <div id="ll-count" class="text-xs text-slate-500 mb-3"></div>
  <div id="ll-grid" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-3"></div>
</section>

<!-- ============ MAP ============ -->
<section data-section="map" class="section hidden">
  <div class="mb-3">
    <h2 class="text-2xl font-bold">แผนที่ · Retail Map</h2>
    <p class="text-sm text-slate-500">เลือกดู: พื้นที่เช่า · สาขาแบรนด์ · ห้าง · ที่ดิน — เปรียบเทียบระยะห่าง / คู่แข่ง / ความหนาแน่นของแบรนด์ตัวเอง</p>
  </div>
  <div class="grid lg:grid-cols-[300px_1fr] gap-4">
    <aside class="bg-white border border-slate-200 rounded-xl p-4 space-y-4 h-fit">
      <div>
        <div class="section-title">เลเยอร์</div>
        <label class="flex items-center gap-2 text-sm py-1"><input type="checkbox" id="layer-properties" checked> พื้นที่เช่า / Listings</label>
        <label class="flex items-center gap-2 text-sm py-1"><input type="checkbox" id="layer-malls" checked> ห้าง / Landlord</label>
        <label class="flex items-center gap-2 text-sm py-1"><input type="checkbox" id="layer-brand-stores"> สาขาแบรนด์</label>
        <label class="flex items-center gap-2 text-sm py-1"><input type="checkbox" id="layer-land"> ที่ดินเปล่า</label>
      </div>
      <div>
        <div class="section-title">กรองแบรนด์ (เมื่อเปิดเลเยอร์สาขา)</div>
        <input id="map-brand-search" placeholder="ค้นหาแบรนด์ เช่น After You..." class="w-full border border-slate-200 rounded-lg px-3 py-2 text-sm mb-2"/>
        <select id="map-brand-select" class="w-full border border-slate-200 rounded-lg px-3 py-2 text-sm" multiple size="6"></select>
        <p class="text-[11px] text-slate-500 mt-1">กด Ctrl/⌘ เพื่อเลือกหลายแบรนด์ — เปรียบเทียบคู่แข่ง vs. แบรนด์ตัวเอง</p>
      </div>
      <div>
        <div class="section-title">เครื่องมือ</div>
        <button id="tool-measure" class="w-full text-sm bg-slate-100 hover:bg-slate-200 px-3 py-2 rounded-lg mb-2">📏 วัดระยะห่าง (คลิก 2 จุด)</button>
        <button id="tool-clear" class="w-full text-sm bg-slate-100 hover:bg-slate-200 px-3 py-2 rounded-lg mb-2">🧹 ล้างการวัด</button>
        <button id="tool-recenter" class="w-full text-sm bg-blue-600 text-white hover:bg-blue-700 px-3 py-2 rounded-lg">🇹🇭 ดูทั้งประเทศ</button>
      </div>
      <div id="measure-result" class="hidden bg-blue-50 text-blue-700 text-sm rounded-lg px-3 py-2 font-semibold"></div>
    </aside>
    <div><div id="map"></div></div>
  </div>
</section>

<!-- ============ MATCH ============ -->
<section data-section="match" class="section hidden">
  <div class="mb-3">
    <h2 class="text-2xl font-bold">Match Scoring</h2>
    <p class="text-sm text-slate-500">จับคู่ <strong>แบรนด์ ↔ พื้นที่เช่า</strong> อัตโนมัติด้วยคะแนน 100 จุด — ลด time-to-decision ของทีม Site Selection</p>
  </div>
  <div class="bg-white rounded-2xl border border-slate-200 p-4 mb-4">
    <div class="flex flex-wrap gap-2 items-center">
      <span class="text-sm font-semibold">โหมด:</span>
      <button data-match-mode="b2u" class="match-mode-btn px-3 py-1.5 rounded-full text-xs font-semibold bg-blue-600 text-white">แบรนด์ → ยูนิตที่เหมาะสุด</button>
      <button data-match-mode="u2b" class="match-mode-btn px-3 py-1.5 rounded-full text-xs font-semibold bg-slate-100 text-slate-700">ยูนิต → แบรนด์ที่เหมาะสุด</button>
    </div>
    <div id="match-controls" class="mt-3"></div>
  </div>
  <div id="match-results"></div>
</section>

<!-- ============ DEAL CALCULATOR ============ -->
<section data-section="calc" class="section hidden">
  <div class="mb-3">
    <h2 class="text-2xl font-bold">Deal Calculator · 6-Year TCO + Breakeven</h2>
    <p class="text-sm text-slate-500">คำนวณต้นทุน-รายได้รายปี สำหรับขออนุมัติงบ + ดู breakeven month</p>
  </div>
  <div class="grid lg:grid-cols-[380px_1fr] gap-4">
    <aside class="bg-white border border-slate-200 rounded-2xl p-5 space-y-4 h-fit">
      <div>
        <div class="section-title">เลือกพื้นที่ (Auto-fill)</div>
        <select id="calc-prop" class="w-full border border-slate-200 rounded-lg px-3 py-2 text-sm">
          <option value="">— ใส่ค่ามือเอง —</option>
        </select>
      </div>
      <div class="grid grid-cols-2 gap-3">
        <div><div class="text-xs text-slate-600 mb-1">ขนาด (ตร.ม.)</div><input id="ci-size" type="number" value="120" class="w-full border border-slate-200 rounded-lg px-3 py-2 text-sm"/></div>
        <div><div class="text-xs text-slate-600 mb-1">ค่าเช่า/เดือน (฿)</div><input id="ci-rent" type="number" value="180000" class="w-full border border-slate-200 rounded-lg px-3 py-2 text-sm"/></div>
        <div><div class="text-xs text-slate-600 mb-1">ค่าบริการ/เดือน (฿)</div><input id="ci-service" type="number" value="18000" class="w-full border border-slate-200 rounded-lg px-3 py-2 text-sm"/></div>
        <div><div class="text-xs text-slate-600 mb-1">CAM/เดือน (฿)</div><input id="ci-cam" type="number" value="12000" class="w-full border border-slate-200 rounded-lg px-3 py-2 text-sm"/></div>
        <div><div class="text-xs text-slate-600 mb-1">เงินประกัน (เดือน)</div><input id="ci-deposit" type="number" value="6" class="w-full border border-slate-200 rounded-lg px-3 py-2 text-sm"/></div>
        <div><div class="text-xs text-slate-600 mb-1">Escalation %/ปี</div><input id="ci-esc" type="number" value="5" class="w-full border border-slate-200 rounded-lg px-3 py-2 text-sm"/></div>
        <div><div class="text-xs text-slate-600 mb-1">ระยะสัญญา (ปี)</div><input id="ci-term" type="number" value="6" class="w-full border border-slate-200 rounded-lg px-3 py-2 text-sm"/></div>
        <div><div class="text-xs text-slate-600 mb-1">Fit-out (เดือน)</div><input id="ci-fitout" type="number" value="2" class="w-full border border-slate-200 rounded-lg px-3 py-2 text-sm"/></div>
      </div>
      <div>
        <div class="section-title mt-2">CAPEX & Revenue</div>
        <div class="grid grid-cols-2 gap-3">
          <div><div class="text-xs text-slate-600 mb-1">CAPEX ตกแต่ง (฿/ตร.ม.)</div><input id="ci-capex" type="number" value="35000" class="w-full border border-slate-200 rounded-lg px-3 py-2 text-sm"/></div>
          <div><div class="text-xs text-slate-600 mb-1">รายได้/เดือน (฿)</div><input id="ci-rev" type="number" value="900000" class="w-full border border-slate-200 rounded-lg px-3 py-2 text-sm"/></div>
          <div><div class="text-xs text-slate-600 mb-1">COGS %</div><input id="ci-cogs" type="number" value="35" class="w-full border border-slate-200 rounded-lg px-3 py-2 text-sm"/></div>
          <div><div class="text-xs text-slate-600 mb-1">Payroll/เดือน (฿)</div><input id="ci-payroll" type="number" value="180000" class="w-full border border-slate-200 rounded-lg px-3 py-2 text-sm"/></div>
          <div><div class="text-xs text-slate-600 mb-1">Util/Misc/เดือน (฿)</div><input id="ci-misc" type="number" value="40000" class="w-full border border-slate-200 rounded-lg px-3 py-2 text-sm"/></div>
          <div><div class="text-xs text-slate-600 mb-1">Revenue growth %/ปี</div><input id="ci-rg" type="number" value="6" class="w-full border border-slate-200 rounded-lg px-3 py-2 text-sm"/></div>
        </div>
      </div>
      <button id="calc-run" class="w-full bg-blue-600 hover:bg-blue-700 text-white px-4 py-2 rounded-lg font-semibold">คำนวณ</button>
      <button id="calc-export" class="w-full bg-slate-100 hover:bg-slate-200 text-slate-700 px-4 py-2 rounded-lg text-sm">⬇ Export CSV</button>
    </aside>
    <div id="calc-out" class="space-y-4"></div>
  </div>
</section>

<!-- ============ PITCH CENTER ============ -->
<section data-section="pitch" class="section hidden">
  <h2 class="text-2xl font-bold mb-1">Pitch Center</h2>
  <p class="text-sm text-slate-500 mb-4">เอกสาร / Talking points สำหรับ 3 กลุ่มผู้ฟัง — แก้ไขในไฟล์ก่อนนำเสนอจริง</p>
  <div class="flex gap-2 mb-4">
    <button data-pitch="brand" class="pitch-btn px-4 py-2 rounded-full text-sm font-semibold bg-blue-600 text-white">🏬 พิชชิ่งกับแบรนด์</button>
    <button data-pitch="landlord" class="pitch-btn px-4 py-2 rounded-full text-sm font-semibold bg-slate-100 text-slate-700">🏢 พิชชิ่งกับห้าง</button>
    <button data-pitch="investor" class="pitch-btn px-4 py-2 rounded-full text-sm font-semibold bg-slate-100 text-slate-700">📊 พิชชิ่งกับนักลงทุน</button>
  </div>
  <div id="pitch-content" class="bg-white rounded-2xl border border-slate-200 p-6"></div>
</section>

</main>

<footer class="border-t border-slate-200 bg-white mt-10 no-print">
  <div class="max-w-7xl mx-auto px-4 py-6 text-xs text-slate-500 flex flex-wrap items-center justify-between gap-2">
    <div>© RSL Enhanced · Retail Space Leasing Intelligence — Demo Version</div>
    <div>ข้อมูลเชิงสาธารณะ + ตัวอย่าง template — ยืนยันก่อนใช้พิชชิ่งจริง</div>
  </div>
</footer>

<!-- ============ MODAL ============ -->
<div id="modal" class="modal-backdrop" onclick="if(event.target===this)closeModal()">
  <div class="modal" id="modal-body"></div>
</div>

<script>
/* =========================================================
   DATA · LANDLORDS (Malls / Mall Groups / Land owners)
   ข้อมูลสาธารณะที่รวบรวมได้ + บางส่วนเป็นค่าประมาณการ
   ========================================================= */
const LANDLORDS = [
 {id:'cpn',name:'Central Pattana (CPN)',type:'Mall Operator',group:'CPN',
   hq:'CentralWorld Office Tower, ปทุมวัน, กรุงเทพฯ',
   web:'centralpattana.co.th',
   contact:{leasing:'leasing@cpn.co.th',phone:'02-021-9999',ir:'ir@cpn.co.th'},
   portfolio:'41+ ศูนย์การค้าทั่วประเทศ + 18 community/mixed-use + 11 อาคารสำนักงาน + Robinson 50+ สาขา',
   gla:'~2.4M ตร.ม. (รวมเครือ)',
   notes:'เครือใหญ่สุดในไทย รวม CentralWorld, CentralPlaza, CentralFestival, Robinson Lifestyle Center, Central Embassy (ผ่าน Central Group), บริหารโดย Central Group',
   keyMalls:['CentralWorld','CentralPlaza Ladprao','CentralPlaza Pinklao','CentralPlaza Bangna','CentralPlaza Rama 2','CentralPlaza Rama 3','CentralPlaza Rama 9','CentralPlaza Chaengwattana','CentralPlaza WestVille','CentralPlaza Eastville','CentralFestival EastVille','CentralFestival Pattaya Beach','CentralFestival Phuket Floresta','CentralFestival Chiangmai','CentralFestival Hatyai','CentralFestival Samui','CentralPlaza Khonkaen','CentralPlaza Udonthani','Central Ayutthaya','Central Korat','Central Si Racha','Central Surat Thani','Central Nakhon Sawan']
 },
 {id:'central-grp',name:'Central Group (Retail)',type:'Mall + Anchor Operator',group:'Central Group',
   hq:'Central Embassy Office, ปทุมวัน',
   web:'centralgroup.com',contact:{leasing:'corporate@central.co.th',phone:'02-650-1700'},
   portfolio:'Central Embassy (luxury), Central Chidlom (department store), Central Department Store ~24 สาขา, ZEN, Robinson, supersports, B2S, OfficeMate, Tops, Power Buy',
   notes:'แยกบริหารพื้นที่ห้างจาก CPN — Central Embassy เป็น flagship luxury (~80,000 ตร.ม.)',
   keyMalls:['Central Embassy','Central Chidlom','Central Bangna Annex']
 },
 {id:'themall',name:'The Mall Group',type:'Mall Operator',group:'The Mall Group',
   hq:'The Mall Ramkhamhaeng, กรุงเทพฯ',
   web:'themallgroup.com',contact:{leasing:'leasing@themall.co.th',phone:'02-310-1000'},
   portfolio:'7 ห้างหลัก: Emporium, EmQuartier, EmSphere, Siam Paragon (JV Siam Piwat), Bluport Hua Hin, The Mall Bangkapi, The Mall Bangkae, The Mall Ngamwongwan, The Mall Thapra (รวม ~1.1M ตร.ม.)',
   gla:'~1.1M ตร.ม.',
   notes:'EmSphere เปิด 2023 ขนาด ~200,000 ตร.ม., แผน redevelopment The Mall Bangkapi / Bangkae / Thapra เป็น Bangkok Mall (2026-2027)',
   keyMalls:['Siam Paragon','Emporium','EmQuartier','EmSphere','The Mall Bangkapi','The Mall Bangkae','The Mall Ngamwongwan','The Mall Thapra','Bluport Hua Hin']
 },
 {id:'siampiwat',name:'Siam Piwat',type:'Mall Operator',group:'Siam Piwat',
   hq:'Siam Tower, ปทุมวัน',
   web:'siampiwat.com',contact:{leasing:'corporateaffairs@siampiwat.com',phone:'02-658-1000'},
   portfolio:'ICONSIAM (750,000 ตร.ม.), Siam Paragon (JV The Mall), Siam Center, Siam Discovery, Siam Premium Outlets Bangkok (JV Simon Property)',
   notes:'Anchor: Siam Quarter — มี Apple Store แห่งแรกในไทย (Iconsiam) และ Apple Central World; ตำแหน่ง flagship destination ที่นักท่องเที่ยวสูง',
   keyMalls:['ICONSIAM','Siam Paragon','Siam Center','Siam Discovery','Siam Premium Outlets Bangkok']
 },
 {id:'mbk',name:'MBK Group',type:'Mall Operator',group:'MBK',
   hq:'MBK Center, ปทุมวัน',
   web:'mbkgroup.co.th',contact:{leasing:'leasing@mbk-center.co.th',phone:'02-853-9000'},
   portfolio:'MBK Center (~89,000 ตร.ม.), Paradise Park (Srinakarin), The Nine (Rama 9), Glasshaus Ratchada',
   notes:'จุดเด่น: อายุห้างเก่าแก่ ลูกค้านักท่องเที่ยวสูง — กำลังปรับ tenant mix สู่ Gen Z/lifestyle',
   keyMalls:['MBK Center','Paradise Park','The Nine Center']
 },
 {id:'futurepark',name:'Future Park / Zpell',type:'Mall Operator',group:'Future Park',
   hq:'Future Park Rangsit, ปทุมธานี',
   web:'futurepark.co.th',contact:{leasing:'leasing@futurepark.co.th',phone:'02-958-0011'},
   portfolio:'Future Park Rangsit (~500,000 ตร.ม., 600+ ร้าน) + Zpell',
   notes:'ห้างใหญ่ที่สุดในปริมณฑลเหนือ — traffic 200,000+/วัน',
   keyMalls:['Future Park Rangsit','Zpell']
 },
 {id:'mega',name:'Mega Bangna (SF + IKANO)',type:'Mall Operator',group:'SF/IKANO',
   hq:'Mega Bangna, บางพลี สมุทรปราการ',
   web:'mega-bangna.com',contact:{leasing:'leasing@mega-bangna.com',phone:'02-105-1000'},
   portfolio:'Mega Bangna (~400,000 ตร.ม., 800+ ร้าน), Mega City (อยู่ระหว่างขยาย Phase 2)',
   notes:'IKEA Bangna anchor ตัวแรกในไทย, รวม Big C Extra, Major Cineplex, HomePro, Robinson',
   keyMalls:['Mega Bangna']
 },
 {id:'awc',name:'AWC (Asset World Corporation)',type:'Mall + Retail',group:'AWC',
   hq:'Empire Tower, สาทร',
   web:'assetworldcorp-th.com',contact:{leasing:'info@awc.co.th',phone:'02-679-6444'},
   portfolio:'Asiatique The Riverfront, Pantip Plaza Pratunam/Ngamwongwan, Tawanna Bangkapi, Gateway Ekamai',
   notes:'แผนพัฒนา Asiatique เป็น destination ใหม่ + Aquatique (2026+)',
   keyMalls:['Asiatique The Riverfront','Gateway Ekamai','Tawanna Bangkapi','Pantip Plaza Pratunam']
 },
 {id:'index-living',name:'Index Living Mall',type:'Specialty Mall (Furniture)',group:'Index Living Mall',
   hq:'Index Living Mall HQ, ลาดพร้าว',
   web:'indexlivingmall.com',contact:{leasing:'corporate@indexlivingmall.com',phone:'02-833-0555'},
   portfolio:'30+ สาขาทั่วประเทศ + บาง standalone retail (ตัวอย่าง: Index Bangkae, Index Rama 2)',
   notes:'ส่วนใหญ่เป็น destination store ของตนเอง — บางสาขามี sub-tenant',
   keyMalls:[]
 },
 {id:'sf','name':'SF Holding (SFC)',type:'Mall + Cinema Operator',group:'SF/IKANO',
   hq:'SF World Cinema, CentralWorld',
   web:'sfcinema.com',contact:{leasing:'leasing@sfcinema.com',phone:'02-268-8888'},
   portfolio:'Mega Bangna (JV), Major Cineplex JVs, Maya Lifestyle Shopping Center Chiangmai',
   notes:'',keyMalls:['Maya Lifestyle Chiangmai']
 },
 {id:'major',name:'Major Cineplex Group',type:'Cinema + small mall',group:'Major',
   hq:'Major Tower รัชโยธิน',
   web:'majorcineplexgroup.com',contact:{leasing:'leasing@majorcineplex.com',phone:'02-515-5300'},
   portfolio:'Major Ratchayothin, Major Sukhumvit, EGV, Major Avenue Ratchayothin, Esplanade Ratchadapisek, Major @ Quartier',
   notes:'',keyMalls:['Esplanade Ratchadapisek','Major Avenue Ratchayothin']
 },
 {id:'lotus',name:"Lotus's (CP Group)",type:'Hypermarket+Mall',group:"Lotus's",
   hq:'Sathorn, กรุงเทพฯ',
   web:'lotuss.com',contact:{leasing:'mall.leasing@lotuss.com',phone:'02-797-9000'},
   portfolio:'~220 hypermarkets + 1,800+ Lotus’s go fresh + Lotus’s Mall format (เช่น Lotus’s Rama 1, Lotus’s Rangsit, Lotus’s North Pattaya)',
   notes:'อยู่ระหว่างปรับ tenant mix สู่ lifestyle community — พื้นที่ให้เช่า inline shop และ kiosk เยอะ',
   keyMalls:["Lotus's North Ratchadapisek","Lotus's Rama 1","Lotus's Rangsit","Lotus's Pattaya North","Lotus's Sukhumvit 50"]
 },
 {id:'bigc',name:'Big C / Berli Jucker (TCC)',type:'Hypermarket+Mall',group:'Big C',
   hq:'อาคาร Berli Jucker, คลองเตย',
   web:'bigc.co.th',contact:{leasing:'leasing@bigc.co.th',phone:'02-655-0666'},
   portfolio:'150+ Big C + Big C Place mall format + Big C Mini convenience',
   notes:'TCC Group ของเจ้าสัวเจริญ — ลงทุนต่อเนื่องด้าน community retail',
   keyMalls:['Big C Ratchadamri','Big C Saphan Khwai','Big C Bangna']
 },
 {id:'amarin',name:'Amarin Plaza',type:'Mall',group:'Independent',
   hq:'ราชดำริ, ปทุมวัน',
   web:'amarinplaza.com',contact:{leasing:'leasing@amarinplaza.com',phone:'02-650-4704'},
   portfolio:'Amarin Plaza (~28,000 ตร.ม.) ใจกลาง Ratchaprasong',notes:'',keyMalls:['Amarin Plaza']
 },
 {id:'gaysorn',name:'Gaysorn Property',type:'Luxury Mall',group:'Independent',
   hq:'Gaysorn Village, ปทุมวัน',
   web:'gaysornvillage.com',contact:{leasing:'leasing@gaysornproperty.com',phone:'02-656-1149'},
   portfolio:'Gaysorn Village (luxury mall ~26,000 ตร.ม.), Gaysorn Amarin, Gaysorn Tower',
   notes:'Target: luxury / hi-end accessories, watches, fine dining',keyMalls:['Gaysorn Village','Gaysorn Amarin']
 },
 {id:'pier21',name:'Terminal 21 (LH Mall)',type:'Mall',group:'Land & Houses Mall',
   hq:'Terminal 21 Asok, วัฒนา',
   web:'terminal21.co.th',contact:{leasing:'info@terminal21.co.th',phone:'02-108-0888'},
   portfolio:'Terminal 21 Asok (~60,000 ตร.ม.), Terminal 21 Korat, Terminal 21 Pattaya, Terminal 21 Rama 3',
   notes:'',keyMalls:['Terminal 21 Asok','Terminal 21 Korat','Terminal 21 Pattaya','Terminal 21 Rama 3']
 },
 {id:'sho',name:'Show DC',type:'Mall',group:'Independent',
   hq:'Show DC พระราม 9',
   web:'showdcoasis.com',contact:{leasing:'leasing@showdcoasis.com'},
   portfolio:'Show DC (Pet/lifestyle/entertainment positioning)',notes:'',keyMalls:['Show DC']
 },
 {id:'season',name:'CDC / Crystal Design Center',type:'Specialty Lifestyle Mall',group:'Independent',
   hq:'CDC ประดิษฐ์มนูธรรม',web:'crystaldesigncenter.com',contact:{leasing:'leasing@cdc.co.th',phone:'02-101-5999'},
   portfolio:'CDC (~57,000 ตร.ม.), The Crystal PTT Ekamai-Ramintra, The Crystal SB Ratchaphruek, Plearnary Mall',
   notes:'Lifestyle community mall positioning — F&B + furniture/design heavy',
   keyMalls:['CDC Crystal Design Center','The Crystal Ekamai-Ramintra','The Crystal SB Ratchaphruek','Plearnary Mall']
 },
 {id:'gateway',name:'Gateway Mall (JLL/AWC)',type:'Mall',group:'AWC',
   hq:'Gateway Ekamai',contact:{leasing:'info@gatewayekamai.com'},
   portfolio:'Gateway Ekamai (~38,000 ตร.ม., Japanese town positioning)',notes:'',keyMalls:['Gateway Ekamai','Gateway Bangsue']
 },
 {id:'season-mall','name':'Seacon Group',type:'Mall',group:'Independent',
   hq:'Seacon Square, ศรีนครินทร์',web:'seaconsquare.com',contact:{leasing:'leasing@seaconsquare.com',phone:'02-721-8888'},
   portfolio:'Seacon Square Srinakarin (~500,000 ตร.ม., ใหญ่ที่สุดในเอเชียตะวันออกเฉียงใต้ในขณะที่สร้าง), Seacon Bangkae',
   notes:'',keyMalls:['Seacon Square Srinakarin','Seacon Bangkae']
 },
 {id:'fashion-island',name:'Fashion Island Group',type:'Mall',group:'Independent',
   hq:'Fashion Island, มีนบุรี',web:'fashionisland.co.th',contact:{leasing:'leasing@fashionisland.co.th',phone:'02-947-5000'},
   portfolio:'Fashion Island Ramintra, The Promenade Ramintra, Terminal Hall Ramintra (ใหม่)',notes:'',keyMalls:['Fashion Island','The Promenade Ramintra']
 },
 {id:'silom-complex',name:'Silom Complex (CPN)',type:'Mall',group:'CPN',
   hq:'Silom Complex, บางรัก',contact:{leasing:'leasing@cpn.co.th'},
   portfolio:'Silom Complex (~38,000 ตร.ม., รีโนเวทใหม่ 2022)',notes:'',keyMalls:['Silom Complex']
 },
 {id:'union-mall',name:'Union Mall',type:'Mall',group:'Independent',
   hq:'Union Mall, ลาดพร้าว',web:'unionmall.co.th',contact:{leasing:'leasing@unionmall.co.th',phone:'02-512-5111'},
   portfolio:'Union Mall (~80,000 ตร.ม., wholesale fashion positioning)',notes:'',keyMalls:['Union Mall']
 },
 {id:'platinum',name:'Platinum Fashion Mall',type:'Wholesale Mall',group:'Independent',
   hq:'Platinum Fashion Mall, ราชเทวี',web:'platinumfashionmall.com',contact:{leasing:'leasing@platinumfashionmall.com',phone:'02-121-8000'},
   portfolio:'Platinum Fashion Mall (~110,000 ตร.ม., 4,000+ ร้านขายส่ง)',notes:'',keyMalls:['Platinum Fashion Mall']
 },
 {id:'terminalhall',name:'Index Mall (Index Living Mall)',type:'Anchor specialty',group:'Index Living Mall',
   hq:'หลายสาขาทั่วประเทศ',contact:{leasing:'corporate@indexlivingmall.com'},
   portfolio:'30+ สาขา anchor / standalone',notes:'',keyMalls:[]
 }
];

/* land plots (vacant retail-grade) — ตัวอย่าง template ที่พบบ่อยจากนายหน้า */
const LAND_PLOTS = [
  {id:'land-bangna',title:'ที่ดินติด ถ.บางนา-ตราด กม.5',area:'8 ไร่',price:'฿180,000/ตร.ว./ปี (เช่า) หรือซื้อ',lat:13.6648,lng:100.6481,owner:'นายหน้าอิสระ',contact:'(ตัวอย่าง) ติดต่อนายหน้า — ยืนยันก่อนใช้',use:'Standalone retail, community mall, supermarket'},
  {id:'land-bangyai',title:'ที่ดินใกล้ MRT บางใหญ่',area:'12 ไร่',price:'เช่า 30 ปี',lat:13.8589,lng:100.4232,owner:'เจ้าของรายเดียว',contact:'(ตัวอย่าง template)',use:'Community mall, big-box'},
  {id:'land-pakchong',title:'ที่ดิน Khao Yai (เขาใหญ่)',area:'15 ไร่',price:'฿8M/ไร่ (ซื้อ)',lat:14.6486,lng:101.4196,owner:'ส่วนบุคคล',contact:'(ตัวอย่าง template)',use:'Resort retail, lifestyle outlet'},
  {id:'land-phuket-cherngtalay',title:'ที่ดินเชิงทะเล ภูเก็ต',area:'5 ไร่',price:'฿25M/ไร่',lat:7.9943,lng:98.2954,owner:'นายหน้า',contact:'(ตัวอย่าง template)',use:'Boutique mall, F&B cluster'},
  {id:'land-hua-hin',title:'ที่ดินติด ถ.เพชรเกษม หัวหิน',area:'4 ไร่',price:'฿15M/ไร่',lat:12.5684,lng:99.9577,owner:'ส่วนบุคคล',contact:'(ตัวอย่าง template)',use:'Strip mall, F&B'},
  {id:'land-chiangmai-sankampaeng',title:'ที่ดินสันกำแพง เชียงใหม่',area:'10 ไร่',price:'฿5M/ไร่',lat:18.7530,lng:99.1186,owner:'ส่วนบุคคล',contact:'(ตัวอย่าง template)',use:'Tourist retail, lifestyle outlet'},
];

/* =========================================================
   DATA · BRANDS (Tenants directory)
   ตัวเลขสาขา/แผน expansion อ้างอิงจากข้อมูลเปิดเผยและสื่อ
   ========================================================= */
const BRANDS = [
  // ===== F&B =====
  {id:'afteryou',name:'After You',cat:'F&B',sub:'Dessert Cafe',parent:'After You PCL (SET: AU)',
    country:'TH',since:2007,branches:{total:'~50',bkk:'~35',upcountry:'~15',overseas:'0'},
    expansion:'5-7 สาขา/ปี · ขยาย mall tier 2-3 + standalone destination · เริ่ม overseas (HK, Japan kiosks)',
    format:['Inline','Flagship'],size:'80-200 ตร.ม.',rentBudget:'฿1,500-3,500/ตร.ม./เดือน',
    siteCriteria:'Mall ระดับ A-B, ground/F1, ใกล้ supermarket หรือ cinema lobby, traffic 30k+/วัน',
    target:'Gen Z-Millennial, female 70%, avg ticket ฿250-400',
    bd:{name:'BD/Real Estate Team',email:'corporate@afteryoudessert.com',phone:'02-129-4598',hq:'กรุงเทพฯ'},
    status:'active',notes:'IPO 2016, ขยายสู่ retail products + delivery'},
  {id:'cafe-amazon',name:'Café Amazon',cat:'F&B',sub:'Coffee Shop',parent:'OR (SET: OR) — PTTOR',
    country:'TH',since:2002,branches:{total:'4,200+',bkk:'~600',upcountry:'~3,600',overseas:'400+ (CN, MY, SG, KH, LA, OM, JP)'},
    expansion:'300-500 สาขา/ปี (เป้า 5,500 ภายในปี 2027)',
    format:['Kiosk','Inline','Flagship Concept Store'],size:'30-300 ตร.ม.',rentBudget:'฿600-1,800/ตร.ม./เดือน (mall); GP-share สำหรับ standalone in PTT Station',
    siteCriteria:'ปั๊ม PTT, mall ทุก tier, hospital, office building',
    target:'mass market all-day, avg ฿55-120',
    bd:{name:'OR Retail Business Development',email:'cafeamazon.bd@pttor.com',phone:'02-196-5959',hq:'OR HQ, เอ็นเนอร์ยี่ คอมเพล็กซ์ จตุจักร'},status:'active',notes:'Coffee chain ใหญ่สุดของ SEA โดยจำนวนสาขา'},
  {id:'starbucks',name:'Starbucks (TH)',cat:'F&B',sub:'Coffee Shop',parent:'Coffee Concepts (Thailand) — Starbucks Coffee International',
    country:'TH/Global',since:1998,branches:{total:'~500',bkk:'~280',upcountry:'~220',overseas:'-'},
    expansion:'30-40 สาขา/ปี · เน้น drive-thru + reserve bar concept',
    format:['Inline','Flagship','Drive-Thru','Reserve'],size:'120-450 ตร.ม.',rentBudget:'฿1,200-3,000/ตร.ม./เดือน',
    siteCriteria:'Mall A, office tower, BTS/MRT station, ทำเลกลางเมือง + tourist',target:'White-collar, ฿120-220',
    bd:{name:'Real Estate & New Store Development',email:'TH.realestate@starbucks.com',phone:'02-339-0500',hq:'กรุงเทพฯ'},status:'active'},
  {id:'mk',name:'MK Restaurants',cat:'F&B',sub:'Hot Pot/Thai-Sukiyaki',parent:'M Foods (SET: M)',
    country:'TH',since:1986,branches:{total:'~460 (MK Suki) + ~190 Yayoi + 32 Hot Yum + อื่นๆ',bkk:'~200',upcountry:'~260',overseas:'~50 (JP, VN, SG, MY)'},
    expansion:'20-30 สาขา/ปี รวมทั้งเครือ',format:['Inline','Anchor F&B','Drive-Thru'],size:'150-400 ตร.ม.',
    rentBudget:'฿700-1,500/ตร.ม./เดือน',siteCriteria:'Family mall, community mall, hypermarket',target:'Family 35+, avg ฿380/คน',
    bd:{name:'Property Development',email:'bd@mkrestaurant.com',phone:'02-248-0033',hq:'กรุงเทพฯ'},status:'active'},
  {id:'sushiro',name:'Sushiro',cat:'F&B',sub:'Conveyor Sushi',parent:'Food and Life Companies (JP) + พันธมิตร TH',
    country:'TH/Global',since:2021,branches:{total:'~50+',bkk:'~32',upcountry:'~18'},
    expansion:'10-15 สาขา/ปี · ขยายต่างจังหวัด tier 2',
    format:['Inline','Anchor F&B'],size:'180-300 ตร.ม.',rentBudget:'฿1,000-2,000/ตร.ม./เดือน',
    siteCriteria:'Mall A-B, ใกล้ cinema/family zone',target:'Family + young office, avg ฿380',
    bd:{name:'Sushiro Thailand BD',email:'th-info@food-and-life.com',hq:'กรุงเทพฯ'},status:'active'},
  {id:'bonchon',name:'Bonchon',cat:'F&B',sub:'Korean Fried Chicken',parent:'Minor Food Group',
    country:'TH',since:2011,branches:{total:'~100+',bkk:'~60',upcountry:'~40'},
    expansion:'15-20 สาขา/ปี',format:['Inline','Kiosk (delivery hub)'],size:'80-200 ตร.ม.',
    rentBudget:'฿1,000-2,200/ตร.ม./เดือน',siteCriteria:'Mall A-B, community mall, office area',target:'Young 18-35, avg ฿250',
    bd:{name:'Minor Food Real Estate',email:'realestate@minor.com',phone:'02-365-7500',hq:'Anantara Bangkok Riverside (Minor HQ)'},status:'active'},
  {id:'minor',name:'Minor Food (Pizza Co/Swensen\'s/Sizzler/Dairy Queen/Burger King/The Coffee Club)',
    cat:'F&B',sub:'Multi-Brand Restaurant Group',parent:'Minor International (SET: MINT)',
    country:'TH/Global',since:1980,
    branches:{total:'2,400+ (TH+SEA+CN); ในไทย ~1,500',bkk:'~600',upcountry:'~900',overseas:'900+'},
    expansion:'150-200 สาขา/ปี ทั่วเครือ',format:['Kiosk','Inline','Anchor F&B','Drive-Thru'],size:'30-400 ตร.ม.',
    rentBudget:'฿600-2,500/ตร.ม./เดือน (แล้วแต่แบรนด์)',siteCriteria:'หลากหลายตาม sub-brand',target:'Mass to upscale',
    bd:{name:'Real Estate & Development',email:'realestate@minor.com',phone:'02-365-7500',hq:'Anantara Riverside'},status:'active'},
  {id:'crg',name:'CRG (Central Restaurants Group)',cat:'F&B',sub:'Multi-Brand (KFC, Mister Donut, Auntie Anne\'s, Pepper Lunch, Ootoya, Cold Stone, Tenya, Arigato, Yoshinoya)',
    parent:'Central Group',country:'TH',since:1978,
    branches:{total:'~1,800',bkk:'~700',upcountry:'~1,100'},
    expansion:'100-150 สาขา/ปี ทั่วเครือ',format:['Kiosk','Inline','Drive-Thru'],size:'30-300 ตร.ม.',
    bd:{name:'CRG Property',email:'property@crg.co.th',phone:'02-664-5000',hq:'Central Embassy'},status:'active'},
  {id:'qsra',name:'QSR Brands (Pizza Hut TH/Taco Bell)',cat:'F&B',sub:'QSR',parent:'QSR Brands (Yum China Partner)',
    country:'TH',since:1994,branches:{total:'~180 Pizza Hut'},expansion:'10-15 สาขา/ปี',
    format:['Inline','Kiosk'],size:'80-200 ตร.ม.',bd:{email:'enquiries@pizzahut.co.th'},status:'selective'},
  {id:'oishi',name:'Oishi Group (Shabushi, Oishi Buffet, Kakashi)',cat:'F&B',sub:'Japanese Buffet',parent:'Thai Beverage (SET: THBEV)',
    country:'TH',since:1999,branches:{total:'~280',bkk:'~120',upcountry:'~160'},
    expansion:'10-15 สาขา/ปี',format:['Inline','Anchor F&B'],size:'200-500 ตร.ม.',
    bd:{name:'Oishi Property',email:'leasing@oishigroup.com',hq:'กรุงเทพฯ'},status:'active'},
  {id:'zen',name:'ZEN Group (ZEN Sushi, AKA, On The Table, Tetsu, Khiang)',cat:'F&B',sub:'Japanese + Thai chain',parent:'ZEN Corporation (SET: ZEN)',
    country:'TH',since:1991,branches:{total:'~340',bkk:'~180',upcountry:'~160'},
    expansion:'25-40 สาขา/ปี',format:['Inline','Anchor F&B','Drive-Thru'],size:'120-350 ตร.ม.',
    bd:{name:'ZEN Property',email:'property@zengroup.co.th',phone:'02-291-8889',hq:'กรุงเทพฯ'},status:'active'},
  {id:'mcdonalds',name:"McDonald's (TH)",cat:'F&B',sub:'QSR Burger',parent:'McThai (Bangkok Family)',
    country:'TH',since:1985,branches:{total:'~250',bkk:'~140',upcountry:'~110'},
    expansion:'15-20 สาขา/ปี (drive-thru เน้น)',format:['Inline','Drive-Thru','Kiosk'],size:'150-400 ตร.ม.',
    bd:{name:'McThai New Store Development',email:'leasing@mcthai.co.th',phone:'02-009-1000'},status:'active'},
  {id:'kfc',name:'KFC (TH)',cat:'F&B',sub:'QSR Fried Chicken',parent:'CRG + RD (Restaurant Development) + KFC International',
    country:'TH',since:1984,branches:{total:'~1,000+'},expansion:'40-60 สาขา/ปี',
    format:['Inline','Drive-Thru','Kiosk','Mall'],size:'100-300 ตร.ม.',
    bd:{name:'KFC RD/CRG Property',email:'property@crg.co.th'},status:'active'},
  {id:'tims',name:'Tim Hortons',cat:'F&B',sub:'Coffee+Donut Chain',parent:'Restaurant Brands International (CA) / Master Franchise TH: Berli Jucker Foods',
    country:'CA→TH',since:2024,branches:{total:'~10 (กำลังขยายไทย)'},expansion:'แผน 100+ ใน 5 ปี · เป้าหมายเมืองหลัก + กทม.',
    format:['Inline','Kiosk','Drive-Thru'],size:'80-200 ตร.ม.',
    siteCriteria:'High-traffic mall, office tower, BTS/MRT exit',
    bd:{name:'BJC Food (Berli Jucker)',email:'info@bjc.co.th',phone:'02-146-5999'},status:'active'},
  {id:'donki',name:'Don Don Donki',cat:'Mass/Convenience',sub:'Japanese Discount Lifestyle',parent:'Pan Pacific International (JP)',
    country:'JP→TH',since:2019,branches:{total:'~7 (TH)',bkk:'~6',upcountry:'~1 (Pattaya)'},
    expansion:'2-4 สาขา/ปี · แผน 30 สาขาภายใน 2030',format:['Anchor (3,000-6,000 ตร.ม.)','Flagship','Mid-format (1,500 ตร.ม.)'],
    size:'1,500-6,000 ตร.ม.',rentBudget:'฿400-900/ตร.ม./เดือน (anchor zone)',
    siteCriteria:'24-hour ready, mall A หรือ standalone กลางเมือง, ใกล้ residential ความหนาแน่นสูง',
    target:'Local + Japanese + tourist, all-age',
    bd:{name:'Pan Pacific Retail BD',email:'realestate@dondonki.com.sg',hq:'Pan Pacific Retail Asia (SG)'},status:'active',
    notes:'Site target ปัจจุบัน: Thonglor, EmSphere, Onnut, Phrom Phong, Ratchada, Pinklao + ขยายสู่เมืองหลัก'},
  {id:'daiso',name:'Daiso',cat:'Mass/Convenience',sub:'Japanese 100-Yen Variety',parent:'Daiso Industries (JP) — Master Franchise TH: Saha Group / Daiso Japan TH',
    country:'JP→TH',since:2007,branches:{total:'~140',bkk:'~80',upcountry:'~60'},
    expansion:'15-25 สาขา/ปี ทั่วประเทศ',format:['Inline 250-450 ตร.ม.','Anchor Specialty'],size:'250-700 ตร.ม.',
    rentBudget:'฿500-1,200/ตร.ม./เดือน',siteCriteria:'Mall A-C, hypermarket, community mall, ใกล้ supermarket',
    target:'Family + Gen Z, mass market, avg ฿120/คน',
    bd:{name:'Daiso Japan TH BD',email:'info@daiso.co.th',phone:'02-105-1700',hq:'กรุงเทพฯ'},status:'active'},
  // ===== Fashion / Beauty =====
  {id:'uniqlo',name:'Uniqlo',cat:'Fashion',sub:'Apparel Specialty',parent:'Fast Retailing (JP) — JV กับ Mitsubishi/Central',
    country:'JP→TH',since:2011,branches:{total:'~75',bkk:'~40',upcountry:'~35'},
    expansion:'6-10 สาขา/ปี',format:['Anchor (800-2,500 ตร.ม.)','Flagship'],size:'800-2,500 ตร.ม.',
    rentBudget:'฿500-1,200/ตร.ม./เดือน (anchor)',siteCriteria:'Mall A หรือ tier 1 lifestyle',target:'All-age, avg ฿800',
    bd:{name:'Uniqlo TH Property',email:'property.th@uniqlo.com'},status:'active'},
  {id:'zara',name:'Zara',cat:'Fashion',sub:'Fast Fashion',parent:'Inditex (ES) — Master Franchise TH: Central Group',
    country:'ES→TH',since:2006,branches:{total:'~14',bkk:'~10',upcountry:'~4'},
    expansion:'1-2 สาขา/ปี (selective)',format:['Flagship','Anchor (1,500-3,500 ตร.ม.)'],size:'1,500-3,500 ตร.ม.',
    bd:{email:'realestate@inditex.com'},status:'selective'},
  {id:'hm',name:'H&M',cat:'Fashion',sub:'Fast Fashion',parent:'H&M Group (SE)',
    country:'SE→TH',since:2011,branches:{total:'~18',bkk:'~12',upcountry:'~6'},
    expansion:'1-2 สาขา/ปี',format:['Anchor (1,200-2,500 ตร.ม.)'],size:'1,200-2,500 ตร.ม.',
    bd:{email:'expansion.th@hm.com'},status:'selective'},
  {id:'muji',name:'MUJI',cat:'Lifestyle/Specialty',sub:'Lifestyle Department',parent:'Ryohin Keikaku (JP) — Master Franchise TH: Central Group',
    country:'JP→TH',since:2006,branches:{total:'~30',bkk:'~22',upcountry:'~8'},
    expansion:'3-5 สาขา/ปี',format:['Inline','Anchor (500-1,500 ตร.ม.)'],size:'500-1,500 ตร.ม.',
    bd:{email:'realestate.muji@central.co.th'},status:'active'},
  {id:'decathlon',name:'Decathlon',cat:'Lifestyle/Specialty',sub:'Sports Retail',parent:'Decathlon (FR)',
    country:'FR→TH',since:2012,branches:{total:'~7',bkk:'~5',upcountry:'~2'},
    expansion:'1-2 สาขา/ปี (anchor)',format:['Anchor (3,000-5,000 ตร.ม.)','Standalone'],
    size:'3,000-5,000 ตร.ม.',rentBudget:'฿250-500/ตร.ม./เดือน',
    bd:{email:'thailand.expansion@decathlon.com'},status:'active'},
  {id:'sephora',name:'Sephora',cat:'Beauty/Health',sub:'Beauty Specialty',parent:'LVMH (FR) — TH: DKSH',
    country:'FR→TH',since:2013,branches:{total:'~30+',bkk:'~22',upcountry:'~8'},
    expansion:'3-5 สาขา/ปี',format:['Inline 200-500 ตร.ม.','Flagship'],size:'200-500 ตร.ม.',
    bd:{email:'sephora.th@dksh.com'},status:'active'},
  {id:'watsons',name:'Watsons',cat:'Beauty/Health',sub:'Health & Beauty Chain',parent:'AS Watson (HK) — CP Group JV',
    country:'HK→TH',since:1996,branches:{total:'~600',bkk:'~250',upcountry:'~350'},
    expansion:'30-50 สาขา/ปี',format:['Inline','Kiosk Pharmacy'],size:'100-300 ตร.ม.',
    bd:{email:'watsons.realestate@aswatson.com'},status:'active'},
  {id:'boots',name:'Boots',cat:'Beauty/Health',sub:'Health & Beauty Chain',parent:'Walgreens Boots Alliance',
    country:'UK→TH',since:1997,branches:{total:'~280',bkk:'~140',upcountry:'~140'},
    expansion:'10-20 สาขา/ปี',format:['Inline'],size:'100-250 ตร.ม.',
    bd:{email:'boots.realestate@boots.co.th'},status:'active'},
  {id:'eveandboy',name:'Eveandboy',cat:'Beauty/Health',sub:'Multi-Brand Beauty',parent:'Eveandboy Co.',
    country:'TH',since:2005,branches:{total:'~30',bkk:'~20',upcountry:'~10'},
    expansion:'3-5 สาขา/ปี',format:['Anchor 1,000-1,800 ตร.ม.','Inline'],size:'500-1,800 ตร.ม.',
    bd:{email:'corporate@eveandboy.com'},status:'active'},
  // ===== Lifestyle / Furniture / Home =====
  {id:'index',name:'Index Living Mall',cat:'Home/Furniture',sub:'Furniture Specialty',parent:'Index Living Mall PCL (SET: ILM)',
    country:'TH',since:1973,branches:{total:'~30',bkk:'~15',upcountry:'~15'},
    expansion:'2-3 สาขา/ปี',format:['Anchor 5,000-12,000 ตร.ม.','Standalone'],size:'5,000-12,000 ตร.ม.',
    bd:{email:'corporate@indexlivingmall.com',phone:'02-833-0555'},status:'active'},
  {id:'homepro',name:'HomePro',cat:'Home/Furniture',sub:'Home Improvement',parent:'Home Product Center (SET: HMPRO) — Land & Houses Group',
    country:'TH',since:1995,branches:{total:'~95',bkk:'~40',upcountry:'~55'},
    expansion:'4-6 สาขา/ปี',format:['Anchor 8,000-15,000 ตร.ม.','Standalone'],size:'8,000-15,000 ตร.ม.',
    bd:{email:'corporate@homepro.co.th',phone:'02-832-1000'},status:'active'},
  {id:'thaiwatsadu',name:'Thai Watsadu',cat:'Home/Furniture',sub:'Construction & Home',parent:'CRC Thai Watsadu (Central Group)',
    country:'TH',since:1997,branches:{total:'~80',bkk:'~25',upcountry:'~55'},
    expansion:'5-8 สาขา/ปี',format:['Anchor/Standalone 10,000-20,000 ตร.ม.'],size:'10,000-20,000 ตร.ม.',
    bd:{email:'leasing@thaiwatsadu.com'},status:'active'},
  {id:'ikea',name:'IKEA',cat:'Home/Furniture',sub:'Furniture/Home',parent:'IKANO (Master Franchise SEA)',
    country:'SE→TH',since:2011,branches:{total:'4 (Bangna, Bangyai, Sukhumvit, Phuket coming)'},
    expansion:'1 สาขา/ปี · เป้า 6-8 สาขาภายในปี 2030',format:['Anchor 30,000-50,000 ตร.ม.','City format'],
    size:'5,000-50,000 ตร.ม.',bd:{email:'realestate.thailand@ikea.com'},status:'active'},
  {id:'powerbuy',name:'Power Buy',cat:'Electronics',sub:'Electronics Specialty',parent:'CRC (Central Group)',
    country:'TH',since:1989,branches:{total:'~130'},expansion:'5-10 สาขา/ปี',
    format:['Anchor 500-2,500 ตร.ม.','Inline'],size:'500-2,500 ตร.ม.',
    bd:{email:'leasing@powerbuy.co.th'},status:'active'},
  // ===== Convenience =====
  {id:'7-11',name:'7-Eleven',cat:'Mass/Convenience',sub:'Convenience Store',parent:'CP All (SET: CPALL)',
    country:'TH',since:1989,branches:{total:'~14,000+',bkk:'~4,000',upcountry:'~10,000'},
    expansion:'700-800 สาขา/ปี',format:['Inline (street/mall)','Standalone'],size:'80-180 ตร.ม.',
    bd:{email:'leasing@cpall.co.th',phone:'02-071-2999'},status:'active'},
  {id:'lawson',name:'Lawson 108',cat:'Mass/Convenience',sub:'Convenience Store',parent:'Saha-Lawson (JV Saha + Lawson JP)',
    country:'TH',since:1996,branches:{total:'~1,200'},expansion:'50-80 สาขา/ปี',
    format:['Inline'],size:'80-150 ตร.ม.',bd:{email:'corporate@saha-lawson.co.th'},status:'active'},
  // ===== Edutainment =====
  {id:'kidzania',name:'KidZania',cat:'Edutainment',sub:'Edutainment Anchor',parent:'KidZania International',
    country:'MX→TH',since:2013,branches:{total:'1 (Siam Paragon)'},expansion:'แผน 1 สาขาภูมิภาคใหม่ภายใน 3 ปี',
    format:['Anchor 7,000-12,000 ตร.ม.'],size:'7,000-12,000 ตร.ม.',bd:{email:'realestate@kidzaniabangkok.com'},status:'selective'},
  {id:'harborland',name:'Harbor Land',cat:'Edutainment',sub:'Indoor Playground',parent:'Harbor Mall',
    country:'TH',since:2017,branches:{total:'~10',bkk:'~4',upcountry:'~6'},expansion:'2-3 สาขา/ปี',
    format:['Anchor 1,500-3,000 ตร.ม.'],size:'1,500-3,000 ตร.ม.',bd:{email:'corporate@harborland.co.th'},status:'active'},
  {id:'funarium',name:'Funarium',cat:'Edutainment',sub:'Family Activity Center',parent:'Funarium',
    country:'TH',since:2007,branches:{total:'~4'},expansion:'1-2 สาขา/ปี',format:['Anchor 800-2,000 ตร.ม.'],
    size:'800-2,000 ตร.ม.',bd:{email:'info@funarium.co.th'},status:'selective'},
  // ===== F&B (Batch 2) =====
  {id:'pepperlunch',name:'Pepper Lunch',cat:'F&B',sub:'Japanese DIY Steak',parent:'CRG (Central Restaurants Group)',
    country:'JP→TH',since:2007,branches:{total:'~50',bkk:'~30',upcountry:'~20'},expansion:'4-6 สาขา/ปี',
    format:['Inline'],size:'120-200 ตร.ม.',rentBudget:'฿1,000-1,800/ตร.ม./เดือน',
    bd:{name:'CRG Property',email:'property@crg.co.th',phone:'02-664-5000'},status:'active'},
  {id:'krispy-kreme',name:'Krispy Kreme',cat:'F&B',sub:'Donut Specialty',parent:'KK Doughnuts Thailand',
    country:'US→TH',since:2010,branches:{total:'~25'},expansion:'2-3 สาขา/ปี',
    format:['Inline','Kiosk'],size:'80-200 ตร.ม.',bd:{email:'info@krispykreme.co.th'},status:'selective'},
  {id:'subway',name:'Subway',cat:'F&B',sub:'QSR Sandwich',parent:'Subway International',
    country:'US→TH',since:2003,branches:{total:'~100'},expansion:'10-15 สาขา/ปี',
    format:['Inline','Kiosk'],size:'60-150 ตร.ม.',rentBudget:'฿800-1,800/ตร.ม./เดือน',
    bd:{email:'realestate@subway.co.th'},status:'active'},
  {id:'burger-king',name:'Burger King',cat:'F&B',sub:'QSR Burger',parent:'Minor Food',
    country:'US→TH',since:1995,branches:{total:'~120'},expansion:'8-12 สาขา/ปี',
    format:['Inline','Drive-Thru'],size:'150-300 ตร.ม.',rentBudget:'฿800-1,800/ตร.ม./เดือน',
    bd:{name:'Minor Real Estate',email:'realestate@minor.com',phone:'02-365-7500'},status:'active'},
  {id:'aw',name:'A&W',cat:'F&B',sub:'QSR Burger/Rootbeer',parent:'Global Consumer Co. / GFA Corp',
    country:'US→TH',since:1983,branches:{total:'~80'},expansion:'5-10 สาขา/ปี',
    format:['Inline','Drive-Thru','Kiosk'],size:'80-300 ตร.ม.',bd:{email:'corporate@aw.co.th'},status:'active'},
  {id:'inthanin',name:'Inthanin Coffee',cat:'F&B',sub:'Coffee Chain',parent:'Bangchak Corp (SET: BCP)',
    country:'TH',since:2006,branches:{total:'~1,000+'},expansion:'80-100 สาขา/ปี · กำลังขยายต่างประเทศ',
    format:['Kiosk','Inline','Standalone'],size:'30-200 ตร.ม.',rentBudget:'฿500-1,200/ตร.ม./เดือน · GP-share for Bangchak stations',
    siteCriteria:'ปั๊ม Bangchak, mall ทุก tier, ทำเลทั่วไป',
    bd:{name:'Bangchak Retail BD',email:'inthanin@bangchak.co.th'},status:'active',
    notes:'แบรนด์กาแฟอันดับ 2 ในไทยตามจำนวนสาขา (รองจาก Café Amazon)'},
  {id:'class-cafe',name:'Class Cafe',cat:'F&B',sub:'Lifestyle Coffee + Co-Working',parent:'Class Coffee Co. (NCR-based)',
    country:'TH',since:2014,branches:{total:'~30'},expansion:'5-8 สาขา/ปี · เน้นภูมิภาค',
    format:['Inline','Standalone'],size:'150-400 ตร.ม.',
    bd:{email:'corporate@class-cafe.com',hq:'นครราชสีมา'},status:'active'},
  {id:'arabica',name:'%Arabica',cat:'F&B',sub:'Specialty Coffee',parent:'%Arabica Japan (Master Franchise TH)',
    country:'JP→TH',since:2022,branches:{total:'~10'},expansion:'3-5 สาขา/ปี (Selective)',
    format:['Flagship','Kiosk'],size:'40-150 ตร.ม.',rentBudget:'฿1,500-3,500/ตร.ม./เดือน',
    siteCriteria:'Tourist destination, A-list mall, riverfront',
    bd:{email:'th.realestate@arabica.coffee'},status:'selective'},
  {id:'iberry',name:'iberry',cat:'F&B',sub:'Ice Cream / Dessert',parent:'Iberry Group',
    country:'TH',since:1999,branches:{total:'~30'},expansion:'3-5 สาขา/ปี',
    format:['Inline','Kiosk'],size:'60-200 ตร.ม.',bd:{email:'info@iberryhomemade.com'},status:'active'},
  {id:'yenly-yours',name:'Yenly Yours',cat:'F&B',sub:'Mango Dessert',parent:'Yenly Yours',
    country:'TH',since:2014,branches:{total:'~15'},expansion:'3-5 สาขา/ปี · เน้น mall A',
    format:['Inline','Kiosk'],size:'40-120 ตร.ม.',bd:{email:'corporate@yenlyyours.com'},status:'active'},
  {id:'bar-b-q-plaza',name:'Bar B Q Plaza',cat:'F&B',sub:'Korean BBQ',parent:'Foodpassion',
    country:'TH',since:1987,branches:{total:'~140',bkk:'~60',upcountry:'~80'},
    expansion:'10-15 สาขา/ปี',format:['Inline','Anchor F&B'],size:'250-450 ตร.ม.',
    rentBudget:'฿700-1,500/ตร.ม./เดือน',bd:{email:'corporate@barbqplaza.com'},status:'active'},
  {id:'sukishi',name:'Sukishi',cat:'F&B',sub:'Korean Charcoal BBQ',parent:'Sukishi Group',
    country:'TH',since:2005,branches:{total:'~60'},expansion:'5-8 สาขา/ปี',
    format:['Inline','Anchor F&B'],size:'200-400 ตร.ม.',bd:{email:'corporate@sukishi.com'},status:'active'},
  {id:'mo-mo-paradise',name:'Mo-Mo-Paradise',cat:'F&B',sub:'Japanese Sukiyaki/Shabu',parent:'NOBLE Asia Lifestyle Holdings',
    country:'JP→TH',since:2007,branches:{total:'~35'},expansion:'3-5 สาขา/ปี',
    format:['Inline','Anchor F&B'],size:'200-400 ตร.ม.',bd:{email:'corporate@momoparadise.co.th'},status:'active'},
  {id:'shabushi',name:'Shabushi',cat:'F&B',sub:'Conveyor Shabu Buffet',parent:'Oishi Group (Thai Beverage)',
    country:'TH',since:2003,branches:{total:'~150'},expansion:'10-15 สาขา/ปี',
    format:['Inline','Anchor F&B'],size:'200-400 ตร.ม.',bd:{email:'leasing@oishigroup.com'},status:'active'},
  {id:'tonkatsu-maisen',name:'Tonkatsu Maisen',cat:'F&B',sub:'Japanese Tonkatsu',parent:'Maisen Thailand',
    country:'JP→TH',since:2008,branches:{total:'~15'},expansion:'2-3 สาขา/ปี',
    format:['Inline'],size:'150-250 ตร.ม.',bd:{email:'info@maisen-thailand.com'},status:'selective'},
  {id:'auntie-annes',name:"Auntie Anne's",cat:'F&B',sub:'Pretzel Kiosk',parent:'CRG',
    country:'US→TH',since:1996,branches:{total:'~190'},expansion:'10-15 สาขา/ปี',
    format:['Kiosk'],size:'8-30 ตร.ม.',rentBudget:'฿2,500-5,000/ตร.ม./เดือน',bd:{email:'property@crg.co.th'},status:'active'},
  {id:'mister-donut',name:'Mister Donut',cat:'F&B',sub:'Donut Chain',parent:'CRG',
    country:'JP→TH',since:1978,branches:{total:'~325'},expansion:'15-20 สาขา/ปี',
    format:['Kiosk','Inline'],size:'30-120 ตร.ม.',bd:{email:'property@crg.co.th'},status:'active'},
  {id:'dunkin',name:"Dunkin'",cat:'F&B',sub:'Donut/Coffee Chain',parent:"Mudman PCL (Domino's/Dunkin TH)",
    country:'US→TH',since:1981,branches:{total:'~260'},expansion:'10-15 สาขา/ปี',
    format:['Kiosk','Inline'],size:'30-150 ตร.ม.',bd:{email:'corporate@mudmangroup.com'},status:'active'},
  {id:'yoshinoya',name:'Yoshinoya',cat:'F&B',sub:'Japanese Beef Bowl',parent:'CRG',
    country:'JP→TH',since:2014,branches:{total:'~10'},expansion:'2-3 สาขา/ปี',
    format:['Inline'],size:'80-180 ตร.ม.',bd:{email:'property@crg.co.th'},status:'selective'},
  {id:'coco-ichibanya',name:'Coco Ichibanya',cat:'F&B',sub:'Japanese Curry',parent:'Ichibanya (JP) — Master Franchise',
    country:'JP→TH',since:2008,branches:{total:'~40'},expansion:'3-5 สาขา/ปี',
    format:['Inline'],size:'80-200 ตร.ม.',bd:{email:'th.realestate@ichibanya.co.jp'},status:'active'},
  // ===== Fashion / Footwear =====
  {id:'charles-keith',name:'Charles & Keith',cat:'Fashion',sub:'Footwear / Accessory',parent:'Charles & Keith Group (SG)',
    country:'SG→TH',since:2002,branches:{total:'~30'},expansion:'3-5 สาขา/ปี',
    format:['Inline'],size:'80-200 ตร.ม.',rentBudget:'฿1,000-2,500/ตร.ม./เดือน',
    bd:{email:'sea.realestate@charleskeith.com'},status:'active'},
  {id:'pomelo',name:'Pomelo Fashion',cat:'Fashion',sub:'Fast Fashion (TH-born)',parent:'Pomelo Fashion (TH)',
    country:'TH',since:2013,branches:{total:'~30 Tap-Try hubs'},expansion:'5-10 สาขา/ปี · เน้น mall A-B + ในเขต BTS/MRT',
    format:['Inline','Tap-Try Pickup'],size:'100-250 ตร.ม.',bd:{email:'realestate@pomelofashion.com'},status:'active'},
  {id:'mango',name:'Mango',cat:'Fashion',sub:'Fashion',parent:'Mango (ES)',
    country:'ES→TH',since:1999,branches:{total:'~25'},expansion:'1-2 สาขา/ปี',
    format:['Anchor (400-800 ตร.ม.)'],size:'400-800 ตร.ม.',bd:{email:'expansion.th@mango.com'},status:'selective'},
  {id:'levis',name:"Levi's",cat:'Fashion',sub:'Apparel / Denim',parent:'Levi Strauss & Co.',
    country:'US→TH',since:1971,branches:{total:'~50'},expansion:'3-5 สาขา/ปี',
    format:['Inline','Flagship'],size:'80-300 ตร.ม.',bd:{email:'leasing.th@levi.com'},status:'active'},
  {id:'cos',name:'COS',cat:'Fashion',sub:'Premium Fashion',parent:'H&M Group (SE)',
    country:'SE→TH',since:2018,branches:{total:'~5'},expansion:'1 สาขา/ปี (selective)',
    format:['Anchor (300-600 ตร.ม.)'],size:'300-600 ตร.ม.',bd:{email:'expansion.th@hm.com'},status:'selective'},
  {id:'pull-bear',name:'Pull & Bear',cat:'Fashion',sub:'Fast Fashion',parent:'Inditex (ES) / Central',
    country:'ES→TH',since:2018,branches:{total:'~8'},expansion:'1-2 สาขา/ปี',
    format:['Anchor (600-1,200 ตร.ม.)'],size:'600-1,200 ตร.ม.',bd:{email:'realestate@inditex.com'},status:'selective'},
  {id:'stradivarius',name:'Stradivarius',cat:'Fashion',sub:'Fast Fashion (Women)',parent:'Inditex / Central',
    country:'ES→TH',since:2018,branches:{total:'~7'},expansion:'1-2 สาขา/ปี',
    format:['Inline'],size:'500-1,000 ตร.ม.',bd:{email:'realestate@inditex.com'},status:'selective'},
  {id:'massimo-dutti',name:'Massimo Dutti',cat:'Fashion',sub:'Premium Fashion',parent:'Inditex / Central',
    country:'ES→TH',since:2017,branches:{total:'~5'},expansion:'1 สาขา/ปี',
    format:['Anchor (400-800 ตร.ม.)'],size:'400-800 ตร.ม.',bd:{email:'realestate@inditex.com'},status:'selective'},
  {id:'crocs',name:'Crocs',cat:'Fashion',sub:'Footwear',parent:'Crocs Inc. (US)',
    country:'US→TH',since:2007,branches:{total:'~50'},expansion:'5-8 สาขา/ปี',
    format:['Inline','Kiosk'],size:'40-150 ตร.ม.',bd:{email:'sea.realestate@crocs.com'},status:'active'},
  {id:'skechers',name:'Skechers',cat:'Fashion',sub:'Sports Footwear',parent:'Skechers (US)',
    country:'US→TH',since:2010,branches:{total:'~80'},expansion:'8-12 สาขา/ปี',
    format:['Inline'],size:'100-250 ตร.ม.',bd:{email:'sea.realestate@skechers.com'},status:'active'},
  {id:'adidas',name:'adidas',cat:'Fashion',sub:'Sports Apparel/Footwear',parent:'adidas AG (DE)',
    country:'DE→TH',since:1989,branches:{total:'~100+'},expansion:'10-15 สาขา/ปี',
    format:['Inline','Flagship'],size:'150-500 ตร.ม.',bd:{email:'realestate.thailand@adidas.com'},status:'active'},
  {id:'nike',name:'Nike',cat:'Fashion',sub:'Sports Apparel/Footwear',parent:'Nike Inc. (US)',
    country:'US→TH',since:1985,branches:{total:'~100+'},expansion:'10-15 สาขา/ปี',
    format:['Inline','Flagship','Factory Store'],size:'150-600 ตร.ม.',bd:{email:'th.realestate@nike.com'},status:'active'},
  {id:'onitsuka',name:'Onitsuka Tiger',cat:'Fashion',sub:'Heritage Footwear',parent:'ASICS (JP)',
    country:'JP→TH',since:2010,branches:{total:'~25'},expansion:'2-4 สาขา/ปี',
    format:['Inline'],size:'80-200 ตร.ม.',bd:{email:'th.realestate@asics.com'},status:'active'},
  // ===== Beauty =====
  {id:'mac',name:'M·A·C Cosmetics',cat:'Beauty/Health',sub:'Pro Makeup',parent:'Estée Lauder Companies',
    country:'US→TH',since:1996,branches:{total:'~30'},expansion:'2-3 สาขา/ปี',
    format:['Inline','Counter'],size:'30-120 ตร.ม.',bd:{email:'th.realestate@elcompanies.com'},status:'active'},
  {id:'innisfree',name:'innisfree',cat:'Beauty/Health',sub:'K-Beauty',parent:'Amorepacific (KR)',
    country:'KR→TH',since:2017,branches:{total:'~25'},expansion:'3-5 สาขา/ปี',
    format:['Inline'],size:'80-200 ตร.ม.',bd:{email:'th.realestate@amorepacific.com'},status:'active'},
  {id:'laneige',name:'Laneige',cat:'Beauty/Health',sub:'K-Beauty Skincare',parent:'Amorepacific (KR)',
    country:'KR→TH',since:2010,branches:{total:'~40 counters'},expansion:'3-5 สาขา/ปี',
    format:['Counter','Inline'],size:'30-100 ตร.ม.',bd:{email:'th.realestate@amorepacific.com'},status:'active'},
  {id:'body-shop',name:'The Body Shop',cat:'Beauty/Health',sub:'Natural Beauty',parent:'Natura&Co (BR)',
    country:'UK→TH',since:1992,branches:{total:'~40'},expansion:'2-4 สาขา/ปี',
    format:['Inline'],size:'50-150 ตร.ม.',bd:{email:'th.realestate@thebodyshop.com'},status:'active'},
  {id:'bath-body-works',name:'Bath & Body Works',cat:'Beauty/Health',sub:'Bath & Body',parent:'L Brands (US) Master Franchise',
    country:'US→TH',since:2018,branches:{total:'~15'},expansion:'2-3 สาขา/ปี',
    format:['Inline'],size:'150-300 ตร.ม.',bd:{email:'th.expansion@bathandbodyworks.com'},status:'active'},
  // ===== Electronics =====
  {id:'istudio',name:'iStudio',cat:'Electronics',sub:'Apple Premium Reseller',parent:'SPVi PCL (SET: SPVI)',
    country:'TH',since:2008,branches:{total:'~80'},expansion:'5-10 สาขา/ปี',
    format:['Inline','Flagship'],size:'100-400 ตร.ม.',rentBudget:'฿1,000-2,500/ตร.ม./เดือน',
    bd:{name:'SPVi Property',email:'corporate@spvi.co.th'},status:'active'},
  {id:'studio7',name:'Studio7',cat:'Electronics',sub:'Apple Premium Reseller',parent:'Comseven (SET: COM7)',
    country:'TH',since:2013,branches:{total:'~100'},expansion:'5-10 สาขา/ปี',
    format:['Inline'],size:'100-400 ตร.ม.',bd:{email:'corporate@com7.co.th'},status:'active'},
  {id:'banana-it',name:'BaNANA',cat:'Electronics',sub:'IT/Electronics Specialty',parent:'Comseven (SET: COM7)',
    country:'TH',since:2008,branches:{total:'~200+'},expansion:'15-20 สาขา/ปี',
    format:['Inline','Kiosk'],size:'80-300 ตร.ม.',bd:{email:'corporate@com7.co.th'},status:'active'},
  {id:'jib',name:'JIB Computer',cat:'Electronics',sub:'PC/Gaming Specialty',parent:'JIB Computer Group',
    country:'TH',since:1998,branches:{total:'~25'},expansion:'2-3 สาขา/ปี',
    format:['Anchor (300-1,000 ตร.ม.)'],size:'200-1,000 ตร.ม.',bd:{email:'corporate@jib.co.th'},status:'active'},
  {id:'powermall',name:'Power Mall',cat:'Electronics',sub:'Electronics Department',parent:'The Mall Group',
    country:'TH',since:1994,branches:{total:'~7'},expansion:'ตาม The Mall',
    format:['Anchor (1,500-3,000 ตร.ม.)'],size:'1,500-3,000 ตร.ม.',bd:{email:'leasing@themall.co.th'},status:'selective'},
  // ===== Home / Furniture (additional) =====
  {id:'sb-furniture',name:'SB Design Square',cat:'Home/Furniture',sub:'Furniture Retail',parent:'SB Furniture',
    country:'TH',since:1966,branches:{total:'~50'},expansion:'3-5 สาขา/ปี',
    format:['Anchor (3,000-8,000 ตร.ม.)','Inline'],size:'2,000-8,000 ตร.ม.',
    bd:{email:'corporate@sb-furniture.com'},status:'active'},
  {id:'modernform',name:'Modernform',cat:'Home/Furniture',sub:'Office/Home Furniture',parent:'Modernform Group',
    country:'TH',since:1980,branches:{total:'~30'},expansion:'2-4 สาขา/ปี',
    format:['Anchor 1,500-4,000 ตร.ม.'],size:'1,500-4,000 ตร.ม.',bd:{email:'corporate@modernform.co.th'},status:'active'},
  {id:'koncept',name:'Koncept Furniture',cat:'Home/Furniture',sub:'Furniture Retail',parent:'Koncept',
    country:'TH',since:2008,branches:{total:'~10'},expansion:'1-2 สาขา/ปี',
    format:['Anchor 1,000-3,000 ตร.ม.'],size:'1,000-3,000 ตร.ม.',bd:{email:'info@koncept-furniture.com'},status:'selective'},
  // ===== Books / Stationery =====
  {id:'b2s',name:'B2S',cat:'Lifestyle/Specialty',sub:'Books & Stationery',parent:'Central Group',
    country:'TH',since:1995,branches:{total:'~100'},expansion:'5-10 สาขา/ปี',
    format:['Inline','Anchor (200-800 ตร.ม.)'],size:'200-800 ตร.ม.',bd:{email:'leasing@b2s.co.th'},status:'active'},
  {id:'se-ed',name:'SE-ED Bookstore',cat:'Lifestyle/Specialty',sub:'Books',parent:'SE-EDUCATION (SET: SE-ED)',
    country:'TH',since:1974,branches:{total:'~400'},expansion:'10-20 สาขา/ปี',
    format:['Inline','Kiosk'],size:'80-300 ตร.ม.',bd:{email:'leasing@se-ed.com'},status:'active'},
  {id:'asia-books',name:'Asia Books',cat:'Lifestyle/Specialty',sub:'English Books',parent:'Asia Books',
    country:'TH',since:1969,branches:{total:'~25'},expansion:'2-3 สาขา/ปี',
    format:['Inline'],size:'150-400 ตร.ม.',bd:{email:'corporate@asiabooks.com'},status:'selective'},
  {id:'kinokuniya',name:'Kinokuniya',cat:'Lifestyle/Specialty',sub:'International Books',parent:'Kinokuniya (JP)',
    country:'JP→TH',since:1980,branches:{total:'~5'},expansion:'Selective expansion',
    format:['Anchor (500-1,500 ตร.ม.)'],size:'500-1,500 ตร.ม.',bd:{email:'th.realestate@kinokuniya.co.jp'},status:'selective'},
  // ===== Edutainment =====
  {id:'bounce',name:'BOUNCE Trampoline',cat:'Edutainment',sub:'Trampoline Park',parent:'BOUNCE',
    country:'AU→TH',since:2016,branches:{total:'~5'},expansion:'1-2 สาขา/ปี',
    format:['Anchor (1,500-3,000 ตร.ม.)'],size:'1,500-3,000 ตร.ม.',bd:{email:'corporate@bounce.in.th'},status:'active'},
];

/* =========================================================
   DATA · PROPERTIES (Retail spaces — listings)
   ========================================================= */
const PROPERTIES = [
  {id:'p001',title:'พื้นที่ค้าปลีกพรีเมียม สยามสแควร์วัน',mall:'Siam Square One',landlord:'CU Property (จุฬาฯ)',
    type:'mall',region:'bkk',district:'ปทุมวัน',lat:13.7448,lng:100.5343,size:120,
    rent:350000,service:30000,cam:18000,deposit:'6 เดือน',escalation:'5% ต่อปี',
    leaseTerm:'3+3 (ต่อสัญญาได้)',handoverDate:'1 ส.ค. 2026',fitout:'45 วัน',handoverCond:'Bareshell',
    currentTenant:'ผู้เช่าเดิมยังไม่รื้อ — ตอบกลับรับพื้นที่ As-is ภายใน 30 มิ.ย. 2026',
    renovationPlan:'มีแผน partial refresh F1-F2 ปี 2027 (3-4 เดือน, ไม่กระทบยูนิตชั้น G)',
    status:'available',match:95,image:'',
    extras:{stores:'~200 ร้าน',occupancy:'92%',gla:'~28,000 ตร.ม.',traffic:'~25,000/วัน (ทำงาน), ~45,000/วัน (สุดสัปดาห์)',
      parking:'500 รถยนต์ / 200 มอเตอร์ไซด์ (Siam Square cluster)',anchor:'Loft, Boots, Daiso',
      supermarket:'Tops Daily (ใกล้ Siam Center)',mix:'F&B 35% · Fashion 30% · Beauty 15% · Lifestyle 20%',
      demographic:'Gen Z 50% · Millennial 30% · Tourist 15%',transport:'BTS Siam 75% · รถยนต์ 15% · อื่นๆ 10%'},
    contact:'leasing@chulapropertymgmt.co.th · 02-218-3801'},
  {id:'p002',title:'ยูนิตศูนย์การค้าสีลมคอมเพล็กซ์',mall:'Silom Complex',landlord:'CPN',type:'mall',region:'bkk',district:'บางรัก',
    lat:13.7282,lng:100.5343,size:85,rent:180000,service:18000,cam:12000,deposit:'6 เดือน',escalation:'5% ต่อปี',
    leaseTerm:'3+3',handoverDate:'15 ก.ย. 2026',fitout:'60 วัน',handoverCond:'Bareshell',
    currentTenant:'ว่าง — พร้อมส่งมอบ',renovationPlan:'รีโนเวทใหญ่เสร็จปี 2022 ไม่มีแผน 3-6 ปีข้างหน้า',
    status:'available',match:88,
    extras:{stores:'~150 ร้าน',occupancy:'90%',gla:'~38,000 ตร.ม.',traffic:'~30,000/วัน (office workers)',
      parking:'600 รถยนต์ / 250 มอเตอร์ไซด์',anchor:'Robinson, Tops, Major Cineplex',
      supermarket:'Tops Market',mix:'F&B 30% · Fashion 25% · Beauty 15% · Lifestyle 30%',
      demographic:'Office worker 60% · BKK resident 30% · Tourist 10%',transport:'BTS Sala Daeng 60% · MRT Silom 20%'},
    contact:'leasing@cpn.co.th · 02-021-9999'},
  {id:'p003',title:'พื้นที่บูติก ชั้น G เอ็มควอเทียร์',mall:'EmQuartier',landlord:'The Mall Group',type:'mall',region:'bkk',district:'คลองเตย',
    lat:13.7305,lng:100.5697,size:200,rent:500000,service:50000,cam:25000,deposit:'9 เดือน',escalation:'5% ต่อปี',
    leaseTerm:'3+3',handoverDate:'1 ต.ค. 2026',fitout:'75 วัน',handoverCond:'Bareshell',
    currentTenant:'มีผู้เช่า — ต้องตอบกลับรับ As-is ภายใน 15 ส.ค. 2026',
    renovationPlan:'ไม่มีแผนรีโนเวท (มีแผนเชื่อม Em District กับ EmSphere ผ่าน sky bridge 2027)',
    status:'available',match:92,
    extras:{stores:'~600 ร้าน (Em District รวม)',occupancy:'95%',gla:'~250,000 ตร.ม. (EmQuartier เดี่ยว)',
      traffic:'~80,000/วัน',parking:'3,000 รถยนต์ / 800 มอเตอร์ไซด์ (Em District)',
      anchor:'Gourmet Market, MUJI, Tokyu Hands',supermarket:'Gourmet Market',
      mix:'Fashion 35% · F&B 30% · Beauty 15% · Lifestyle 20%',
      demographic:'Affluent 35-55 50% · Expat 20% · Tourist 20%',transport:'BTS Phrom Phong 70% · รถยนต์ 25%'},
    contact:'leasing@themall.co.th · 02-310-1000'},
  {id:'p004',title:'ล็อคฟู้ดคอร์ท เทอร์มินอล 21 อโศก',mall:'Terminal 21 Asok',landlord:'LH Mall (Terminal 21)',
    type:'mall',region:'bkk',district:'วัฒนา',lat:13.7374,lng:100.5604,size:20,rent:45000,service:5000,cam:3000,
    deposit:'3 เดือน',escalation:'5% ต่อปี',leaseTerm:'2+1 (food court terms)',handoverDate:'15 มิ.ย. 2026',fitout:'14 วัน',
    handoverCond:'As-is (พื้นที่ counter พร้อมระบบ)',currentTenant:'ว่าง',renovationPlan:'ไม่มี',
    status:'available',match:97,
    extras:{stores:'~600 ร้าน',occupancy:'93%',gla:'~60,000 ตร.ม.',traffic:'~80,000/วัน',
      parking:'1,000 รถยนต์ / 300 มอเตอร์ไซด์',anchor:'Major Cineplex, Robinson Lifestyle',
      supermarket:'Gourmet Market',mix:'F&B 30% · Fashion 40% · Beauty 15% · Lifestyle 15%',
      demographic:'Tourist 45% · Office worker 30% · Resident 25%',
      transport:'BTS Asok 50% · MRT Sukhumvit 30% · รถยนต์ 15%'},
    contact:'info@terminal21.co.th · 02-108-0888'},
  {id:'p006',title:'ร้านค้ามุมถนนทองหล่อ พร้อมที่นั่งกลางแจ้ง',mall:'-',landlord:'เจ้าของส่วนบุคคล',
    type:'standalone',region:'bkk',district:'วัฒนา',lat:13.7376,lng:100.5784,size:180,rent:220000,service:0,cam:5000,
    deposit:'6 เดือน',escalation:'7% ต่อปี',leaseTerm:'3+3+3',handoverDate:'1 ก.ค. 2026',fitout:'90 วัน',
    handoverCond:'As-is (เคยเป็นร้านอาหาร — ครัวยังอยู่)',currentTenant:'ว่าง',renovationPlan:'-',
    status:'available',match:85,
    extras:{traffic:'~12,000 vehicle/วัน (ถนนทองหล่อ)',anchor:'Donki Thonglor 200 ม., The Commons 300 ม.'},
    contact:'(ตัวอย่างนายหน้า) ติดต่อ RSL พร้อมยืนยัน'},
  {id:'p019',title:'พื้นที่แองเคอร์เทแนนท์ เมกาบางนา',mall:'Mega Bangna',landlord:'SF + IKANO',type:'mall',region:'bkk',district:'บางพลี',
    lat:13.6483,lng:100.6831,size:500,rent:450000,service:50000,cam:30000,deposit:'6 เดือน',escalation:'5% ต่อปี',
    leaseTerm:'3+3+3 (anchor terms)',handoverDate:'1 พ.ย. 2026',fitout:'120 วัน',handoverCond:'Bareshell',
    currentTenant:'ผู้เช่าเดิมยังไม่รื้อ — ตอบกลับ As-is ภายใน 31 ส.ค. 2026',
    renovationPlan:'Phase 2 ขยายปี 2026-2028 (ฝั่งใต้) — ไม่กระทบ unit เดิม',
    status:'available',match:86,
    extras:{stores:'~800 ร้าน',occupancy:'97%',gla:'~400,000 ตร.ม.',traffic:'~150,000/วัน (สุดสัปดาห์)',
      parking:'12,000 รถยนต์ / 2,000 มอเตอร์ไซด์',anchor:'IKEA, Big C Extra, Major Cineplex, HomePro, Robinson Lifestyle, Don Don Donki (เปิด 2024)',
      supermarket:'Big C Extra, Gourmet Market',mix:'F&B 25% · Fashion 25% · Specialty/Home 30% · Lifestyle 20%',
      demographic:'Family Eastern BKK 45% · Office Bangna 25% · Tourist 15%',
      transport:'รถยนต์ 80% · Shuttle BTS Udom Suk 15%'},
    contact:'leasing@mega-bangna.com · 02-105-1000'},
  {id:'p022',title:'พื้นที่คีออส เซ็นทรัลเวิลด์',mall:'CentralWorld',landlord:'CPN',type:'kiosk',region:'bkk',district:'ปทุมวัน',
    lat:13.7466,lng:100.5394,size:15,rent:80000,service:10000,cam:5000,deposit:'6 เดือน',escalation:'5% ต่อปี',
    leaseTerm:'1+1',handoverDate:'15 พ.ย. 2026',fitout:'21 วัน',handoverCond:'Bareshell (kiosk shell)',
    currentTenant:'มีผู้เช่าเดิม pop-up — ตอบกลับ As-is ภายใน 30 ก.ย. 2026',
    renovationPlan:'Atrium refresh 2027 (2 เดือน, ไม่กระทบ kiosk)',
    status:'coming-soon',match:96,
    extras:{stores:'~500 ร้าน',occupancy:'95%',gla:'~830,000 ตร.ม. (Ratchaprasong rooftop เพิ่ม)',traffic:'~150,000/วัน',
      parking:'7,000 รถยนต์',anchor:'Isetan, Zen, Tops, Major Cineplex, B2S, Power Buy',
      supermarket:'Tops Food Hall, Gourmet Market (Paragon ใกล้)',
      mix:'Fashion 35% · F&B 25% · Beauty 15% · Lifestyle 25%',
      demographic:'Tourist 45% · BKK office/resident 45% · Expat 10%',
      transport:'BTS Chit Lom/Siam 60% · รถยนต์ 30% · MRT Phloen Chit 5%'},
    contact:'leasing@cpn.co.th · 02-021-9999'},
  {id:'p013',title:'ร้านค้าย่านนักท่องเที่ยว ถนนข้าวสาร',mall:'-',landlord:'เจ้าของส่วนบุคคล',type:'standalone',region:'bkk',district:'พระนคร',
    lat:13.7589,lng:100.4977,size:30,rent:45000,service:0,cam:2000,deposit:'6 เดือน',escalation:'5%',
    leaseTerm:'3+3',handoverDate:'1 ก.ค. 2026',fitout:'30 วัน',handoverCond:'As-is',
    currentTenant:'ว่าง',renovationPlan:'-',status:'available',match:90,
    extras:{traffic:'~30,000 คน/วัน (ถนนข้าวสาร high season)'},
    contact:'(ตัวอย่างนายหน้า) — ยืนยันก่อนใช้'},
  {id:'p014',title:'ล็อคตลาดนัดรัชดา',mall:'JJ Green/ตลาดนัดรัชดา',landlord:'เจ้าของตลาด',type:'kiosk',region:'bkk',district:'ห้วยขวาง',
    lat:13.7691,lng:100.5651,size:12,rent:15000,service:1500,cam:0,deposit:'2 เดือน',escalation:'5%',
    leaseTerm:'1+1',handoverDate:'1 มิ.ย. 2026',fitout:'7 วัน',handoverCond:'As-is',
    currentTenant:'ว่าง',renovationPlan:'-',status:'available',match:88,
    extras:{traffic:'~15,000 คน/คืน (เย็น-ดึก)'},contact:'(ตัวอย่าง) ติดต่อนายหน้าตลาดนัด'},
  {id:'p015',title:'พื้นที่บาร์และร้านอาหาร สุขุมวิท ซอย 11',mall:'-',landlord:'เจ้าของส่วนบุคคล',type:'standalone',region:'bkk',district:'คลองเตย',
    lat:13.7415,lng:100.5572,size:250,rent:200000,service:0,cam:0,deposit:'12 เดือน',escalation:'7%',
    leaseTerm:'3+3+3',handoverDate:'15 ส.ค. 2026',fitout:'120 วัน',handoverCond:'As-is (เคยเป็นบาร์)',
    currentTenant:'มีผู้เช่าเดิม — รับ As-is ภายใน 30 มิ.ย. 2026',renovationPlan:'-',status:'available',match:87,
    extras:{traffic:'~25,000 คน/คืน (Soi 11 nightlife)'},contact:'(ตัวอย่างนายหน้า) — ยืนยัน'},
  {id:'p030',title:'พื้นที่ Anchor Phase 2 เซ็นทรัล เวสต์เกต',mall:'Central Westgate',landlord:'CPN',type:'mall',region:'bkk',district:'บางใหญ่ (นนทบุรี)',
    lat:13.8762,lng:100.4123,size:1200,rent:380000,service:80000,cam:50000,deposit:'9 เดือน',escalation:'5% ต่อปี',
    leaseTerm:'3+3+3',handoverDate:'1 ม.ค. 2027',fitout:'90 วัน',handoverCond:'Bareshell',
    currentTenant:'ว่าง',renovationPlan:'Phase 2 ฝั่งใต้ขยาย retail 30,000 ตร.ม. (2027-2028)',
    status:'coming-soon',match:88,
    extras:{stores:'~300 ร้าน',occupancy:'94%',gla:'~150,000 ตร.ม.',traffic:'~80,000/วัน',
      parking:'4,000 รถยนต์',anchor:'Big C Extra, Robinson, Major Cineplex, SF Cinema',
      supermarket:'Tops Food Hall',mix:'F&B 25% · Fashion 25% · Specialty 30% · Lifestyle 20%',
      demographic:'Family West BKK 60% · Tourist 5%',transport:'MRT Khlong Bang Phai 15% · รถยนต์ 75%'},
    contact:'leasing@cpn.co.th'},
  {id:'p040',title:'ยูนิต ICONSIAM ชั้น G',mall:'ICONSIAM',landlord:'Siam Piwat',type:'mall',region:'bkk',district:'คลองสาน',
    lat:13.7261,lng:100.5106,size:80,rent:420000,service:42000,cam:25000,deposit:'9 เดือน',escalation:'5%',
    leaseTerm:'3+3',handoverDate:'1 ธ.ค. 2026',fitout:'60 วัน',handoverCond:'Bareshell',
    currentTenant:'มีผู้เช่าเดิม — รับ As-is ภายใน 31 ต.ค. 2026',renovationPlan:'ไม่มี',
    status:'coming-soon',match:91,
    extras:{stores:'~500 ร้าน',occupancy:'95%',gla:'~750,000 ตร.ม.',traffic:'~100,000/วัน',
      parking:'5,000 รถยนต์',anchor:'Apple Store, Sookjai, Takashimaya, ICONLUXE, ICON Craft',
      supermarket:'Sook Siam (food hall)',mix:'Luxury 30% · Fashion 25% · F&B 25% · Lifestyle 20%',
      demographic:'Affluent + Tourist 50% · Resident 30% · Expat 20%',
      transport:'MRT Charoen Nakhon 25% · ICONSIAM ferry 20% · รถยนต์ 50%'},
    contact:'corporateaffairs@siampiwat.com · 02-658-1000'},
  {id:'p050',title:'ที่ดินเปล่า ใกล้ MRT บางใหญ่',mall:'-',landlord:'เจ้าของรายเดียว',type:'land',region:'bkk',district:'บางใหญ่ (นนทบุรี)',
    lat:13.8589,lng:100.4232,size:19200,rent:0,service:0,cam:0,deposit:'-',escalation:'-',
    leaseTerm:'เช่า 30 ปี / ขาย',handoverDate:'ตามตกลง',fitout:'-',handoverCond:'As-is (ถนนตัดผ่าน)',
    currentTenant:'-',renovationPlan:'-',status:'available',match:75,
    extras:{area:'12 ไร่',price:'ราคาตลาด ~฿15-18M/ไร่ (ซื้อ) หรือเช่า 30 ปี'},
    contact:'(ตัวอย่างนายหน้า) — RSL จะเชื่อมให้'},
  {id:'p051',title:'ที่ดิน Khao Yai (เขาใหญ่) ใกล้ Toscana',mall:'-',landlord:'ส่วนบุคคล',type:'land',region:'central',district:'ปากช่อง',
    lat:14.6486,lng:101.4196,size:24000,rent:0,service:0,cam:0,deposit:'-',escalation:'-',
    leaseTerm:'ขาย / เช่า 30 ปี',handoverDate:'ตามตกลง',fitout:'-',handoverCond:'As-is',
    currentTenant:'-',renovationPlan:'-',status:'available',match:78,
    extras:{area:'15 ไร่',price:'~฿8M/ไร่',use:'Resort retail, lifestyle outlet'},
    contact:'(ตัวอย่าง template)'},
  {id:'p060',title:'ยูนิต Central Festival Phuket Floresta',mall:'Central Phuket Floresta',landlord:'CPN',type:'mall',region:'south',district:'เมืองภูเก็ต',
    lat:7.8929,lng:98.3793,size:150,rent:240000,service:25000,cam:15000,deposit:'6 เดือน',escalation:'5%',
    leaseTerm:'3+3',handoverDate:'15 ก.ย. 2026',fitout:'60 วัน',handoverCond:'Bareshell',
    currentTenant:'ว่าง',renovationPlan:'ไม่มี (Floresta เปิด 2018 ยังใหม่)',status:'available',match:84,
    extras:{stores:'~250 ร้าน',occupancy:'90%',gla:'~80,000 ตร.ม.',traffic:'~60,000/วัน (high season)',
      parking:'2,500 รถยนต์',anchor:'Tops Food Hall, Aquaria, Major Cineplex',
      supermarket:'Tops Food Hall',mix:'F&B 25% · Fashion 30% · Lifestyle 25% · Luxury 20%',
      demographic:'Tourist 60% · Phuket resident 30% · Expat 10%',transport:'รถยนต์ 85% · Shuttle 15%'},
    contact:'leasing@cpn.co.th'},
  {id:'p070',title:'ยูนิต Central Chiangmai Festival',mall:'CentralFestival Chiangmai',landlord:'CPN',type:'mall',region:'north',district:'เมืองเชียงใหม่',
    lat:18.8044,lng:99.0288,size:100,rent:135000,service:15000,cam:8000,deposit:'6 เดือน',escalation:'5%',
    leaseTerm:'3+3',handoverDate:'1 ส.ค. 2026',fitout:'45 วัน',handoverCond:'Bareshell',
    currentTenant:'ว่าง',renovationPlan:'มีแผนรีเฟรช F2 ปี 2027',status:'available',match:82,
    extras:{stores:'~250 ร้าน',occupancy:'89%',gla:'~95,000 ตร.ม.',traffic:'~50,000/วัน',
      parking:'3,000 รถยนต์',anchor:'Tops Food Hall, Robinson, SF Cinema',
      supermarket:'Tops Food Hall',mix:'F&B 28% · Fashion 28% · Lifestyle 24% · Specialty 20%',
      demographic:'Family ChiangMai 60% · Tourist 30% · Expat 10%',
      transport:'รถยนต์ 80% · มอเตอร์ไซด์ 15% · Shuttle 5%'},
    contact:'leasing@cpn.co.th'},
  {id:'p080',title:'ยูนิต Central Korat',mall:'Central Korat',landlord:'CPN',type:'mall',region:'northeast',district:'เมืองนครราชสีมา',
    lat:14.9799,lng:102.0978,size:90,rent:95000,service:10000,cam:6000,deposit:'6 เดือน',escalation:'5%',
    leaseTerm:'3+3',handoverDate:'1 ก.ค. 2026',fitout:'45 วัน',handoverCond:'Bareshell',
    currentTenant:'ว่าง',renovationPlan:'ไม่มี',status:'available',match:80,
    extras:{stores:'~220 ร้าน',occupancy:'88%',gla:'~75,000 ตร.ม.',traffic:'~45,000/วัน',
      parking:'2,500 รถยนต์',anchor:'Tops, Robinson, SF Cinema',
      supermarket:'Tops',mix:'F&B 28% · Fashion 25% · Specialty 25% · Lifestyle 22%',
      demographic:'Family Korat 75% · Tourist 15%',transport:'รถยนต์ 85%'},contact:'leasing@cpn.co.th'},
  {id:'p090',title:'ยูนิต Central Hatyai',mall:'CentralFestival Hatyai',landlord:'CPN',type:'mall',region:'south',district:'หาดใหญ่',
    lat:7.0086,lng:100.4747,size:80,rent:88000,service:9000,cam:5000,deposit:'6 เดือน',escalation:'5%',
    leaseTerm:'3+3',handoverDate:'1 ก.ย. 2026',fitout:'45 วัน',handoverCond:'Bareshell',currentTenant:'ว่าง',renovationPlan:'-',status:'available',match:79,
    extras:{stores:'~200 ร้าน',occupancy:'87%',gla:'~85,000 ตร.ม.',traffic:'~50,000/วัน',
      parking:'2,200 รถยนต์',anchor:'Tops, Robinson, SF Cinema',supermarket:'Tops',
      demographic:'Family Hatyai 60% · Malaysian tourist 25% · BKK tourist 10%',transport:'รถยนต์ 85%'},
    contact:'leasing@cpn.co.th'},
  {id:'p100',title:'ยูนิต Robinson Lifestyle Sriracha',mall:'Robinson Lifestyle Sriracha',landlord:'CPN/Robinson',type:'community',region:'east',district:'ศรีราชา (ชลบุรี)',
    lat:13.1670,lng:100.9226,size:60,rent:48000,service:5000,cam:3500,deposit:'6 เดือน',escalation:'5%',
    leaseTerm:'3+3',handoverDate:'15 ก.ค. 2026',fitout:'30 วัน',handoverCond:'Bareshell',currentTenant:'ว่าง',renovationPlan:'-',status:'available',match:76,
    extras:{stores:'~120 ร้าน',occupancy:'88%',gla:'~32,000 ตร.ม.',traffic:'~25,000/วัน',
      parking:'1,200 รถยนต์',anchor:'Robinson, Tops, Major Cineplex',
      demographic:'Family + Japanese expat (Sriracha cluster)',transport:'รถยนต์ 90%'},contact:'leasing@cpn.co.th'},
  {id:'p110',title:'ยูนิต Future Park Rangsit',mall:'Future Park Rangsit',landlord:'Future Park',type:'mall',region:'bkk',district:'ธัญบุรี (ปทุมธานี)',
    lat:14.0220,lng:100.7212,size:65,rent:75000,service:9000,cam:5000,deposit:'6 เดือน',escalation:'5%',
    leaseTerm:'3+3',handoverDate:'15 ส.ค. 2026',fitout:'45 วัน',handoverCond:'Bareshell',currentTenant:'มีผู้เช่าเดิม — รับ As-is 30 มิ.ย. 2026',renovationPlan:'รีเฟรช Zpell ปี 2027',
    status:'available',match:82,
    extras:{stores:'~600 ร้าน',occupancy:'94%',gla:'~500,000 ตร.ม.',traffic:'~200,000/วัน',
      parking:'10,000 รถยนต์',anchor:'Robinson, Tops, Big C Extra, Major Cineplex, SF Cinema',
      mix:'F&B 25% · Fashion 30% · Specialty 25% · Lifestyle 20%',
      demographic:'Family ปริมณฑลเหนือ 75% · Student (ม.ราชภัฏ/ม.รังสิต) 15%',transport:'รถยนต์ 85% · Mini Bus 10%'},
    contact:'leasing@futurepark.co.th'},
];

/* ====== BRAND store coordinates — sample dataset เพื่อใช้บน Map (ดัชนีสาขาแบบสุ่ม) ====== */
const BRAND_STORES = [
  {brand:'After You',lat:13.7466,lng:100.5394,branch:'CentralWorld'},
  {brand:'After You',lat:13.7305,lng:100.5697,branch:'EmQuartier'},
  {brand:'After You',lat:13.7261,lng:100.5106,branch:'ICONSIAM'},
  {brand:'After You',lat:13.7448,lng:100.5343,branch:'Siam Paragon'},
  {brand:'After You',lat:13.6483,lng:100.6831,branch:'Mega Bangna'},
  {brand:'After You',lat:18.8044,lng:99.0288,branch:'Central Chiangmai'},
  {brand:'Café Amazon',lat:13.7466,lng:100.5394,branch:'CentralWorld'},
  {brand:'Café Amazon',lat:13.7305,lng:100.5697,branch:'Em District'},
  {brand:'Café Amazon',lat:13.7261,lng:100.5106,branch:'ICONSIAM'},
  {brand:'Café Amazon',lat:14.0220,lng:100.7212,branch:'Future Park'},
  {brand:'Café Amazon',lat:7.8929,lng:98.3793,branch:'Central Phuket Floresta'},
  {brand:'Café Amazon',lat:18.8044,lng:99.0288,branch:'Central Chiangmai'},
  {brand:'Café Amazon',lat:14.9799,lng:102.0978,branch:'Central Korat'},
  {brand:'Starbucks (TH)',lat:13.7466,lng:100.5394,branch:'CentralWorld'},
  {brand:'Starbucks (TH)',lat:13.7282,lng:100.5343,branch:'Silom Complex'},
  {brand:'Starbucks (TH)',lat:13.7305,lng:100.5697,branch:'EmQuartier'},
  {brand:'Starbucks (TH)',lat:13.7261,lng:100.5106,branch:'ICONSIAM'},
  {brand:'Starbucks (TH)',lat:13.6483,lng:100.6831,branch:'Mega Bangna'},
  {brand:'Starbucks (TH)',lat:7.8929,lng:98.3793,branch:'Phuket Floresta'},
  {brand:'Don Don Donki',lat:13.7376,lng:100.5784,branch:'Thonglor (The Market)'},
  {brand:'Don Don Donki',lat:13.7305,lng:100.5697,branch:'EmSphere'},
  {brand:'Don Don Donki',lat:13.7050,lng:100.6020,branch:'On Nut (Habito)'},
  {brand:'Don Don Donki',lat:13.6483,lng:100.6831,branch:'Mega Bangna'},
  {brand:'Don Don Donki',lat:13.7691,lng:100.5651,branch:'The Street Ratchada'},
  {brand:'Don Don Donki',lat:12.9276,lng:100.8780,branch:'Pattaya'},
  {brand:'Daiso',lat:13.7466,lng:100.5394,branch:'CentralWorld'},
  {brand:'Daiso',lat:13.7448,lng:100.5343,branch:'Siam Square One'},
  {brand:'Daiso',lat:13.7374,lng:100.5604,branch:'Terminal 21 Asok'},
  {brand:'Daiso',lat:13.6483,lng:100.6831,branch:'Mega Bangna'},
  {brand:'Daiso',lat:14.0220,lng:100.7212,branch:'Future Park'},
  {brand:'Daiso',lat:18.8044,lng:99.0288,branch:'Central Chiangmai'},
  {brand:'Daiso',lat:7.8929,lng:98.3793,branch:'Phuket Floresta'},
  {brand:'Uniqlo',lat:13.7466,lng:100.5394,branch:'CentralWorld'},
  {brand:'Uniqlo',lat:13.7305,lng:100.5697,branch:'EmQuartier'},
  {brand:'Uniqlo',lat:13.7261,lng:100.5106,branch:'ICONSIAM'},
  {brand:'Uniqlo',lat:13.6483,lng:100.6831,branch:'Mega Bangna'},
  {brand:'Uniqlo',lat:14.0220,lng:100.7212,branch:'Future Park'},
  {brand:'Uniqlo',lat:7.8929,lng:98.3793,branch:'Phuket Floresta'},
  {brand:'MUJI',lat:13.7305,lng:100.5697,branch:'EmQuartier'},
  {brand:'MUJI',lat:13.7261,lng:100.5106,branch:'ICONSIAM'},
  {brand:'MUJI',lat:13.7466,lng:100.5394,branch:'CentralWorld'},
  {brand:'MUJI',lat:13.6483,lng:100.6831,branch:'Mega Bangna'},
  {brand:'IKEA',lat:13.6483,lng:100.6831,branch:'Bangna'},
  {brand:'IKEA',lat:13.8762,lng:100.4123,branch:'Bangyai (Westgate)'},
  {brand:'IKEA',lat:13.7305,lng:100.5697,branch:'Sukhumvit (EmSphere)'},
  {brand:'Watsons',lat:13.7466,lng:100.5394,branch:'CentralWorld'},
  {brand:'Watsons',lat:13.7448,lng:100.5343,branch:'Siam Paragon'},
  {brand:'Watsons',lat:13.7374,lng:100.5604,branch:'Terminal 21 Asok'},
  {brand:'Watsons',lat:13.6483,lng:100.6831,branch:'Mega Bangna'},
  {brand:'Watsons',lat:14.0220,lng:100.7212,branch:'Future Park'},
  {brand:'Boots',lat:13.7466,lng:100.5394,branch:'CentralWorld'},
  {brand:'Boots',lat:13.7282,lng:100.5343,branch:'Silom Complex'},
  {brand:'Boots',lat:13.7305,lng:100.5697,branch:'EmQuartier'},
  {brand:'Boots',lat:13.7374,lng:100.5604,branch:'Terminal 21 Asok'},
  {brand:'Sephora',lat:13.7466,lng:100.5394,branch:'CentralWorld'},
  {brand:'Sephora',lat:13.7448,lng:100.5343,branch:'Siam Paragon'},
  {brand:'Sephora',lat:13.7305,lng:100.5697,branch:'EmQuartier'},
  {brand:'Sephora',lat:13.7261,lng:100.5106,branch:'ICONSIAM'},
  {brand:'MK Restaurants',lat:13.7466,lng:100.5394,branch:'CentralWorld'},
  {brand:'MK Restaurants',lat:13.7282,lng:100.5343,branch:'Silom Complex'},
  {brand:'MK Restaurants',lat:13.6483,lng:100.6831,branch:'Mega Bangna'},
  {brand:'MK Restaurants',lat:14.0220,lng:100.7212,branch:'Future Park'},
  {brand:'MK Restaurants',lat:18.8044,lng:99.0288,branch:'Central Chiangmai'},
  {brand:'Sushiro',lat:13.7466,lng:100.5394,branch:'CentralWorld'},
  {brand:'Sushiro',lat:13.7305,lng:100.5697,branch:'EmQuartier'},
  {brand:'Sushiro',lat:13.6483,lng:100.6831,branch:'Mega Bangna'},
  {brand:'Sushiro',lat:13.7261,lng:100.5106,branch:'ICONSIAM'},
  {brand:'Bonchon',lat:13.7466,lng:100.5394,branch:'CentralWorld'},
  {brand:'Bonchon',lat:13.7282,lng:100.5343,branch:'Silom Complex'},
  {brand:'Bonchon',lat:13.7374,lng:100.5604,branch:'Terminal 21 Asok'},
  {brand:'KFC (TH)',lat:13.7466,lng:100.5394,branch:'CentralWorld'},
  {brand:'KFC (TH)',lat:13.7282,lng:100.5343,branch:'Silom Complex'},
  {brand:'KFC (TH)',lat:13.6483,lng:100.6831,branch:'Mega Bangna'},
  {brand:'KFC (TH)',lat:14.0220,lng:100.7212,branch:'Future Park'},
  {brand:'KFC (TH)',lat:18.8044,lng:99.0288,branch:'Central Chiangmai'},
  {brand:"McDonald's (TH)",lat:13.7466,lng:100.5394,branch:'CentralWorld'},
  {brand:"McDonald's (TH)",lat:13.7282,lng:100.5343,branch:'Silom Complex'},
  {brand:"McDonald's (TH)",lat:13.7374,lng:100.5604,branch:'Terminal 21 Asok'},
];

/* ====== BRAND LOGO DOMAINS (Clearbit + Google favicon fallback) ====== */
const BRAND_DOMAINS = {
  'afteryou':'afteryoudessert.com','cafe-amazon':'cafe-amazon.com','starbucks':'starbucks.co.th',
  'mk':'mkrestaurant.com','sushiro':'akindo-sushiro.co.jp','bonchon':'bonchon.co.th',
  'minor':'minor.com','crg':'crg.co.th','qsra':'pizzahut.co.th','oishi':'oishigroup.com',
  'zen':'zengroup.co.th','mcdonalds':'mcthai.co.th','kfc':'kfc.co.th','tims':'timhortons.com',
  'donki':'dondondonki.com','daiso':'daisojapan.com','uniqlo':'uniqlo.com','zara':'zara.com',
  'hm':'hm.com','muji':'muji.com','decathlon':'decathlon.co.th','sephora':'sephora.com',
  'watsons':'watsons.co.th','boots':'boots.co.th','eveandboy':'eveandboy.com',
  'index':'indexlivingmall.com','homepro':'homepro.co.th','thaiwatsadu':'thaiwatsadu.com',
  'ikea':'ikea.com','powerbuy':'powerbuy.co.th','7-11':'7eleven.co.th','lawson':'lawson108.com',
  'kidzania':'kidzaniabangkok.com','harborland':'harborland.co.th','funarium':'funarium.co.th',
  // batch 2
  'pepperlunch':'pepperlunch.com','krispy-kreme':'krispykreme.co.th','subway':'subway.co.th',
  'burger-king':'burgerking.co.th','aw':'aw.co.th','inthanin':'inthanin.co.th',
  'class-cafe':'class-cafe.com','arabica':'arabica.coffee','iberry':'iberryhomemade.com',
  'yenly-yours':'yenlyyours.com','bar-b-q-plaza':'barbqplaza.com','sukishi':'sukishi.com',
  'mo-mo-paradise':'momoparadise.co.th','shabushi':'oishigroup.com','tonkatsu-maisen':'maisen-thailand.com',
  'auntie-annes':'auntieannes.co.th','mister-donut':'misterdonut.co.th','dunkin':'dunkindonuts.co.th',
  'yoshinoya':'yoshinoya.co.th','coco-ichibanya':'ichibanya.co.jp',
  'charles-keith':'charleskeith.com','pomelo':'pomelofashion.com','mango':'mango.com',
  'levis':'levi.com','cos':'cos.com','pull-bear':'pullandbear.com','stradivarius':'stradivarius.com',
  'massimo-dutti':'massimodutti.com','crocs':'crocs.co.th','skechers':'skechers.co.th',
  'adidas':'adidas.co.th','nike':'nike.com','onitsuka':'onitsukatiger.com',
  'mac':'maccosmetics.co.th','innisfree':'innisfree.com','laneige':'laneige.com',
  'body-shop':'thebodyshop.co.th','bath-body-works':'bathandbodyworks.com',
  'istudio':'istudio.store','studio7':'studio7thailand.com','banana-it':'bnn.in.th',
  'jib':'jib.co.th','powermall':'powermall.co.th',
  'sb-furniture':'sbdesignsquare.com','modernform':'modernform.co.th','koncept':'koncept-furniture.com',
  'b2s':'b2s.co.th','se-ed':'se-ed.com','asia-books':'asiabooks.com','kinokuniya':'kinokuniya.com',
  'bounce':'bounce.in.th'
};

function brandLogo(id,size=40){
  const d=BRAND_DOMAINS[id];const px=size+'px';
  if(!d)return `<div style="width:${px};height:${px}" class="rounded-lg bg-slate-100 flex items-center justify-center text-slate-400 font-bold">●</div>`;
  return `<img src="https://logo.clearbit.com/${d}" onerror="this.onerror=null;this.src='https://www.google.com/s2/favicons?domain=${d}&sz=128'" style="width:${px};height:${px}" class="rounded-lg bg-white object-contain border border-slate-100 p-1" alt=""/>`;
}

/* ====== MALL LOCATIONS DICTIONARY (สำหรับ generate brand stores) ====== */
const MALL_LOCATIONS = {
  // Bangkok Core CBD
  'central-world':{name:'CentralWorld',lat:13.7466,lng:100.5394,region:'bkk'},
  'siam-paragon':{name:'Siam Paragon',lat:13.7460,lng:100.5340,region:'bkk'},
  'siam-center':{name:'Siam Center',lat:13.7459,lng:100.5300,region:'bkk'},
  'siam-discovery':{name:'Siam Discovery',lat:13.7461,lng:100.5320,region:'bkk'},
  'siam-square-one':{name:'Siam Square One',lat:13.7448,lng:100.5343,region:'bkk'},
  'mbk':{name:'MBK Center',lat:13.7444,lng:100.5300,region:'bkk'},
  'iconsiam':{name:'ICONSIAM',lat:13.7261,lng:100.5106,region:'bkk'},
  'emquartier':{name:'EmQuartier',lat:13.7305,lng:100.5697,region:'bkk'},
  'emsphere':{name:'EmSphere',lat:13.7298,lng:100.5688,region:'bkk'},
  'emporium':{name:'Emporium',lat:13.7310,lng:100.5694,region:'bkk'},
  'central-embassy':{name:'Central Embassy',lat:13.7437,lng:100.5478,region:'bkk'},
  'central-chidlom':{name:'Central Chidlom',lat:13.7445,lng:100.5450,region:'bkk'},
  'gaysorn':{name:'Gaysorn Village',lat:13.7449,lng:100.5410,region:'bkk'},
  'amarin':{name:'Amarin Plaza',lat:13.7448,lng:100.5430,region:'bkk'},
  'silom-complex':{name:'Silom Complex',lat:13.7282,lng:100.5343,region:'bkk'},
  'terminal21-asok':{name:'Terminal 21 Asok',lat:13.7374,lng:100.5604,region:'bkk'},
  'gateway-ekamai':{name:'Gateway Ekamai',lat:13.7197,lng:100.5853,region:'bkk'},
  'the-commons-thonglor':{name:'The Commons Thonglor',lat:13.7376,lng:100.5784,region:'bkk'},
  'donki-thonglor':{name:'Donki Mall Thonglor',lat:13.7376,lng:100.5784,region:'bkk'},
  // BKK Suburbs
  'mega-bangna':{name:'Mega Bangna',lat:13.6483,lng:100.6831,region:'bkk'},
  'central-bangna':{name:'CentralPlaza Bangna',lat:13.6680,lng:100.6068,region:'bkk'},
  'central-ladprao':{name:'CentralPlaza Ladprao',lat:13.8166,lng:100.5612,region:'bkk'},
  'central-pinklao':{name:'CentralPlaza Pinklao',lat:13.7775,lng:100.4860,region:'bkk'},
  'central-rama2':{name:'CentralPlaza Rama 2',lat:13.6597,lng:100.4346,region:'bkk'},
  'central-rama3':{name:'CentralPlaza Rama 3',lat:13.6912,lng:100.5333,region:'bkk'},
  'central-rama9':{name:'CentralPlaza Grand Rama 9',lat:13.7585,lng:100.5651,region:'bkk'},
  'central-chaengwattana':{name:'CentralPlaza Chaengwattana',lat:13.8842,lng:100.5500,region:'bkk'},
  'central-westgate':{name:'Central Westgate',lat:13.8762,lng:100.4123,region:'bkk'},
  'central-eastville':{name:'Central EastVille',lat:13.8074,lng:100.6189,region:'bkk'},
  'central-westville':{name:'Central WestVille',lat:13.8950,lng:100.4040,region:'bkk'},
  'fashion-island':{name:'Fashion Island',lat:13.8264,lng:100.6695,region:'bkk'},
  'the-promenade':{name:'The Promenade Ramintra',lat:13.8235,lng:100.6740,region:'bkk'},
  'show-dc':{name:'Show DC',lat:13.7567,lng:100.5613,region:'bkk'},
  'esplanade':{name:'Esplanade Ratchada',lat:13.7691,lng:100.5651,region:'bkk'},
  'union-mall':{name:'Union Mall',lat:13.8166,lng:100.5612,region:'bkk'},
  'future-park':{name:'Future Park Rangsit',lat:14.0220,lng:100.7212,region:'bkk'},
  'themall-bangkapi':{name:'The Mall Bangkapi',lat:13.7654,lng:100.6433,region:'bkk'},
  'themall-bangkae':{name:'The Mall Bangkae',lat:13.7106,lng:100.4067,region:'bkk'},
  'themall-ngamwongwan':{name:'The Mall Ngamwongwan',lat:13.8475,lng:100.5278,region:'bkk'},
  'themall-thapra':{name:'The Mall Thapra',lat:13.7174,lng:100.4760,region:'bkk'},
  'seacon-square':{name:'Seacon Square Srinakarin',lat:13.6889,lng:100.6428,region:'bkk'},
  'seacon-bangkae':{name:'Seacon Bangkae',lat:13.7140,lng:100.4076,region:'bkk'},
  'cdc':{name:'CDC Crystal Design Center',lat:13.7935,lng:100.6157,region:'bkk'},
  'crystal-ekamai-ramintra':{name:'The Crystal Ekamai-Ramintra',lat:13.7950,lng:100.6225,region:'bkk'},
  'asiatique':{name:'Asiatique The Riverfront',lat:13.7060,lng:100.5034,region:'bkk'},
  'platinum':{name:'Platinum Fashion Mall',lat:13.7503,lng:100.5398,region:'bkk'},
  'paradise-park':{name:'Paradise Park',lat:13.6888,lng:100.6443,region:'bkk'},
  'the-nine':{name:'The Nine Rama 9',lat:13.7480,lng:100.5810,region:'bkk'},
  'onnut-habito':{name:'Habito Mall On Nut',lat:13.7050,lng:100.6020,region:'bkk'},
  'i-am-park':{name:'I am Park Suanluang',lat:13.7400,lng:100.5901,region:'bkk'},
  'major-ratchayothin':{name:'Major Avenue Ratchayothin',lat:13.8389,lng:100.5675,region:'bkk'},
  // Chiang Mai / North
  'central-chiangmai':{name:'CentralFestival Chiangmai',lat:18.8044,lng:99.0288,region:'north'},
  'maya-chiangmai':{name:'Maya Lifestyle Chiangmai',lat:18.8019,lng:98.9678,region:'north'},
  'promenada-chiangmai':{name:'Promenada Chiangmai',lat:18.7560,lng:99.0383,region:'north'},
  'central-chiangrai':{name:'CentralPlaza Chiangrai',lat:19.9072,lng:99.8267,region:'north'},
  'central-lampang':{name:'CentralPlaza Lampang',lat:18.2783,lng:99.4933,region:'north'},
  // Northeast
  'central-korat':{name:'CentralPlaza Korat',lat:14.9799,lng:102.0978,region:'northeast'},
  'terminal21-korat':{name:'Terminal 21 Korat',lat:14.9716,lng:102.0782,region:'northeast'},
  'central-khonkaen':{name:'CentralPlaza Khonkaen',lat:16.4406,lng:102.8276,region:'northeast'},
  'central-udonthani':{name:'CentralPlaza Udonthani',lat:17.4138,lng:102.7878,region:'northeast'},
  'central-ubon':{name:'CentralPlaza Ubonratchathani',lat:15.2333,lng:104.8500,region:'northeast'},
  // East
  'central-pattaya':{name:'CentralFestival Pattaya Beach',lat:12.9276,lng:100.8780,region:'east'},
  'terminal21-pattaya':{name:'Terminal 21 Pattaya',lat:12.9610,lng:100.8916,region:'east'},
  'royal-garden-pattaya':{name:'Royal Garden Plaza Pattaya',lat:12.9301,lng:100.8800,region:'east'},
  'central-sriracha':{name:'Robinson Lifestyle Sriracha',lat:13.1670,lng:100.9226,region:'east'},
  'central-chonburi':{name:'CentralPlaza Chonburi',lat:13.3611,lng:100.9847,region:'east'},
  'central-rayong':{name:'CentralPlaza Rayong',lat:12.6849,lng:101.2543,region:'east'},
  // South
  'central-phuket-floresta':{name:'Central Phuket Floresta',lat:7.8929,lng:98.3793,region:'south'},
  'central-phuket-festival':{name:'Central Phuket Festival',lat:7.8902,lng:98.3779,region:'south'},
  'jungceylon':{name:'Jungceylon Phuket',lat:7.8950,lng:98.2960,region:'south'},
  'central-hatyai':{name:'CentralFestival Hatyai',lat:7.0086,lng:100.4747,region:'south'},
  'central-samui':{name:'CentralFestival Samui',lat:9.5350,lng:100.0625,region:'south'},
  'central-suratthani':{name:'CentralPlaza Surat Thani',lat:9.1382,lng:99.3215,region:'south'},
  'central-nakhonsithammarat':{name:'CentralPlaza Nakhonsithammarat',lat:8.4304,lng:99.9631,region:'south'},
  // Central
  'central-ayutthaya':{name:'CentralPlaza Ayutthaya',lat:14.3417,lng:100.5803,region:'central'},
  'central-nakhonsawan':{name:'CentralPlaza Nakhon Sawan',lat:15.7008,lng:100.1230,region:'central'},
  'bluport':{name:'Bluport Hua Hin',lat:12.5684,lng:99.9577,region:'central'},
};

/* ====== BRAND PRESENCE (brand → mall codes) — sample dataset เพื่อแสดงบนแผนที่ ====== */
/* หมายเหตุ: เป็นตัวอย่างสาขาตามแบรนด์ ไม่ใช่รายการครบทุกสาขา */
const BRAND_PRESENCE = {
  'cafe-amazon':['central-world','siam-paragon','iconsiam','emquartier','emsphere','terminal21-asok','silom-complex','mega-bangna','central-bangna','central-ladprao','central-pinklao','central-rama2','central-rama3','central-rama9','central-chaengwattana','central-westgate','central-eastville','fashion-island','future-park','themall-bangkapi','themall-bangkae','seacon-square','central-chiangmai','maya-chiangmai','central-korat','central-khonkaen','central-udonthani','central-pattaya','central-sriracha','central-phuket-floresta','central-hatyai','central-samui','central-suratthani','central-ayutthaya','central-chonburi','central-rayong','terminal21-korat','terminal21-pattaya','central-chiangrai','central-ubon','asiatique','show-dc'],
  'starbucks':['central-world','siam-paragon','iconsiam','emquartier','emsphere','emporium','central-embassy','central-chidlom','gaysorn','silom-complex','terminal21-asok','gateway-ekamai','mega-bangna','central-bangna','central-ladprao','central-rama9','central-westgate','central-eastville','fashion-island','future-park','themall-bangkapi','central-chiangmai','maya-chiangmai','central-korat','central-khonkaen','central-pattaya','central-phuket-floresta','jungceylon','central-hatyai','central-samui','central-ayutthaya','siam-square-one'],
  'mk':['central-world','siam-paragon','silom-complex','terminal21-asok','mega-bangna','central-bangna','central-ladprao','central-pinklao','central-rama2','central-rama9','central-chaengwattana','central-westgate','central-eastville','fashion-island','future-park','themall-bangkapi','themall-bangkae','seacon-square','seacon-bangkae','central-chiangmai','central-korat','central-khonkaen','central-pattaya','central-phuket-floresta','central-hatyai','union-mall','the-nine','paradise-park'],
  'kfc':['central-world','siam-paragon','mbk','silom-complex','terminal21-asok','mega-bangna','central-bangna','central-ladprao','central-pinklao','central-rama2','central-rama9','central-westgate','fashion-island','future-park','themall-bangkapi','seacon-square','central-chiangmai','central-korat','central-khonkaen','central-udonthani','central-pattaya','central-phuket-floresta','central-hatyai','central-samui','platinum','asiatique','show-dc','the-nine'],
  'mcdonalds':['central-world','siam-paragon','mbk','silom-complex','terminal21-asok','mega-bangna','central-bangna','central-ladprao','central-rama2','central-rama9','central-westgate','fashion-island','future-park','themall-bangkapi','central-chiangmai','central-korat','central-pattaya','central-phuket-floresta','central-hatyai','asiatique','siam-square-one','union-mall'],
  'bonchon':['central-world','siam-paragon','iconsiam','emquartier','silom-complex','terminal21-asok','mega-bangna','central-bangna','central-ladprao','central-rama9','central-westgate','central-eastville','fashion-island','future-park','themall-bangkapi','central-chiangmai','central-korat','central-pattaya','siam-square-one','the-nine'],
  'sushiro':['central-world','siam-paragon','iconsiam','emquartier','emsphere','terminal21-asok','mega-bangna','central-bangna','central-ladprao','central-rama9','central-westgate','central-eastville','fashion-island','future-park','themall-bangkapi','central-chiangmai','central-pattaya','central-phuket-floresta'],
  'afteryou':['central-world','siam-paragon','iconsiam','emquartier','emsphere','terminal21-asok','mega-bangna','central-ladprao','central-rama9','central-westgate','central-eastville','future-park','themall-bangkapi','central-chiangmai','maya-chiangmai','central-pattaya','central-phuket-floresta','central-hatyai','central-samui','siam-square-one','the-commons-thonglor'],
  'oishi':['central-world','siam-paragon','terminal21-asok','mega-bangna','central-bangna','central-ladprao','central-rama2','central-rama9','central-westgate','fashion-island','future-park','themall-bangkapi','central-chiangmai','central-korat','central-pattaya','central-phuket-floresta'],
  'zen':['central-world','siam-paragon','iconsiam','emquartier','terminal21-asok','mega-bangna','central-bangna','central-ladprao','central-rama9','central-westgate','central-eastville','fashion-island','future-park','central-chiangmai','central-korat','central-pattaya','central-phuket-floresta'],
  'donki':['donki-thonglor','emsphere','onnut-habito','mega-bangna','esplanade','central-pattaya','i-am-park'],
  'daiso':['central-world','siam-square-one','siam-paragon','mbk','terminal21-asok','mega-bangna','central-bangna','central-ladprao','central-pinklao','central-rama2','central-rama9','central-westgate','central-eastville','fashion-island','future-park','themall-bangkapi','seacon-square','central-chiangmai','central-korat','central-khonkaen','central-pattaya','central-phuket-floresta','central-hatyai','platinum','union-mall'],
  'tims':['central-world','siam-paragon','emquartier','central-rama9','mega-bangna','central-ladprao','central-eastville','central-westgate','themall-bangkapi'],
  'uniqlo':['central-world','siam-paragon','iconsiam','emquartier','emsphere','terminal21-asok','mega-bangna','central-bangna','central-ladprao','central-pinklao','central-rama2','central-rama9','central-westgate','central-eastville','fashion-island','future-park','themall-bangkapi','central-chiangmai','central-korat','central-pattaya','central-phuket-floresta','central-hatyai','siam-square-one'],
  'zara':['central-world','siam-paragon','iconsiam','emquartier','central-embassy','central-chidlom','mega-bangna','central-ladprao','central-rama9','central-westgate','central-chiangmai','central-pattaya','central-phuket-floresta'],
  'hm':['central-world','siam-paragon','iconsiam','emquartier','terminal21-asok','mega-bangna','central-ladprao','central-rama9','central-westgate','central-eastville','fashion-island','future-park','central-chiangmai','central-pattaya','central-phuket-floresta','siam-square-one'],
  'muji':['central-world','siam-paragon','iconsiam','emquartier','emsphere','central-embassy','central-chidlom','terminal21-asok','mega-bangna','central-ladprao','central-rama9','central-westgate','central-chiangmai','central-pattaya','central-phuket-floresta','siam-discovery'],
  'decathlon':['mega-bangna','central-westgate','central-rama9','central-bangna','central-eastville','central-chiangmai'],
  'sephora':['central-world','siam-paragon','iconsiam','emquartier','central-embassy','terminal21-asok','mega-bangna','central-ladprao','central-rama9','central-westgate','central-chiangmai','central-phuket-floresta','siam-square-one'],
  'watsons':['central-world','siam-paragon','iconsiam','emquartier','terminal21-asok','silom-complex','mega-bangna','central-bangna','central-ladprao','central-pinklao','central-rama2','central-rama3','central-rama9','central-chaengwattana','central-westgate','central-eastville','fashion-island','future-park','themall-bangkapi','themall-bangkae','seacon-square','central-chiangmai','central-korat','central-khonkaen','central-udonthani','central-pattaya','central-phuket-floresta','central-hatyai','central-samui','union-mall','platinum'],
  'boots':['central-world','siam-paragon','iconsiam','emquartier','emsphere','terminal21-asok','silom-complex','mega-bangna','central-bangna','central-ladprao','central-rama9','central-westgate','central-eastville','fashion-island','future-park','themall-bangkapi','central-chiangmai','central-korat','central-pattaya','central-phuket-floresta','central-hatyai','siam-square-one','siam-center'],
  'eveandboy':['central-world','siam-paragon','siam-square-one','emquartier','mega-bangna','central-ladprao','central-rama9','central-westgate','central-eastville','future-park','central-chiangmai','central-pattaya','central-phuket-floresta'],
  'ikea':['mega-bangna','central-westgate','emsphere'],
  'homepro':['central-rama2','central-rama3','central-bangna','central-chaengwattana','central-westgate','central-pinklao','mega-bangna','future-park','central-eastville','central-chiangmai','central-korat','central-khonkaen','central-udonthani','central-pattaya','central-phuket-floresta','central-hatyai'],
  'index':['central-bangna','central-rama2','central-chaengwattana','central-westgate','mega-bangna','future-park','central-chiangmai','central-korat','central-khonkaen','central-pattaya','central-phuket-floresta','central-hatyai'],
  'powerbuy':['central-world','siam-paragon','emquartier','terminal21-asok','mega-bangna','central-bangna','central-ladprao','central-rama2','central-rama9','central-westgate','central-eastville','fashion-island','future-park','central-chiangmai','central-korat','central-pattaya','central-phuket-floresta','central-hatyai'],
  // batch 2
  'inthanin':['central-world','siam-paragon','iconsiam','emquartier','terminal21-asok','mega-bangna','central-bangna','central-ladprao','central-pinklao','central-rama2','central-rama9','central-westgate','central-eastville','fashion-island','future-park','themall-bangkapi','seacon-square','central-chiangmai','maya-chiangmai','central-korat','central-khonkaen','central-udonthani','central-pattaya','central-sriracha','central-phuket-floresta','central-hatyai','central-samui','central-ayutthaya','asiatique','union-mall','platinum'],
  'subway':['central-world','siam-paragon','silom-complex','terminal21-asok','mega-bangna','central-bangna','central-ladprao','central-rama9','central-westgate','fashion-island','future-park','central-chiangmai','central-pattaya','central-phuket-floresta'],
  'burger-king':['central-world','siam-paragon','silom-complex','terminal21-asok','mega-bangna','central-bangna','central-ladprao','central-rama2','central-rama9','central-westgate','fashion-island','future-park','central-chiangmai','central-korat','central-pattaya','central-phuket-floresta'],
  'mister-donut':['central-world','siam-paragon','siam-square-one','terminal21-asok','mega-bangna','central-bangna','central-ladprao','central-pinklao','central-rama2','central-rama9','central-westgate','central-eastville','fashion-island','future-park','themall-bangkapi','seacon-square','central-chiangmai','central-korat','central-khonkaen','central-pattaya','central-phuket-floresta','central-hatyai'],
  'dunkin':['central-world','siam-paragon','mbk','silom-complex','terminal21-asok','mega-bangna','central-bangna','central-ladprao','central-rama9','central-westgate','fashion-island','future-park','themall-bangkapi','central-chiangmai','central-korat','central-pattaya','union-mall'],
  'auntie-annes':['central-world','siam-paragon','mbk','silom-complex','terminal21-asok','mega-bangna','central-bangna','central-ladprao','central-rama2','central-rama9','central-westgate','central-eastville','fashion-island','future-park','themall-bangkapi','seacon-square','central-chiangmai','central-pattaya','central-phuket-floresta'],
  'bar-b-q-plaza':['central-world','siam-paragon','mega-bangna','central-bangna','central-ladprao','central-pinklao','central-rama2','central-rama9','central-westgate','central-eastville','fashion-island','future-park','themall-bangkapi','seacon-square','central-chiangmai','central-korat','central-khonkaen','central-pattaya','central-phuket-floresta','central-hatyai'],
  'sukishi':['central-world','siam-paragon','mega-bangna','central-bangna','central-ladprao','central-rama9','central-westgate','fashion-island','future-park','central-chiangmai','central-korat','central-pattaya','central-phuket-floresta'],
  'shabushi':['central-world','siam-paragon','silom-complex','mega-bangna','central-bangna','central-ladprao','central-rama2','central-rama9','central-westgate','central-eastville','fashion-island','future-park','themall-bangkapi','seacon-square','central-chiangmai','central-korat','central-khonkaen','central-pattaya','central-phuket-floresta','central-hatyai'],
  'pepperlunch':['central-world','siam-paragon','emquartier','terminal21-asok','mega-bangna','central-bangna','central-ladprao','central-rama9','central-westgate','fashion-island','future-park','central-chiangmai','central-pattaya'],
  'mo-mo-paradise':['central-world','siam-paragon','iconsiam','emquartier','terminal21-asok','mega-bangna','central-rama9','central-westgate','central-chiangmai','central-phuket-floresta'],
  'coco-ichibanya':['central-world','siam-paragon','emquartier','terminal21-asok','mega-bangna','central-rama9','central-eastville','central-chiangmai','central-pattaya','central-phuket-floresta'],
  'iberry':['central-world','siam-paragon','emquartier','iconsiam','mega-bangna','central-ladprao','central-rama9','central-westgate','central-chiangmai','central-pattaya','central-phuket-floresta'],
  'yenly-yours':['central-world','siam-paragon','iconsiam','emquartier','siam-square-one','terminal21-asok','mega-bangna','central-rama9','central-westgate','central-chiangmai','central-phuket-floresta'],
  'tonkatsu-maisen':['central-world','siam-paragon','emquartier','iconsiam','central-embassy','mega-bangna','central-chiangmai'],
  'krispy-kreme':['central-world','siam-paragon','iconsiam','emquartier','terminal21-asok','mega-bangna','central-ladprao','central-rama9','central-westgate','future-park','central-chiangmai','central-pattaya','central-phuket-floresta'],
  'arabica':['iconsiam','central-embassy','emsphere','asiatique','central-phuket-floresta','siam-paragon','gaysorn','siam-discovery'],
  'charles-keith':['central-world','siam-paragon','iconsiam','emquartier','central-embassy','terminal21-asok','mega-bangna','central-ladprao','central-rama9','central-westgate','central-eastville','central-chiangmai','central-pattaya','central-phuket-floresta','central-hatyai'],
  'pomelo':['central-world','siam-paragon','siam-square-one','emquartier','iconsiam','terminal21-asok','mega-bangna','central-ladprao','central-rama9','central-westgate','central-chiangmai','central-pattaya','central-phuket-floresta'],
  'mango':['central-world','siam-paragon','iconsiam','emquartier','central-embassy','mega-bangna','central-ladprao','central-rama9','central-westgate','central-chiangmai','central-pattaya','central-phuket-floresta'],
  'levis':['central-world','siam-paragon','iconsiam','emquartier','terminal21-asok','mega-bangna','central-bangna','central-ladprao','central-rama9','central-westgate','fashion-island','future-park','central-chiangmai','central-korat','central-pattaya','central-phuket-floresta','siam-center'],
  'crocs':['central-world','siam-paragon','iconsiam','emquartier','terminal21-asok','mega-bangna','central-bangna','central-ladprao','central-rama9','central-westgate','fashion-island','future-park','central-chiangmai','central-pattaya','central-phuket-floresta'],
  'skechers':['central-world','siam-paragon','iconsiam','emquartier','terminal21-asok','mega-bangna','central-bangna','central-ladprao','central-pinklao','central-rama2','central-rama9','central-westgate','central-eastville','fashion-island','future-park','themall-bangkapi','central-chiangmai','central-korat','central-pattaya','central-phuket-floresta','central-hatyai'],
  'adidas':['central-world','siam-paragon','iconsiam','emquartier','siam-center','terminal21-asok','mega-bangna','central-bangna','central-ladprao','central-rama9','central-westgate','central-eastville','fashion-island','future-park','themall-bangkapi','central-chiangmai','central-korat','central-pattaya','central-phuket-floresta','central-hatyai'],
  'nike':['central-world','siam-paragon','iconsiam','emquartier','siam-center','siam-square-one','terminal21-asok','mega-bangna','central-bangna','central-ladprao','central-rama9','central-westgate','central-eastville','fashion-island','future-park','themall-bangkapi','central-chiangmai','central-korat','central-pattaya','central-phuket-floresta','central-hatyai'],
  'onitsuka':['central-world','siam-paragon','iconsiam','emquartier','central-embassy','mega-bangna','central-ladprao','central-rama9','central-westgate','central-chiangmai','central-pattaya','central-phuket-floresta'],
  'mac':['central-world','siam-paragon','iconsiam','emquartier','emporium','central-embassy','central-chidlom','mega-bangna','central-ladprao','central-rama9','central-westgate','central-chiangmai','central-pattaya','central-phuket-floresta'],
  'innisfree':['central-world','siam-paragon','siam-square-one','iconsiam','emquartier','mega-bangna','central-ladprao','central-rama9','central-westgate','central-eastville','central-chiangmai','central-pattaya','central-phuket-floresta'],
  'laneige':['central-world','siam-paragon','iconsiam','emquartier','terminal21-asok','mega-bangna','central-ladprao','central-rama9','central-westgate','central-chiangmai','central-pattaya'],
  'body-shop':['central-world','siam-paragon','iconsiam','emquartier','silom-complex','terminal21-asok','mega-bangna','central-bangna','central-ladprao','central-rama9','central-westgate','central-eastville','fashion-island','future-park','central-chiangmai','central-korat','central-pattaya','central-phuket-floresta','central-hatyai'],
  'bath-body-works':['central-world','siam-paragon','iconsiam','emquartier','central-embassy','mega-bangna','central-ladprao','central-rama9','central-westgate','central-chiangmai','central-phuket-floresta'],
  'istudio':['central-world','siam-paragon','iconsiam','emquartier','emsphere','central-embassy','terminal21-asok','mega-bangna','central-bangna','central-ladprao','central-rama2','central-rama9','central-westgate','central-eastville','fashion-island','future-park','themall-bangkapi','central-chiangmai','central-korat','central-pattaya','central-phuket-floresta','central-hatyai'],
  'studio7':['central-world','siam-paragon','iconsiam','emquartier','terminal21-asok','mega-bangna','central-bangna','central-ladprao','central-rama9','central-westgate','central-eastville','fashion-island','future-park','central-chiangmai','central-korat','central-pattaya','central-phuket-floresta'],
  'banana-it':['central-world','siam-paragon','mbk','siam-square-one','siam-discovery','silom-complex','terminal21-asok','mega-bangna','central-bangna','central-ladprao','central-rama2','central-rama9','central-westgate','central-eastville','fashion-island','future-park','themall-bangkapi','seacon-square','central-chiangmai','central-korat','central-khonkaen','central-pattaya','central-phuket-floresta','central-hatyai','union-mall'],
  'jib':['mbk','fashion-island','seacon-square','mega-bangna','central-rama9','future-park','central-chiangmai','central-korat'],
  'powermall':['emporium','emquartier','emsphere','themall-bangkapi','themall-bangkae','themall-ngamwongwan','themall-thapra','bluport'],
  'sb-furniture':['central-rama2','central-rama3','central-chaengwattana','central-westgate','central-pinklao','mega-bangna','seacon-square','crystal-ekamai-ramintra','cdc','central-chiangmai','central-korat','central-pattaya'],
  'modernform':['central-rama2','central-bangna','central-westgate','mega-bangna','crystal-ekamai-ramintra','cdc','central-chiangmai','central-pattaya'],
  'b2s':['central-world','siam-paragon','central-embassy','iconsiam','emquartier','terminal21-asok','mega-bangna','central-bangna','central-ladprao','central-pinklao','central-rama2','central-rama9','central-westgate','central-eastville','fashion-island','future-park','central-chiangmai','central-korat','central-khonkaen','central-pattaya','central-phuket-floresta','central-hatyai'],
  'se-ed':['central-world','siam-paragon','siam-square-one','mbk','terminal21-asok','mega-bangna','central-bangna','central-ladprao','central-pinklao','central-rama2','central-rama9','central-westgate','central-eastville','fashion-island','future-park','themall-bangkapi','seacon-square','central-chiangmai','central-korat','central-khonkaen','central-pattaya','central-phuket-floresta','central-hatyai','union-mall'],
  'asia-books':['central-world','siam-paragon','emquartier','central-embassy','iconsiam','terminal21-asok','central-chidlom','central-chiangmai','central-phuket-floresta'],
  'kinokuniya':['siam-paragon','emquartier','central-world','central-chidlom','iconsiam'],
  'bounce':['esplanade','central-westgate','mega-bangna','central-eastville','central-chiangmai'],
};

/* Generate brand stores from BRAND_PRESENCE */
Object.entries(BRAND_PRESENCE).forEach(([brandId,malls])=>{
  const b=BRANDS.find(x=>x.id===brandId);if(!b)return;
  malls.forEach(mc=>{
    const loc=MALL_LOCATIONS[mc];if(!loc)return;
    BRAND_STORES.push({brand:b.name,brandId,lat:loc.lat,lng:loc.lng,branch:loc.name,mallCode:mc});
  });
});

/* =========================================================
   RENDERERS / FILTERS
   ========================================================= */
function fmt(n){return Number(n).toLocaleString('th-TH')}
function statusBadge(s){
  if(s==='available')return '<span class="pill badge-green">ว่าง</span>';
  if(s==='coming-soon')return '<span class="pill badge-blue">เร็วๆ นี้</span>';
  if(s==='leased')return '<span class="pill badge-slate">ปล่อยเช่าแล้ว</span>';
  return '<span class="pill badge-slate">-</span>';
}
function typeBadge(t){
  const m={mall:'ห้าง',standalone:'ตึกแถว',kiosk:'Kiosk',land:'ที่ดิน',community:'Community'};
  return `<span class="pill badge-slate">${m[t]||t}</span>`;
}

function propertyCard(p){
  return `<a href="javascript:void(0)" onclick="openProperty('${p.id}')" class="card block bg-white rounded-2xl border border-slate-200 overflow-hidden">
    <div class="aspect-[4/3] bg-gradient-to-br from-slate-200 to-slate-300 relative flex items-center justify-center">
      <div class="text-slate-400 text-3xl">${p.type==='land'?'🟫':p.type==='kiosk'?'🛒':p.type==='standalone'?'🏪':'🏬'}</div>
      <div class="absolute top-2.5 left-2.5">${statusBadge(p.status)}</div>
      <div class="absolute bottom-2.5 right-2.5 bg-white/90 rounded-full w-10 h-10 flex items-center justify-center text-xs font-bold text-emerald-700 shadow">${p.match||'—'}</div>
    </div>
    <div class="p-3.5">
      <div class="text-sm font-semibold line-clamp-1">${p.title}</div>
      <div class="text-xs text-slate-500 flex items-center gap-1 mt-1">📍 ${p.district}</div>
      <div class="flex items-end justify-between mt-2">
        <div>
          <div class="text-base font-bold text-blue-600">${p.rent?'฿'+fmt(p.rent)+'/เดือน':'ติดต่อ'}</div>
          <div class="text-xs text-slate-500">${p.size>1000?fmt(p.size)+' ตร.ม. ('+(p.size/1600).toFixed(1)+' ไร่)':fmt(p.size)+' ตร.ม.'}</div>
        </div>
        ${typeBadge(p.type)}
      </div>
    </div>
  </a>`;
}

function brandCard(b){
  const statusMap={active:'<span class="pill badge-green">Active Scouting</span>',
    selective:'<span class="pill badge-amber">Selective</span>',
    paused:'<span class="pill badge-slate">Paused</span>'};
  return `<a href="javascript:void(0)" onclick="openBrand('${b.id}')" class="card block bg-white rounded-2xl border border-slate-200 p-4">
    <div class="flex items-center justify-between gap-2">
      <div class="flex items-center gap-3 min-w-0">
        ${brandLogo(b.id,44)}
        <div class="min-w-0">
          <div class="font-bold text-base leading-tight truncate">${b.name}</div>
          <div class="text-xs text-slate-500 mt-0.5 truncate">${b.sub}</div>
        </div>
      </div>
      ${statusMap[b.status]||''}
    </div>
    <div class="grid grid-cols-3 gap-2 mt-3 text-center">
      <div class="bg-slate-50 rounded-lg py-2"><div class="text-base font-bold text-slate-900">${b.branches.total}</div><div class="text-[10px] text-slate-500">สาขาปัจจุบัน</div></div>
      <div class="bg-blue-50 rounded-lg py-2"><div class="text-xs font-bold text-blue-700 leading-tight px-1">${(b.expansion||'').split('·')[0]}</div><div class="text-[10px] text-slate-500">แผนขยาย</div></div>
      <div class="bg-emerald-50 rounded-lg py-2"><div class="text-xs font-bold text-emerald-700">${b.size}</div><div class="text-[10px] text-slate-500">ขนาดร้าน</div></div>
    </div>
    <div class="mt-3 flex flex-wrap gap-1">
      <span class="pill badge-blue">${b.cat}</span>
      ${(b.format||[]).slice(0,2).map(f=>`<span class="pill badge-slate">${f}</span>`).join('')}
    </div>
    <div class="text-xs text-blue-600 mt-3">ดูรายละเอียด BD contact →</div>
  </a>`;
}

function landlordCard(l){
  return `<a href="javascript:void(0)" onclick="openLandlord('${l.id}')" class="card block bg-white rounded-2xl border border-slate-200 p-4">
    <div class="flex items-center justify-between gap-2">
      <div>
        <div class="font-bold text-base">${l.name}</div>
        <div class="text-xs text-slate-500">${l.type} · ${l.group}</div>
      </div>
      <span class="pill badge-purple">${(l.keyMalls||[]).length} ห้าง</span>
    </div>
    <p class="text-xs text-slate-600 mt-3 line-clamp-3">${l.portfolio}</p>
    <div class="text-xs text-slate-500 mt-3 line-clamp-1">📧 ${l.contact?.leasing||'-'}</div>
    <div class="text-xs text-blue-600 mt-1">ดูรายละเอียดและพื้นที่ว่าง →</div>
  </a>`;
}

/* ===== MODAL OPEN FUNCTIONS ===== */
function openModal(html){
  const m=document.getElementById('modal');
  document.getElementById('modal-body').innerHTML=html;
  m.classList.add('open');document.body.style.overflow='hidden';
}
function closeModal(){document.getElementById('modal').classList.remove('open');document.body.style.overflow=''}

function openProperty(id){
  const p=PROPERTIES.find(x=>x.id===id);if(!p)return;
  const ex=p.extras||{};
  const html=`<div class="p-6">
    <div class="flex items-start justify-between gap-3">
      <div>
        <div class="flex items-center gap-2 flex-wrap">${statusBadge(p.status)}${typeBadge(p.type)}<span class="text-xs text-slate-500">📍 ${p.district}</span></div>
        <h2 class="text-2xl font-bold mt-2">${p.title}</h2>
        <div class="text-sm text-slate-500">${p.mall} · ${p.landlord}</div>
      </div>
      <button onclick="closeModal()" class="text-slate-400 hover:text-slate-700 text-2xl leading-none">×</button>
    </div>

    <div class="grid md:grid-cols-3 gap-4 mt-5">
      <div class="bg-blue-50 rounded-xl p-4"><div class="text-xs text-blue-700 font-semibold">ค่าเช่า</div><div class="text-2xl font-extrabold text-blue-700">฿${fmt(p.rent)}<span class="text-sm font-normal">/เดือน</span></div></div>
      <div class="bg-emerald-50 rounded-xl p-4"><div class="text-xs text-emerald-700 font-semibold">ขนาด</div><div class="text-2xl font-extrabold text-emerald-700">${fmt(p.size)} <span class="text-sm font-normal">ตร.ม.</span></div></div>
      <div class="bg-purple-50 rounded-xl p-4"><div class="text-xs text-purple-700 font-semibold">Match Score</div><div class="text-2xl font-extrabold text-purple-700">${p.match}%</div></div>
    </div>

    <h3 class="section-title mt-6">เงื่อนไขการเช่า (ข้อมูลที่จำเป็น)</h3>
    <dl class="grid grid-cols-2 md:grid-cols-4 gap-4 grid-row">
      <div><dt>ระยะเวลาเช่า</dt><dd>${p.leaseTerm}</dd></div>
      <div><dt>ค่าบริการ</dt><dd>฿${fmt(p.service)}/เดือน</dd></div>
      <div><dt>ค่าส่วนกลาง (CAM)</dt><dd>฿${fmt(p.cam)}/เดือน</dd></div>
      <div><dt>เงินประกัน</dt><dd>${p.deposit}</dd></div>
      <div><dt>เรทปรับขึ้น</dt><dd>${p.escalation}</dd></div>
      <div><dt>วันส่งมอบ (Handover)</dt><dd>${p.handoverDate}</dd></div>
      <div><dt>Fit-out Period</dt><dd>${p.fitout}</dd></div>
      <div><dt>ลักษณะส่งมอบ</dt><dd>${p.handoverCond}</dd></div>
    </dl>

    <div class="mt-4 bg-amber-50 border-l-4 border-amber-400 rounded-r-lg p-3">
      <div class="text-xs font-bold text-amber-800 uppercase mb-1">สถานะผู้เช่าเดิม</div>
      <div class="text-sm text-amber-900">${p.currentTenant}</div>
    </div>

    <div class="mt-3 bg-indigo-50 border-l-4 border-indigo-400 rounded-r-lg p-3">
      <div class="text-xs font-bold text-indigo-800 uppercase mb-1">แผนรีโนเวท 3-6 ปีข้างหน้า</div>
      <div class="text-sm text-indigo-900">${p.renovationPlan||'ไม่มีข้อมูล / สอบถามทาง landlord'}</div>
    </div>

    ${p.type!=='land'&&p.type!=='standalone'?`
    <h3 class="section-title mt-6">ข้อมูลศูนย์การค้า (ข้อมูลประกอบ)</h3>
    <dl class="grid grid-cols-2 md:grid-cols-4 gap-4 grid-row">
      <div><dt>จำนวนร้านค้า</dt><dd>${ex.stores||'-'}</dd></div>
      <div><dt>Occupancy Rate</dt><dd>${ex.occupancy||'-'}</dd></div>
      <div><dt>GLA ศูนย์</dt><dd>${ex.gla||'-'}</dd></div>
      <div><dt>Traffic</dt><dd>${ex.traffic||'-'}</dd></div>
      <div class="col-span-2"><dt>ที่จอด</dt><dd>${ex.parking||'-'}</dd></div>
      <div class="col-span-2"><dt>ร้านค้าหลัก (Anchor)</dt><dd>${ex.anchor||'-'}</dd></div>
      <div class="col-span-2"><dt>Supermarket</dt><dd>${ex.supermarket||'-'}</dd></div>
      <div class="col-span-2"><dt>สัดส่วนประเภทร้าน</dt><dd class="font-normal text-xs">${ex.mix||'-'}</dd></div>
      <div class="col-span-2"><dt>กลุ่มลูกค้า</dt><dd class="font-normal text-xs">${ex.demographic||'-'}</dd></div>
      <div class="col-span-2"><dt>วิธีเดินทาง</dt><dd class="font-normal text-xs">${ex.transport||'-'}</dd></div>
    </dl>
    `:''}

    <h3 class="section-title mt-6">เอกสารที่ต้องขอเพิ่ม</h3>
    <ul class="text-sm text-slate-700 space-y-1 list-disc pl-5">
      <li>ไฟล์ CAD และ M&E (วางผังประกอบการขออนุมัติ)</li>
      <li>ยอดขายของร้านค้าใกล้เคียงในโครงการ (หากเปิดเผยได้)</li>
      <li>ร้านที่ขายสินค้าใกล้เคียงในโครงการ — ตำแหน่ง</li>
      <li>ประเภทร้านค้าแต่ละชั้น/โซน (Tenant Mix Plan)</li>
      <li>เอกสารสนับสนุนอื่น ๆ (Brochure, Floor Plan, NRZ ฯลฯ)</li>
    </ul>

    <h3 class="section-title mt-6">ติดต่อ</h3>
    <div class="bg-slate-50 rounded-xl p-3 text-sm">📞 ${p.contact}</div>

    <div class="mt-5 flex flex-wrap gap-2">
      <button onclick="closeModal();switchTab('map');setTimeout(()=>focusMap(${p.lat},${p.lng}),300)" class="px-4 py-2 bg-slate-100 hover:bg-slate-200 rounded-lg text-sm">ดูบนแผนที่</button>
      <button onclick="window.print()" class="px-4 py-2 bg-blue-600 text-white hover:bg-blue-700 rounded-lg text-sm">Export PDF</button>
    </div>
  </div>`;
  openModal(html);
}

function openBrand(id){
  const b=BRANDS.find(x=>x.id===id);if(!b)return;
  const br=b.branches||{};
  const html=`<div class="p-6">
    <div class="flex items-start justify-between gap-3">
      <div class="flex items-start gap-4">
        ${brandLogo(b.id,64)}
        <div>
          <div class="text-xs text-slate-500">${b.sub} · ${b.parent}</div>
          <h2 class="text-2xl font-bold mt-1">${b.name}</h2>
          <div class="flex flex-wrap gap-1 mt-2">
            <span class="pill badge-blue">${b.cat}</span>
            ${(b.format||[]).map(f=>`<span class="pill badge-slate">${f}</span>`).join('')}
            ${b.status==='active'?'<span class="pill badge-green">Active Scouting</span>':b.status==='selective'?'<span class="pill badge-amber">Selective</span>':'<span class="pill badge-slate">Paused</span>'}
          </div>
        </div>
      </div>
      <button onclick="closeModal()" class="text-slate-400 hover:text-slate-700 text-2xl leading-none">×</button>
    </div>

    <h3 class="section-title mt-6">Footprint</h3>
    <div class="grid grid-cols-2 md:grid-cols-4 gap-3">
      <div class="bg-slate-50 rounded-xl p-3 text-center"><div class="text-xs text-slate-500">รวมทั้งหมด</div><div class="text-xl font-extrabold">${br.total||'-'}</div></div>
      <div class="bg-slate-50 rounded-xl p-3 text-center"><div class="text-xs text-slate-500">กรุงเทพฯ/ปริมณฑล</div><div class="text-xl font-extrabold">${br.bkk||'-'}</div></div>
      <div class="bg-slate-50 rounded-xl p-3 text-center"><div class="text-xs text-slate-500">ต่างจังหวัด</div><div class="text-xl font-extrabold">${br.upcountry||'-'}</div></div>
      <div class="bg-slate-50 rounded-xl p-3 text-center"><div class="text-xs text-slate-500">ต่างประเทศ</div><div class="text-xl font-extrabold">${br.overseas||'-'}</div></div>
    </div>

    <h3 class="section-title mt-6">แผนการขยายสาขา</h3>
    <div class="bg-blue-50 rounded-xl p-4 text-sm text-blue-900">${b.expansion||'-'}</div>

    <h3 class="section-title mt-6">Store Format & Site Criteria</h3>
    <dl class="grid grid-cols-2 gap-4 grid-row">
      <div><dt>รูปแบบร้าน</dt><dd>${(b.format||[]).join(' · ')}</dd></div>
      <div><dt>ขนาดร้านมาตรฐาน</dt><dd>${b.size||'-'}</dd></div>
      <div><dt>งบค่าเช่าที่รับได้</dt><dd>${b.rentBudget||'-'}</dd></div>
      <div><dt>เกณฑ์ทำเล</dt><dd class="font-normal text-xs">${b.siteCriteria||'-'}</dd></div>
      <div class="col-span-2"><dt>กลุ่มเป้าหมาย</dt><dd class="font-normal text-xs">${b.target||'-'}</dd></div>
    </dl>

    <h3 class="section-title mt-6">Business Development Contact</h3>
    <div class="bg-slate-50 rounded-xl p-4 text-sm space-y-1">
      ${b.bd?.name?`<div><strong>👤 ${b.bd.name}</strong></div>`:''}
      ${b.bd?.email?`<div>📧 <a class="text-blue-600 hover:underline" href="mailto:${b.bd.email}">${b.bd.email}</a></div>`:''}
      ${b.bd?.phone?`<div>📞 ${b.bd.phone}</div>`:''}
      ${b.bd?.hq?`<div>🏢 HQ: ${b.bd.hq}</div>`:''}
    </div>
 — ติดต่อผ่านหน้าเว็บบริษัทเพื่อขอชื่อผู้รับผิดชอบล่าสุด</div>
    ${b.notes?`<h3 class="section-title mt-6">หมายเหตุ</h3><div class="text-sm text-slate-700">${b.notes}</div>`:''}
    <div class="mt-5 flex flex-wrap gap-2">
      <button onclick="closeModal();switchTab('map');setTimeout(()=>showBrandOnMap('${b.name}'),300)" class="px-4 py-2 bg-blue-600 text-white hover:bg-blue-700 rounded-lg text-sm">ดูสาขาบนแผนที่</button>
      <button onclick="window.print()" class="px-4 py-2 bg-slate-100 hover:bg-slate-200 rounded-lg text-sm">Print Profile</button>
    </div>
  </div>`;
  openModal(html);
}

function openLandlord(id){
  const l=LANDLORDS.find(x=>x.id===id);if(!l)return;
  const malls=(l.keyMalls||[]).map(m=>`<li>${m}</li>`).join('')||'<li class="text-slate-500">-</li>';
  const html=`<div class="p-6">
    <div class="flex items-start justify-between gap-3">
      <div><div class="text-xs text-slate-500">${l.type} · ${l.group}</div>
      <h2 class="text-2xl font-bold mt-1">${l.name}</h2>
      <div class="text-xs text-slate-500 mt-1">🌐 ${l.web||'-'}</div></div>
      <button onclick="closeModal()" class="text-slate-400 hover:text-slate-700 text-2xl leading-none">×</button>
    </div>
    <h3 class="section-title mt-6">Portfolio</h3>
    <div class="bg-slate-50 rounded-xl p-4 text-sm">${l.portfolio}</div>
    ${l.gla?`<div class="text-xs text-slate-500 mt-2">รวม GLA: <strong>${l.gla}</strong></div>`:''}
    <h3 class="section-title mt-6">ห้าง / โครงการเด่น</h3>
    <ul class="grid grid-cols-2 md:grid-cols-3 gap-x-4 gap-y-1 text-sm list-disc pl-5">${malls}</ul>
    ${l.notes?`<h3 class="section-title mt-6">Note</h3><div class="text-sm">${l.notes}</div>`:''}
    <h3 class="section-title mt-6">ติดต่อ Leasing</h3>
    <div class="bg-slate-50 rounded-xl p-4 text-sm space-y-1">
      <div>🏢 ${l.hq||'-'}</div><div>📧 ${l.contact?.leasing||'-'}</div>
      <div>📞 ${l.contact?.phone||'-'}</div>${l.contact?.ir?`<div>📊 IR: ${l.contact.ir}</div>`:''}
    </div>
  </div>`;
  openModal(html);
}

function switchTab(t){
  document.querySelectorAll('.section').forEach(s=>s.classList.toggle('hidden',s.dataset.section!==t));
  document.querySelectorAll('.tab-btn,.tab-btn-m').forEach(b=>{
    if(b.dataset.tab===t){b.classList.add('tab-active');b.classList.remove('tab-inactive')}
    else{b.classList.remove('tab-active');b.classList.add('tab-inactive')}
  });
  if(t==='map')setTimeout(()=>map&&map.invalidateSize(),200);
  window.scrollTo({top:0,behavior:'smooth'});
}
document.querySelectorAll('.tab-btn,.tab-btn-m').forEach(b=>b.addEventListener('click',()=>switchTab(b.dataset.tab)));

document.getElementById('kpi-prop').textContent=PROPERTIES.filter(p=>p.type!=='land').length;
document.getElementById('kpi-brand').textContent=BRANDS.length;
document.getElementById('kpi-mall').textContent=LANDLORDS.length;
document.getElementById('kpi-land').textContent=PROPERTIES.filter(p=>p.type==='land').length+LAND_PLOTS.length;

const featured=[...PROPERTIES].sort((a,b)=>(b.match||0)-(a.match||0)).slice(0,8);
document.getElementById('featured-grid').innerHTML=featured.map(propertyCard).join('');

function renderProperties(){
  const q=document.getElementById('prop-search').value.toLowerCase();
  const t=document.getElementById('prop-type').value;
  const r=document.getElementById('prop-region').value;
  const sort=document.getElementById('prop-sort').value;
  let list=PROPERTIES.filter(p=>(!q||(p.title+p.mall+p.district+p.landlord).toLowerCase().includes(q))&&(!t||p.type===t)&&(!r||p.region===r));
  if(sort==='price_asc')list.sort((a,b)=>(a.rent||0)-(b.rent||0));
  else if(sort==='price_desc')list.sort((a,b)=>(b.rent||0)-(a.rent||0));
  else if(sort==='size_asc')list.sort((a,b)=>(a.size||0)-(b.size||0));
  else if(sort==='size_desc')list.sort((a,b)=>(b.size||0)-(a.size||0));
  else list.sort((a,b)=>(b.match||0)-(a.match||0));
  document.getElementById('prop-count').textContent=list.length+' รายการ';
  document.getElementById('prop-grid').innerHTML=list.map(propertyCard).join('')||'<div class="col-span-full text-center text-slate-500 py-10">ไม่พบ</div>';
}
['prop-search','prop-type','prop-region','prop-sort'].forEach(id=>document.getElementById(id).addEventListener('input',renderProperties));
renderProperties();

function renderBrands(){
  const q=document.getElementById('brand-search').value.toLowerCase();
  const c=document.getElementById('brand-cat').value;
  const s=document.getElementById('brand-status').value;
  const f=document.getElementById('brand-format').value;
  const list=BRANDS.filter(b=>(!q||(b.name+b.parent+b.sub).toLowerCase().includes(q))&&(!c||b.cat===c)&&(!s||b.status===s)&&(!f||(b.format||[]).includes(f)));
  document.getElementById('brand-count').textContent=list.length+' แบรนด์';
  document.getElementById('brand-grid').innerHTML=list.map(brandCard).join('')||'<div class="col-span-full text-center text-slate-500 py-10">ไม่พบ</div>';
}
['brand-search','brand-cat','brand-status','brand-format'].forEach(id=>document.getElementById(id).addEventListener('input',renderBrands));
renderBrands();

function renderLandlords(){
  const q=document.getElementById('ll-search').value.toLowerCase();
  const g=document.getElementById('ll-group').value;
  const list=LANDLORDS.filter(l=>(!q||(l.name+l.group+(l.keyMalls||[]).join(' ')+l.portfolio).toLowerCase().includes(q))&&(!g||l.group===g));
  document.getElementById('ll-count').textContent=list.length+' เครือ';
  document.getElementById('ll-grid').innerHTML=list.map(landlordCard).join('')||'<div class="col-span-full text-center text-slate-500 py-10">ไม่พบ</div>';
}
['ll-search','ll-group','ll-region'].forEach(id=>document.getElementById(id).addEventListener('input',renderLandlords));
renderLandlords();

let map,layerProp,layerMalls,layerBrands,layerLand,measureLayer,measurePoints=[];
function initMap(){
  map=L.map('map').setView([13.7563,100.5018],11);
  L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png',{attribution:'© OpenStreetMap',maxZoom:19}).addTo(map);
  layerProp=L.layerGroup();
  PROPERTIES.forEach(p=>{
    if(!p.lat)return;
    const icon=L.divIcon({className:'',html:'<div style="background:#2563EB;color:#fff;padding:3px 8px;border-radius:9999px;font-size:11px;font-weight:700;box-shadow:0 2px 6px rgba(0,0,0,.25);white-space:nowrap">฿'+(p.rent?Math.round(p.rent/1000)+'k':p.type)+'</div>',iconSize:[60,20],iconAnchor:[30,10]});
    const m=L.marker([p.lat,p.lng],{icon}).bindPopup('<div style="min-width:200px"><strong>'+p.title+'</strong><br/>'+p.mall+' · '+p.district+'<br/><span style="color:#2563EB;font-weight:700">฿'+fmt(p.rent)+'/เดือน · '+fmt(p.size)+' ตร.ม.</span><br/><a href="javascript:void(0)" onclick="openProperty(\''+p.id+'\')" style="color:#2563EB;text-decoration:underline">ดูรายละเอียด →</a></div>');
    layerProp.addLayer(m);
  });
  layerProp.addTo(map);
  layerMalls=L.layerGroup();
  Object.entries(MALL_LOCATIONS).forEach(([code,d])=>{
    const icon=L.divIcon({className:'',html:'<div style="background:#7c3aed;color:#fff;width:20px;height:20px;border-radius:50%;border:2px solid #fff;box-shadow:0 2px 6px rgba(0,0,0,.3);display:flex;align-items:center;justify-content:center;font-size:11px">🏬</div>',iconSize:[24,24],iconAnchor:[12,12]});
    L.marker([d.lat,d.lng],{icon}).bindPopup('<strong>'+d.name+'</strong>').addTo(layerMalls);
  });
  layerMalls.addTo(map);
  layerBrands=L.layerGroup();
  layerLand=L.layerGroup();
  [...LAND_PLOTS,...PROPERTIES.filter(p=>p.type==='land')].forEach(l=>{
    if(!l.lat)return;
    const icon=L.divIcon({className:'',html:'<div style="background:#84cc16;color:#fff;width:24px;height:24px;border-radius:6px;border:2px solid #fff;box-shadow:0 2px 6px rgba(0,0,0,.3);display:flex;align-items:center;justify-content:center;font-size:11px">🟫</div>',iconSize:[28,28],iconAnchor:[14,14]});
    L.marker([l.lat,l.lng],{icon}).bindPopup('<strong>'+(l.title||l.name||'ที่ดิน')+'</strong><br/>'+(l.area||fmt(l.size||0)+' ตร.ม.')+'<br/>'+(l.price||(l.rent?'฿'+fmt(l.rent):'-'))).addTo(layerLand);
  });
  const sel=document.getElementById('map-brand-select');
  const brands=[...new Set(BRAND_STORES.map(s=>s.brand))].sort();
  sel.innerHTML=brands.map(b=>'<option value="'+b+'">'+b+'</option>').join('');
  document.getElementById('layer-properties').addEventListener('change',e=>{e.target.checked?layerProp.addTo(map):map.removeLayer(layerProp)});
  document.getElementById('layer-malls').addEventListener('change',e=>{e.target.checked?layerMalls.addTo(map):map.removeLayer(layerMalls)});
  document.getElementById('layer-brand-stores').addEventListener('change',e=>{e.target.checked?refreshBrandLayer():map.removeLayer(layerBrands)});
  document.getElementById('layer-land').addEventListener('change',e=>{e.target.checked?layerLand.addTo(map):map.removeLayer(layerLand)});
  document.getElementById('map-brand-search').addEventListener('input',e=>{
    const q=e.target.value.toLowerCase();
    Array.from(sel.options).forEach(o=>{o.style.display=o.value.toLowerCase().includes(q)?'':'none'});
  });
  sel.addEventListener('change',refreshBrandLayer);
  measureLayer=L.layerGroup().addTo(map);
  let measuring=false;
  document.getElementById('tool-measure').addEventListener('click',()=>{
    measuring=!measuring;measurePoints=[];
    document.getElementById('tool-measure').textContent=measuring?'📏 คลิก 2 จุดบนแผนที่...':'📏 วัดระยะห่าง (คลิก 2 จุด)';
  });
  document.getElementById('tool-clear').addEventListener('click',()=>{
    measureLayer.clearLayers();measurePoints=[];measuring=false;
    document.getElementById('tool-measure').textContent='📏 วัดระยะห่าง (คลิก 2 จุด)';
    document.getElementById('measure-result').classList.add('hidden');
  });
  map.on('click',e=>{
    if(!measuring)return;
    measurePoints.push(e.latlng);
    L.circleMarker(e.latlng,{radius:5,color:'#f59e0b',fillColor:'#f59e0b',fillOpacity:1}).addTo(measureLayer);
    if(measurePoints.length===2){
      const d=map.distance(measurePoints[0],measurePoints[1]);
      L.polyline(measurePoints,{color:'#f59e0b',weight:3,dashArray:'6 6'}).addTo(measureLayer);
      const res=document.getElementById('measure-result');
      res.classList.remove('hidden');
      res.textContent='📏 ระยะห่าง '+(d<1000?Math.round(d)+' เมตร':(d/1000).toFixed(2)+' กม.');
      measuring=false;measurePoints=[];
      document.getElementById('tool-measure').textContent='📏 วัดระยะห่าง (คลิก 2 จุด)';
    }
  });
  document.getElementById('tool-recenter').addEventListener('click',()=>map.setView([13.7563,100.5018],6));
}
function refreshBrandLayer(){
  if(!document.getElementById('layer-brand-stores').checked){map.removeLayer(layerBrands);return}
  layerBrands.clearLayers();
  const sel=document.getElementById('map-brand-select');
  const picked=Array.from(sel.selectedOptions).map(o=>o.value);
  const colors=['#ef4444','#3b82f6','#10b981','#f59e0b','#a855f7','#ec4899','#06b6d4','#84cc16','#f97316'];
  const list=picked.length?BRAND_STORES.filter(s=>picked.includes(s.brand)):BRAND_STORES;
  const colorMap={};(picked.length?picked:[...new Set(list.map(s=>s.brand))]).forEach((b,i)=>colorMap[b]=colors[i%colors.length]);
  list.forEach(s=>{
    const c=colorMap[s.brand]||'#64748b';
    const icon=L.divIcon({className:'',html:'<div style="background:'+c+';color:#fff;width:14px;height:14px;border-radius:50%;border:2px solid #fff;box-shadow:0 1px 3px rgba(0,0,0,.4)"></div>',iconSize:[18,18],iconAnchor:[9,9]});
    L.marker([s.lat,s.lng],{icon}).bindPopup('<strong>'+s.brand+'</strong><br/>'+s.branch).addTo(layerBrands);
  });
  layerBrands.addTo(map);
}
function focusMap(lat,lng){map.setView([lat,lng],15)}
function showBrandOnMap(name){
  const sel=document.getElementById('map-brand-select');
  Array.from(sel.options).forEach(o=>o.selected=(o.value===name));
  document.getElementById('layer-brand-stores').checked=true;
  refreshBrandLayer();
}
initMap();

const PITCHES={};
PITCHES.brand='<div class="space-y-5"><div><h3 class="text-xl font-bold mb-2">พิชชิ่งกับแบรนด์ผู้เช่า</h3><p class="text-sm text-slate-600">เปลี่ยนทีม Site Selection ให้ทำงานเร็วขึ้น 3-5 เท่า — รวมพื้นที่+Mall data+competitor map+Deal Calculator</p></div><div class="grid md:grid-cols-3 gap-3"><div class="bg-blue-50 rounded-xl p-4"><div class="text-2xl font-bold text-blue-700">3-5x</div><div class="text-xs text-slate-600 mt-1">เร็วกว่าการหาเอง</div></div><div class="bg-emerald-50 rounded-xl p-4"><div class="text-2xl font-bold text-emerald-700">-30%</div><div class="text-xs text-slate-600 mt-1">ลด CAPEX ผิดที่</div></div><div class="bg-purple-50 rounded-xl p-4"><div class="text-2xl font-bold text-purple-700">'+PROPERTIES.length+'+</div><div class="text-xs text-slate-600 mt-1">Spaces ใน database</div></div></div><div><h4 class="font-bold mb-2">Talking Points</h4><ul class="text-sm space-y-2 list-disc pl-5 text-slate-700"><li><strong>เทียบ side-by-side</strong> — ค่าเช่า · CAM · 3+3 · Fit-out · Handover · Renovation timeline 3-6 ปี</li><li><strong>Mall mix intelligence</strong> — รู้คู่แข่ง occupancy traffic zoning</li><li><strong>Competitor map</strong> — เห็นสาขาคู่แข่ง+ตัวเองในรัศมีก่อนยื่นขอ approve</li><li><strong>Deal Calculator</strong> — คำนวณ TCO 6 ปี + Breakeven วันเดียว</li></ul></div></div>';
PITCHES.landlord='<div class="space-y-5"><div><h3 class="text-xl font-bold mb-2">พิชชิ่งกับห้าง</h3><p class="text-sm text-slate-600">เปลี่ยนพื้นที่ว่างเป็นรายได้เร็วขึ้น — RSL ทำ matchmaking</p></div><div class="grid md:grid-cols-3 gap-3"><div class="bg-blue-50 rounded-xl p-4"><div class="text-2xl font-bold text-blue-700">'+BRANDS.filter(b=>b.status==="active").length+'+</div><div class="text-xs text-slate-600 mt-1">แบรนด์ Active Scouting</div></div><div class="bg-emerald-50 rounded-xl p-4"><div class="text-2xl font-bold text-emerald-700">-50%</div><div class="text-xs text-slate-600 mt-1">ลด Vacancy time</div></div><div class="bg-purple-50 rounded-xl p-4"><div class="text-2xl font-bold text-purple-700">AI</div><div class="text-xs text-slate-600 mt-1">Match Scoring</div></div></div><div><h4 class="font-bold mb-2">Talking Points</h4><ul class="text-sm space-y-2 list-disc pl-5 text-slate-700"><li>List พื้นที่ว่างฟรี · เข้าถึง verified brand decision-maker</li><li>Matchmaking AI · จับคู่ unit↔brand</li><li>Mall Intelligence Benchmark</li><li>Renovation broadcast · ลด churn</li><li>ลด lead time 4-9 เดือน → 2-4 เดือน</li></ul></div></div>';
PITCHES.investor='<div class="space-y-5"><div><h3 class="text-xl font-bold mb-2">พิชชิ่งกับนักลงทุน</h3><p class="text-sm text-slate-600">Retail Space Leasing Marketplace + Intelligence · ตลาด ~฿3T/ปี</p></div><div class="grid md:grid-cols-4 gap-3"><div class="bg-blue-50 rounded-xl p-4"><div class="text-xs text-slate-600">TAM</div><div class="text-xl font-bold text-blue-700">฿3T</div></div><div class="bg-emerald-50 rounded-xl p-4"><div class="text-xs text-slate-600">SAM</div><div class="text-xl font-bold text-emerald-700">฿8B</div></div><div class="bg-purple-50 rounded-xl p-4"><div class="text-xs text-slate-600">SOM Yr3</div><div class="text-xl font-bold text-purple-700">฿240M</div></div><div class="bg-amber-50 rounded-xl p-4"><div class="text-xs text-slate-600">Mall GLA</div><div class="text-xl font-bold text-amber-700">20M sqm</div></div></div><div><h4 class="font-bold mb-2">Problem</h4><ul class="text-sm space-y-1 list-disc pl-5 text-slate-700"><li>แบรนด์ใช้เวลา 3-6 เดือนในการหา site</li><li>ห้าง vacancy เฉลี่ย 8-15%</li><li>นายหน้าตลาด retail แตกกระจาย fee ไม่โปร่งใส</li></ul></div><div><h4 class="font-bold mb-2">Business Model</h4><ul class="text-sm space-y-1 list-disc pl-5 text-slate-700"><li>Subscription (Brand &amp; Landlord) recurring</li><li>Success fee 0.5-1 เดือนค่าเช่า</li><li>Premium consulting + data product</li></ul></div><div><h4 class="font-bold mb-2">Ask</h4><p class="text-sm text-slate-700">Seed ฿25-50M สำหรับ 18 เดือน — ทีม 10 คน — Target Series A ที่ ARR ฿80M+</p></div></div>';
function renderPitch(k){
  document.getElementById('pitch-content').innerHTML=PITCHES[k];
  document.querySelectorAll('.pitch-btn').forEach(b=>{
    if(b.dataset.pitch===k){b.classList.add('bg-blue-600','text-white');b.classList.remove('bg-slate-100','text-slate-700')}
    else{b.classList.remove('bg-blue-600','text-white');b.classList.add('bg-slate-100','text-slate-700')}
  });
}
document.querySelectorAll('.pitch-btn').forEach(b=>b.addEventListener('click',()=>renderPitch(b.dataset.pitch)));
renderPitch('brand');

function parseBudget(s){if(!s)return null;const m=s.replace(/,/g,'').match(/(\d+)\s*-\s*(\d+)/);return m?{min:+m[1],max:+m[2]}:null}
function parseSize(s){if(!s)return null;const m=s.replace(/,/g,'').match(/(\d+)\s*-\s*(\d+)/);return m?{min:+m[1],max:+m[2]}:null}
function scoreMatch(brand,prop){
  let breakdown={size:0,rent:0,format:0,location:0,competition:0};
  const bs=parseSize(brand.size);
  if(bs&&prop.size){
    if(prop.size>=bs.min&&prop.size<=bs.max)breakdown.size=30;
    else{const dist=prop.size<bs.min?bs.min-prop.size:prop.size-bs.max;const tol=bs.max*0.3;breakdown.size=Math.max(0,30-(dist/tol)*30)}
  }else breakdown.size=15;
  const bb=parseBudget(brand.rentBudget);const ppm=prop.size?prop.rent/prop.size:0;
  if(bb&&ppm){
    if(ppm>=bb.min&&ppm<=bb.max)breakdown.rent=25;
    else if(ppm<bb.min)breakdown.rent=22;
    else{const over=(ppm-bb.max)/bb.max;breakdown.rent=Math.max(0,25-over*40)}
  }else breakdown.rent=12;
  const fmt2=(brand.format||[]).map(f=>f.toLowerCase());
  const propTypeMap={mall:['inline','flagship','anchor','kiosk'],kiosk:['kiosk'],standalone:['flagship','drive-thru','standalone'],community:['inline','anchor'],land:['standalone','flagship']};
  const pf=propTypeMap[prop.type]||[];
  breakdown.format=fmt2.some(f=>pf.some(p=>f.includes(p)||p.includes(f)))?15:5;
  const ex=prop.extras||{};const traffic=parseInt((ex.traffic||'').replace(/[^\d]/g,''))||0;
  if(traffic>=80000)breakdown.location=15;else if(traffic>=40000)breakdown.location=12;else if(traffic>=20000)breakdown.location=8;else breakdown.location=5;
  const sameCat=BRANDS.filter(b=>b.cat===brand.cat&&b.id!==brand.id).map(b=>b.id);
  const nearbyComp=BRAND_STORES.filter(s=>{if(!sameCat.includes(s.brandId))return false;const d=Math.hypot(s.lat-prop.lat,s.lng-prop.lng);return d<0.01}).length;
  if(nearbyComp===0)breakdown.competition=15;else if(nearbyComp<=2)breakdown.competition=12;else if(nearbyComp<=5)breakdown.competition=8;else breakdown.competition=5;
  return {total:Math.round(breakdown.size+breakdown.rent+breakdown.format+breakdown.location+breakdown.competition),breakdown,nearbyComp};
}
let matchMode='b2u';
function renderMatchControls(){
  const c=document.getElementById('match-controls');
  if(matchMode==='b2u'){
    const opts=BRANDS.map(b=>'<option value="'+b.id+'">'+b.name+' ('+b.cat+')</option>').join('');
    c.innerHTML='<label class="text-sm font-semibold">เลือกแบรนด์:</label><select id="match-pick" class="border border-slate-200 rounded-lg px-3 py-2 text-sm ml-2 min-w-[260px]">'+opts+'</select>';
  }else{
    const opts=PROPERTIES.filter(p=>p.type!=='land').map(p=>'<option value="'+p.id+'">'+p.title+' ('+fmt(p.size)+' ตร.ม., ฿'+fmt(p.rent)+')</option>').join('');
    c.innerHTML='<label class="text-sm font-semibold">เลือกยูนิต:</label><select id="match-pick" class="border border-slate-200 rounded-lg px-3 py-2 text-sm ml-2 min-w-[320px]">'+opts+'</select>';
  }
  document.getElementById('match-pick').addEventListener('change',renderMatchResults);
  renderMatchResults();
}
function scoreBar(label,val,max){
  const pct=(val/max)*100;const cls=pct>=70?'bg-emerald-500':pct>=40?'bg-amber-500':'bg-red-400';
  return '<div class="text-[11px]"><div class="flex justify-between mb-0.5"><span>'+label+'</span><span class="font-bold">'+val.toFixed(0)+'/'+max+'</span></div><div class="w-full bg-slate-100 rounded-full h-1.5"><div class="'+cls+' h-1.5 rounded-full" style="width:'+pct+'%"></div></div></div>';
}
function renderMatchResults(){
  const pick=document.getElementById('match-pick');if(!pick)return;
  const results=document.getElementById('match-results');
  if(matchMode==='b2u'){
    const b=BRANDS.find(x=>x.id===pick.value);if(!b){results.innerHTML='';return}
    const scored=PROPERTIES.filter(p=>p.type!=='land').map(p=>({p,s:scoreMatch(b,p)})).sort((a,b)=>b.s.total-a.s.total).slice(0,12);
    let html='<div class="bg-white rounded-2xl border border-slate-200 p-4 mb-3"><div class="flex items-center gap-3">'+brandLogo(b.id,56)+'<div><div class="text-xs text-slate-500">'+b.sub+'</div><div class="text-xl font-bold">'+b.name+'</div><div class="text-xs text-slate-500 mt-1">ขนาด '+(b.size||'-')+' · งบ '+(b.rentBudget||'-')+'</div></div></div></div><div class="grid md:grid-cols-2 gap-3">';
    scored.forEach(({p,s})=>{
      html+='<div class="bg-white rounded-xl border border-slate-200 p-4"><div class="flex items-start justify-between gap-2"><div class="min-w-0"><div class="font-semibold text-sm truncate">'+p.title+'</div><div class="text-xs text-slate-500 mt-0.5">'+p.mall+' · '+p.district+'</div></div><div class="text-2xl font-extrabold '+(s.total>=70?'text-emerald-600':s.total>=50?'text-amber-600':'text-red-500')+'">'+s.total+'</div></div><div class="grid grid-cols-2 gap-2 mt-3">'+scoreBar('Size fit',s.breakdown.size,30)+scoreBar('Rent fit',s.breakdown.rent,25)+scoreBar('Format',s.breakdown.format,15)+scoreBar('Location',s.breakdown.location,15)+scoreBar('Competition',s.breakdown.competition,15)+'</div><div class="text-[11px] text-slate-500 mt-2">คู่แข่งหมวด '+b.cat+' รัศมี ~1กม.: '+s.nearbyComp+' ราย</div><button onclick="openProperty(\''+p.id+'\')" class="mt-3 text-xs text-blue-600 hover:underline">ดูรายละเอียดยูนิต →</button></div>';
    });
    results.innerHTML=html+'</div>';
  }else{
    const p=PROPERTIES.find(x=>x.id===pick.value);if(!p){results.innerHTML='';return}
    const scored=BRANDS.map(b=>({b,s:scoreMatch(b,p)})).sort((a,b)=>b.s.total-a.s.total).slice(0,12);
    let html='<div class="bg-white rounded-2xl border border-slate-200 p-4 mb-3"><div class="text-xs text-slate-500">'+p.mall+' · '+p.district+'</div><div class="text-xl font-bold">'+p.title+'</div><div class="text-xs text-slate-500 mt-1">ขนาด '+fmt(p.size)+' ตร.ม. · ค่าเช่า ฿'+fmt(p.rent)+'/เดือน (฿'+Math.round(p.rent/p.size).toLocaleString()+'/ตร.ม.)</div></div><div class="grid md:grid-cols-2 gap-3">';
    scored.forEach(({b,s})=>{
      html+='<div class="bg-white rounded-xl border border-slate-200 p-4"><div class="flex items-start justify-between gap-2"><div class="flex items-center gap-3 min-w-0">'+brandLogo(b.id,40)+'<div class="min-w-0"><div class="font-semibold text-sm truncate">'+b.name+'</div><div class="text-xs text-slate-500 mt-0.5 truncate">'+b.cat+' · '+b.sub+'</div></div></div><div class="text-2xl font-extrabold '+(s.total>=70?'text-emerald-600':s.total>=50?'text-amber-600':'text-red-500')+'">'+s.total+'</div></div><div class="grid grid-cols-2 gap-2 mt-3">'+scoreBar('Size fit',s.breakdown.size,30)+scoreBar('Rent fit',s.breakdown.rent,25)+scoreBar('Format',s.breakdown.format,15)+scoreBar('Location',s.breakdown.location,15)+scoreBar('Competition',s.breakdown.competition,15)+'</div><button onclick="openBrand(\''+b.id+'\')" class="mt-3 text-xs text-blue-600 hover:underline">ดูโปรไฟล์แบรนด์ →</button></div>';
    });
    results.innerHTML=html+'</div>';
  }
}
document.querySelectorAll('.match-mode-btn').forEach(btn=>btn.addEventListener('click',()=>{
  matchMode=btn.dataset.matchMode;
  document.querySelectorAll('.match-mode-btn').forEach(b=>{
    if(b.dataset.matchMode===matchMode){b.classList.add('bg-blue-600','text-white');b.classList.remove('bg-slate-100','text-slate-700')}
    else{b.classList.remove('bg-blue-600','text-white');b.classList.add('bg-slate-100','text-slate-700')}
  });
  renderMatchControls();
}));
renderMatchControls();

function toCSV(rows){
  if(!rows.length)return '';
  const keys=[...new Set(rows.flatMap(r=>Object.keys(r)))];
  const esc=v=>{if(v===null||v===undefined)return '';if(typeof v==='object')v=JSON.stringify(v);const s=String(v).replace(/"/g,'""');return /[",\n]/.test(s)?'"'+s+'"':s};
  return [keys.join(','),...rows.map(r=>keys.map(k=>esc(r[k])).join(','))].join('\n');
}
function download(filename,content,mime){
  mime=mime||'text/plain';
  const blob=new Blob([content],{type:mime+';charset=utf-8'});
  const a=document.createElement('a');a.href=URL.createObjectURL(blob);a.download=filename;document.body.appendChild(a);a.click();
  setTimeout(()=>{URL.revokeObjectURL(a.href);a.remove()},100);
}
window.exportData=function(what,fmt2){
  let rows,name;
  if(what==='properties'){rows=PROPERTIES;name='rsl_properties'}
  else if(what==='brands'){rows=BRANDS;name='rsl_brands'}
  else if(what==='landlords'){rows=LANDLORDS;name='rsl_landlords'}
  else if(what==='stores'){rows=BRAND_STORES;name='rsl_brand_stores'}
  else if(what==='malls'){rows=Object.entries(MALL_LOCATIONS).map(([id,v])=>({id,...v}));name='rsl_malls'}
  else if(what==='land'){rows=LAND_PLOTS;name='rsl_land'}
  else if(what==='all'){
    const all={properties:PROPERTIES,brands:BRANDS,landlords:LANDLORDS,brandStores:BRAND_STORES,brandDomains:BRAND_DOMAINS,brandPresence:BRAND_PRESENCE,mallLocations:MALL_LOCATIONS,landPlots:LAND_PLOTS};
    download('rsl_dataset.json',JSON.stringify(all,null,2),'application/json');return;
  }
  if(fmt2==='csv')download(name+'.csv',toCSV(rows),'text/csv');
  else download(name+'.json',JSON.stringify(rows,null,2),'application/json');
};

function $i(id){return document.getElementById(id)}
let CALC_RESULT=null;
function setupCalc(){
  const sel=$i('calc-prop');
  sel.innerHTML='<option value="">— ใส่ค่ามือเอง —</option>'+PROPERTIES.filter(p=>p.type!=='land').map(p=>'<option value="'+p.id+'">'+p.title+' ('+fmt(p.size)+'ตร.ม. ฿'+fmt(p.rent)+')</option>').join('');
  sel.addEventListener('change',()=>{
    const p=PROPERTIES.find(x=>x.id===sel.value);if(!p)return;
    $i('ci-size').value=p.size;$i('ci-rent').value=p.rent;
    $i('ci-service').value=p.service||0;$i('ci-cam').value=p.cam||0;
    const dm=(p.deposit||'').match(/(\d+)/);if(dm)$i('ci-deposit').value=+dm[1];
    const em=(p.escalation||'').match(/(\d+)/);if(em)$i('ci-esc').value=+em[1];
    const fm=(p.fitout||'').match(/(\d+)/);if(fm)$i('ci-fitout').value=Math.ceil(+fm[1]/30);
    runCalc();
  });
  $i('calc-run').addEventListener('click',runCalc);
  $i('calc-export').addEventListener('click',exportCalc);
  ['ci-size','ci-rent','ci-service','ci-cam','ci-deposit','ci-esc','ci-term','ci-fitout','ci-capex','ci-rev','ci-cogs','ci-payroll','ci-misc','ci-rg'].forEach(id=>{
    $i(id).addEventListener('input',()=>{clearTimeout(window._ct);window._ct=setTimeout(runCalc,250)});
  });
  runCalc();
}
function runCalc(){
  const size=+$i('ci-size').value||0,rent=+$i('ci-rent').value||0;
  const service=+$i('ci-service').value||0,cam=+$i('ci-cam').value||0;
  const dep=+$i('ci-deposit').value||0,esc=(+$i('ci-esc').value||0)/100;
  const term=+$i('ci-term').value||1,fitout=+$i('ci-fitout').value||0;
  const capexPerSqm=+$i('ci-capex').value||0,rev0=+$i('ci-rev').value||0;
  const cogs=(+$i('ci-cogs').value||0)/100,payroll=+$i('ci-payroll').value||0;
  const misc=+$i('ci-misc').value||0,rg=(+$i('ci-rg').value||0)/100;
  const capex=size*capexPerSqm,depAmt=dep*rent;
  const years=[];let cumCash=-(capex+depAmt);let bMonth=null,month=0;
  for(let y=1;y<=term;y++){
    const r=rent*Math.pow(1+esc,y-1);
    const sv=service*Math.pow(1+esc,y-1);
    const cm=cam*Math.pow(1+esc,y-1);
    const rev=rev0*Math.pow(1+rg,y-1);
    const grossM=rev*(1-cogs);
    const monthsActive=y===1?12-fitout:12;
    const annualRent=(r+sv+cm)*monthsActive;
    const annualRev=rev*monthsActive;
    const annualGM=grossM*monthsActive;
    const opex=(payroll+misc)*monthsActive;
    const annualEbitda=annualGM-annualRent-opex;
    const prevCum=cumCash;
    cumCash+=annualEbitda;
    if(bMonth===null){
      const mEbitda=(grossM-r-sv-cm-payroll-misc);
      for(let m=1;m<=monthsActive;m++){
        if(prevCum+mEbitda*m>=0){bMonth=month+m;break}
      }
    }
    month+=monthsActive;
    years.push({y,rent:r*monthsActive,service:sv*monthsActive,cam:cm*monthsActive,occMonths:monthsActive,rev:annualRev,gm:annualGM,opex,ebitda:annualEbitda,cumCash:cumCash,annualRent});
  }
  CALC_RESULT={years,capex,depAmt,bMonth,term};
  renderCalc();
}
function renderCalc(){
  if(!CALC_RESULT)return;
  const {years,capex,depAmt,bMonth,term}=CALC_RESULT;
  const totalRev=years.reduce((a,b)=>a+b.rev,0);
  const totalRent=years.reduce((a,b)=>a+b.annualRent,0);
  const totalEbitda=years.reduce((a,b)=>a+b.ebitda,0);
  const finalCash=years[years.length-1].cumCash;
  const roi=capex>0?((finalCash+depAmt)/capex*100):0;
  let html='<div class="grid sm:grid-cols-2 lg:grid-cols-4 gap-3">';
  html+='<div class="bg-blue-50 rounded-xl p-4"><div class="text-xs text-blue-700 font-semibold">Total CAPEX+Deposit</div><div class="text-xl font-extrabold text-blue-700">฿'+fmt(Math.round(capex+depAmt))+'</div><div class="text-[10px] text-slate-500 mt-1">CAPEX ฿'+fmt(Math.round(capex))+' + ประกัน ฿'+fmt(Math.round(depAmt))+'</div></div>';
  html+='<div class="bg-emerald-50 rounded-xl p-4"><div class="text-xs text-emerald-700 font-semibold">Total Revenue '+term+'Y</div><div class="text-xl font-extrabold text-emerald-700">฿'+fmt(Math.round(totalRev))+'</div></div>';
  html+='<div class="bg-purple-50 rounded-xl p-4"><div class="text-xs text-purple-700 font-semibold">Total Rent+Svc+CAM</div><div class="text-xl font-extrabold text-purple-700">฿'+fmt(Math.round(totalRent))+'</div><div class="text-[10px] text-slate-500 mt-1">% ของ revenue: '+(totalRev?(totalRent/totalRev*100).toFixed(1):'-')+'%</div></div>';
  html+='<div class="bg-amber-50 rounded-xl p-4"><div class="text-xs text-amber-700 font-semibold">Total EBITDA '+term+'Y</div><div class="text-xl font-extrabold '+(totalEbitda>=0?'text-amber-700':'text-red-600')+'">฿'+fmt(Math.round(totalEbitda))+'</div></div>';
  html+='</div><div class="grid sm:grid-cols-3 gap-3 mt-3">';
  html+='<div class="bg-white border rounded-xl p-4"><div class="text-xs text-slate-500">Breakeven (เดือน)</div><div class="text-2xl font-extrabold '+(bMonth?'text-emerald-600':'text-red-500')+'">'+(bMonth?bMonth+' เดือน':'ไม่ Breakeven ใน '+term+' ปี')+'</div></div>';
  html+='<div class="bg-white border rounded-xl p-4"><div class="text-xs text-slate-500">ROI (cumulative / CAPEX)</div><div class="text-2xl font-extrabold '+(roi>=0?'text-emerald-600':'text-red-500')+'">'+roi.toFixed(0)+'%</div></div>';
  html+='<div class="bg-white border rounded-xl p-4"><div class="text-xs text-slate-500">EBITDA Margin (avg)</div><div class="text-2xl font-extrabold">'+(totalRev?(totalEbitda/totalRev*100).toFixed(1):'-')+'%</div></div>';
  html+='</div><div class="bg-white border border-slate-200 rounded-xl overflow-hidden mt-3"><div class="px-4 py-3 border-b text-sm font-bold">Year-by-Year P&amp;L</div><div class="overflow-x-auto"><table class="w-full text-xs"><thead class="bg-slate-50 text-slate-600"><tr><th class="text-left px-3 py-2">Year</th><th class="text-right px-3 py-2">Months</th><th class="text-right px-3 py-2">Revenue</th><th class="text-right px-3 py-2">Gross Margin</th><th class="text-right px-3 py-2">Rent+Svc+CAM</th><th class="text-right px-3 py-2">Opex</th><th class="text-right px-3 py-2">EBITDA</th><th class="text-right px-3 py-2">Cum.Cash</th></tr></thead><tbody>';
  years.forEach(y=>{
    html+='<tr class="border-t"><td class="px-3 py-2 font-semibold">Y'+y.y+'</td><td class="text-right px-3 py-2">'+y.occMonths+'</td><td class="text-right px-3 py-2">฿'+fmt(Math.round(y.rev))+'</td><td class="text-right px-3 py-2">฿'+fmt(Math.round(y.gm))+'</td><td class="text-right px-3 py-2 text-red-600">฿'+fmt(Math.round(y.annualRent))+'</td><td class="text-right px-3 py-2 text-red-600">฿'+fmt(Math.round(y.opex))+'</td><td class="text-right px-3 py-2 '+(y.ebitda>=0?'text-emerald-600':'text-red-600')+' font-bold">฿'+fmt(Math.round(y.ebitda))+'</td><td class="text-right px-3 py-2 '+(y.cumCash>=0?'text-emerald-700':'text-red-700')+' font-bold">฿'+fmt(Math.round(y.cumCash))+'</td></tr>';
  });
  html+='</tbody></table></div></div><div class="bg-slate-50 rounded-xl p-4 text-xs text-slate-600 mt-3"><strong>หมายเหตุ:</strong> ตัวเลขเป็นการประมาณการ — ไม่ใช่งบประมาณทางบัญชี ปรับด้วย opex แฝง (R&amp;M, marketing, depreciation), ภาษี และความผันผวนรายเดือน</div>';
  $i('calc-out').innerHTML=html;
}
function exportCalc(){
  if(!CALC_RESULT)return;
  const rows=[['Year','Months','Revenue','GM','Rent+Svc+CAM','Opex','EBITDA','CumCash']];
  CALC_RESULT.years.forEach(y=>rows.push([y.y,y.occMonths,Math.round(y.rev),Math.round(y.gm),Math.round(y.annualRent),Math.round(y.opex),Math.round(y.ebitda),Math.round(y.cumCash)]));
  rows.push(['','','','','','','Breakeven',CALC_RESULT.bMonth||'N/A']);
  download('rsl_dealcalc.csv',rows.map(r=>r.join(',')).join('\n'),'text/csv');
}
setupCalc();

</script>
</body>
</html>
