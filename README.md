<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>مولد مفاتيح التفعيل وإدارة العملاء - KEY GENERATOR</title>
<style>
*, *::before, *::after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  border: none !important;
  outline: none !important;
}

:root {
  --bg: #030607;
  --panel: #081012;
  --panel2: #0d1719;
  --panel3: #111d20;
  --lime: #a8ff00;
  --lime2: #c4ff52;
  --text: #f4f7f5;
  --muted: #889997;
  --danger: #ff5b67;
  --blue: #55b8ff;
  --shadow: 0 15px 35px rgba(0,0,0,0.6);
  --border-glass: rgba(168, 255, 0, 0.12);
}

body {
  background: radial-gradient(circle at 15% 10%, rgba(168,255,0,0.07), transparent 30%), var(--bg);
  color: var(--text);
  min-height: 100vh;
  padding: 15px;
  display: flex;
  justify-content: center;
  align-items: flex-start;
}

.app-container {
  width: 100%;
  max-width: 500px;
  background: var(--panel);
  border-radius: 22px;
  box-shadow: var(--shadow);
  display: flex;
  flex-direction: column;
  overflow: hidden;
  position: relative;
  padding: 18px;
  gap: 15px;
  border: 1px solid var(--border-glass) !important;
}

.header {
  background: var(--panel2);
  padding: 14px 16px;
  border-radius: 14px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  border: 1px solid rgba(255,255,255,0.03) !important;
}

.brand {
  display: flex;
  align-items: center;
  gap: 12px;
}

.brand-logo {
  width: 40px;
  height: 40px;
  background: linear-gradient(135deg, var(--lime), #76b300);
  color: #000;
  border-radius: 12px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: 900;
  font-size: 18px;
  box-shadow: 0 5px 15px rgba(168,255,0,0.2);
}

.brand-text h1 {
  font-size: 15px;
  color: var(--lime);
  font-weight: 900;
  letter-spacing: 0.5px;
}

.brand-text span {
  font-size: 9.5px;
  color: var(--muted);
}

.action-bar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: var(--panel2);
  padding: 12px 15px;
  border-radius: 12px;
  border: 1px solid rgba(255,255,255,0.03) !important;
}

.btn-open-form {
  background: var(--lime);
  color: #000;
  padding: 8px 14px;
  border-radius: 9px;
  font-size: 11px;
  font-weight: 900;
  cursor: pointer;
  transition: 0.2s;
  box-shadow: 0 4px 12px rgba(168,255,0,0.2);
}

.btn-open-form:hover {
  opacity: 0.9;
  transform: translateY(-1px);
}

.stats-info {
  font-size: 11px;
  color: var(--muted);
  font-weight: 600;
}

.stats-info span {
  color: var(--lime);
  font-weight: bold;
}

.add-modal-container {
  background: var(--panel2);
  padding: 15px;
  border-radius: 14px;
  display: none;
  flex-direction: column;
  gap: 12px;
  border: 1px solid var(--border-glass) !important;
  animation: fadeIn 0.3s ease;
}

.add-modal-container.active {
  display: flex;
}

@keyframes fadeIn {
  from { opacity: 0; transform: translateY(-8px); }
  to { opacity: 1; transform: translateY(0); }
}

.modal-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-size: 12px;
  color: var(--lime);
  font-weight: bold;
  padding-bottom: 8px;
  border-bottom: 1px solid rgba(255,255,255,0.04);
}

.btn-close-modal {
  background: rgba(255,91,103,0.15);
  color: var(--danger);
  padding: 4px 8px;
  border-radius: 6px;
  font-size: 10px;
  cursor: pointer;
}

.form-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 10px;
}

.form-group {
  display: flex;
  flex-direction: column;
  gap: 5px;
}

.form-group.full {
  grid-column: span 2;
}

.form-group label {
  font-size: 10.5px;
  color: var(--lime2);
  font-weight: 600;
}

.form-input {
  background: var(--panel);
  color: var(--text);
  padding: 10px 12px;
  border-radius: 10px;
  font-size: 11.5px;
  width: 100%;
  border: 1px solid rgba(255,255,255,0.04) !important;
  transition: 0.2s;
}

.form-input:focus {
  border-color: rgba(168,255,0,0.4) !important;
  background: var(--panel3);
}

select.form-input {
  cursor: pointer;
}

.btn-generate {
  background: linear-gradient(135deg, var(--lime), #91e600);
  color: #000;
  padding: 12px;
  border-radius: 10px;
  font-weight: 900;
  font-size: 12px;
  cursor: pointer;
  text-align: center;
  transition: 0.2s;
  grid-column: span 2;
  margin-top: 5px;
  box-shadow: 0 5px 20px rgba(168,255,0,0.25);
}

.btn-generate:hover {
  opacity: 0.95;
}

.output-box {
  background: var(--panel);
  padding: 12px;
  border-radius: 10px;
  display: none;
  flex-direction: column;
  gap: 6px;
  margin-top: 8px;
  border: 1px solid rgba(255,255,255,0.03) !important;
}

.output-box.active {
  display: flex;
}

.key-display {
  background: var(--bg);
  color: var(--lime);
  padding: 10px;
  border-radius: 8px;
  font-family: monospace;
  font-size: 10.5px;
  word-break: break-all;
  text-align: left;
  direction: ltr;
}

.btn-copy {
  background: rgba(85,184,255,0.15);
  color: var(--blue);
  width: 100%;
  padding: 8px;
  border-radius: 8px;
  font-size: 10.5px;
  font-weight: bold;
  cursor: pointer;
  text-align: center;
}

.history-section {
  display: flex;
  flex-direction: column;
  gap: 10px;
  background: var(--panel2);
  padding: 14px;
  border-radius: 14px;
  border: 1px solid rgba(255,255,255,0.03) !important;
}

.history-header-title {
  font-size: 11.5px;
  color: var(--lime);
  font-weight: bold;
  margin-bottom: 2px;
}

.search-box {
  width: 100%;
  background: var(--panel);
  padding: 10px 14px;
  border-radius: 10px;
  color: var(--text);
  font-size: 11px;
  border: 1px solid rgba(255,255,255,0.04) !important;
}

.history-list {
  display: flex;
  flex-direction: column;
  gap: 8px;
  max-height: 350px;
  overflow-y: auto;
  padding-right: 2px;
}

.history-item {
  background: var(--panel);
  padding: 11px;
  border-radius: 10px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  border: 1px solid rgba(255,255,255,0.03) !important;
  transition: 0.2s;
}

.history-item:hover {
  border-color: rgba(168,255,0,0.2) !important;
}

.history-info h4 {
  font-size: 11.5px;
  color: var(--text);
  font-weight: 700;
}

.history-info p {
  font-size: 9.5px;
  color: var(--muted);
  margin-top: 2px;
}

.history-actions {
  display: flex;
  gap: 5px;
}

.btn-sm {
  padding: 5px 9px;
  border-radius: 7px;
  font-size: 9.5px;
  font-weight: bold;
  cursor: pointer;
  transition: 0.2s;
}

.btn-sm-copy {
  background: rgba(85,184,255,0.15);
  color: var(--blue);
}

.btn-sm-del {
  background: rgba(255,91,103,0.15);
  color: var(--danger);
}

.toast {
  position: fixed;
  bottom: 25px;
  left: 50%;
  transform: translateX(-50%) translateY(60px);
  background: var(--panel3);
  color: var(--lime);
  padding: 10px 20px;
  border-radius: 12px;
  font-size: 11px;
  font-weight: bold;
  opacity: 0;
  transition: 0.3s cubic-bezier(0.4, 0, 0.2, 1);
  z-index: 2000;
  box-shadow: 0 10px 30px rgba(0,0,0,0.5);
  border: 1px solid var(--border-glass) !important;
}

.toast.show {
  transform: translateX(-50%) translateY(0);
  opacity: 1;
}
</style>
</head>
<body>

<div class="app-container">
  <header class="header">
    <div class="brand">
      <div class="brand-logo">🔑</div>
      <div class="brand-text">
        <h1>KEY GENERATOR</h1>
        <span>نظام إصدار وإدارة مفاتيح التفعيل الفاخر</span>
      </div>
    </div>
  </header>

  <div class="action-bar">
    <button class="btn-open-form" onclick="toggleAddForm()">➕ إضافة عميل جديد</button>
    <div class="stats-info">إجمالي العملاء: <span id="clientCount">0</span></div>
  </div>

  <div class="add-modal-container" id="addModalContainer">
    <div class="modal-header">
      <span>تعبئة بيانات العميل وتوليد مفتاح التفعيل</span>
      <button class="btn-close-modal" onclick="toggleAddForm()">✕ إغلاق</button>
    </div>

    <div class="form-grid">
      <div class="form-group full">
        <label>اسم المتجر / العميل (Brand Name) *</label>
        <input type="text" class="form-input" id="clientName" placeholder="مثال: SOFIANE SHOP">
      </div>

      <div class="form-group">
        <label>مدة صلاحية الحساب</label>
        <select class="form-input" id="clientDuration">
          <option value="30">شهر (30 يوم)</option>
          <option value="90">3 أشهر (90 يوم)</option>
          <option value="180">6 أشهر (180 يوم)</option>
          <option value="365" selected>سنة (365 يوم)</option>
          <option value="0">دائم (بدون انتهاء)</option>
        </select>
      </div>

      <div class="form-group">
        <label>مدون الحساب / المسؤول</label>
        <input type="text" class="form-input" id="clientAccountant" placeholder="مثال: Soufiane Admin">
      </div>

      <div class="form-group">
        <label>رقم الهاتف الأساسي</label>
        <input type="text" class="form-input" id="clientPhone" placeholder="06 66 22 70 60">
      </div>

      <div class="form-group">
        <label>رقم الواتساب</label>
        <input type="text" class="form-input" id="clientWhatsapp" placeholder="+212 6 30 47 34 98">
      </div>

      <div class="form-group">
        <label>البريد الإلكتروني (Gmail)</label>
        <input type="email" class="form-input" id="clientGmail" placeholder="client@gmail.com">
      </div>

      <div class="form-group full">
        <label>رابط اللوجو الخاص بالعميل (Image URL)</label>
        <input type="text" class="form-input" id="clientLogo" placeholder="https://domain.com/logo.jpg">
      </div>

      <div class="form-group">
        <label>اسم الإمضاء والخاتم</label>
        <input type="text" class="form-input" id="clientSign" placeholder="مثال: Soufiane">
      </div>

      <div class="form-group">
        <label>عنوان المحل / المتجر</label>
        <input type="text" class="form-input" id="clientAddress" placeholder="تطوان - حي المدرسي">
      </div>

      <button class="btn-generate" onclick="generateAndSaveKey()">⚡ إصدار وحفظ كود التفعيل</button>
    </div>

    <div class="output-box" id="outputBox">
      <label style="font-size:10px; color:var(--muted);">كود التفعيل المشفر المولد:</label>
      <div class="key-display" id="keyResult"></div>
      <button class="btn-copy" onclick="copyKey()">📋 نسخ الكود وتسليمه للعميل</button>
    </div>
  </div>

  <div class="history-section">
    <div class="history-header-title">📁 سجل العملاء المفعلين</div>
    <input type="text" class="search-box" id="searchBox" placeholder="🔍 ابحث باسم العميل أو مدون الحساب..." oninput="filterHistory()">
    <div class="history-list" id="historyList"></div>
  </div>
</div>

<div class="toast" id="toastMsg">تمت العملية بنجاح</div>

<script>
let clientsHistory = JSON.parse(localStorage.getItem("app_clients_history") || "[]");

document.addEventListener("DOMContentLoaded", () => {
  renderHistory();
});

function toggleAddForm() {
  const modal = document.getElementById("addModalContainer");
  modal.classList.toggle("active");
  if(modal.classList.contains("active")) {
    document.getElementById("clientName").focus();
  }
}

// دالة مشفرة آمنة تدعم الحروف العربية والرموز بدون أخطاء في الـ Base64
function safeBase64Encode(str) {
  return btoa(encodeURIComponent(str).replace(/%([0-9A-F]{2})/g, function(match, p1) {
    return String.fromCharCode('0x' + p1);
  }));
}

function generateAndSaveKey() {
  const name = document.getElementById("clientName").value.trim();
  const accountant = document.getElementById("clientAccountant").value.trim();
  const phone = document.getElementById("clientPhone").value.trim();
  const whatsapp = document.getElementById("clientWhatsapp").value.trim();
  const gmail = document.getElementById("clientGmail").value.trim();
  const logo = document.getElementById("clientLogo").value.trim();
  const sign = document.getElementById("clientSign").value.trim();
  const address = document.getElementById("clientAddress").value.trim();
  const duration = parseInt(document.getElementById("clientDuration").value);

  if(!name) {
    showToast("يرجى إدخال اسم العميل على الأقل!");
    return;
  }

  const createdAt = new Date().toISOString().split('T')[0];
  let expiresAt = "31/12/2030"; // الصيغة اليوم/الشهر/السنة التي يتوقعها التطبيق الرئيسي

  if (duration > 0) {
    const expDate = new Date();
    expDate.setDate(expDate.getDate() + duration);
    let day = String(expDate.getDate()).padStart(2, '0');
    let month = String(expDate.getMonth() + 1).padStart(2, '0');
    let year = expDate.getFullYear();
    expiresAt = `${day}/${month}/${year}`;
  } else if (duration === 0) {
    expiresAt = "31/12/2030";
  }

  // الهيكل المتوافق مع لوحة الإدارة (n, e, p, w, g, l, s, a)
  const payload = {
    n: name,
    e: expiresAt,
    p: phone || "06 00 00 00 00",
    w: whatsapp || "+212 6 00 00 00 00",
    g: gmail || "support@gmail.com",
    l: logo || "https://i.ibb.co/LXWzbssm/IMG-20261104-145706.jpg",
    s: sign || name.split(" ")[0],
    a: address || "المغرب"
  };

  const jsonStr = JSON.stringify(payload);
  const encodedKey = "KEY_" + safeBase64Encode(jsonStr);

  document.getElementById("keyResult").textContent = encodedKey;
  document.getElementById("outputBox").classList.add("active");

  const clientData = {
    id: Date.now(),
    name: name,
    accountant: accountant || "مسؤول النظام",
    key: encodedKey,
    createdAt: createdAt,
    expiresAt: expiresAt
  };

  clientsHistory.unshift(clientData);
  localStorage.setItem("app_clients_history", JSON.stringify(clientsHistory));
  
  renderHistory();
  showToast("تم توليد الكود وحفظ العميل بنجاح!");
}

function renderHistory(filteredList = null) {
  const listEl = document.getElementById("historyList");
  const countEl = document.getElementById("clientCount");
  
  const dataToRender = filteredList || clientsHistory;
  countEl.textContent = clientsHistory.length;

  if (dataToRender.length === 0) {
    listEl.innerHTML = `<div style="text-align:center; color:var(--muted); font-size:11px; padding:25px;">لا يوجد عملاء مسجلين حالياً</div>`;
    return;
  }

  listEl.innerHTML = dataToRender.map(item => `
    <div class="history-item">
      <div class="history-info">
        <h4>${item.name} <span style="font-size:9px; color:var(--lime);">(${item.accountant})</span></h4>
        <p>الإنشاء: ${item.createdAt} | ينتهي: ${item.expiresAt}</p>
      </div>
      <div class="history-actions">
        <button class="btn-sm btn-sm-copy" onclick="copySpecificKey('${item.key}')">نسخ</button>
        <button class="btn-sm btn-sm-del" onclick="deleteClient(${item.id})">حذف</button>
      </div>
    </div>
  `).join('');
}

function filterHistory() {
  const query = document.getElementById("searchBox").value.toLowerCase();
  const filtered = clientsHistory.filter(item => 
    item.name.toLowerCase().includes(query) || 
    item.accountant.toLowerCase().includes(query)
  );
  renderHistory(filtered);
}

function copyKey() {
  const keyText = document.getElementById("keyResult").textContent;
  copyToClipboard(keyText);
}

function copySpecificKey(key) {
  copyToClipboard(key);
}

function copyToClipboard(text) {
  navigator.clipboard.writeText(text).then(() => {
    showToast("تم نسخ كود التفعيل!");
  });
}

function deleteClient(id) {
  clientsHistory = clientsHistory.filter(item => item.id !== id);
  localStorage.setItem("app_clients_history", JSON.stringify(clientsHistory)); مفضلة
  renderHistory();
  showToast("تم حذف العميل من السجل");
}

function showToast(msg) {
  const t = document.getElementById("toastMsg");
  t.textContent = msg;
  t.classList.add('show');
  setTimeout(() => t.classList.remove('show'), 2000);
}
</script>
</body>
</html>
