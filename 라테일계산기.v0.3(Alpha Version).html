<!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>메모리얼 계산기 · 라테일</title>
<meta name="theme-color" content="#0c0c0c">
<link rel="icon" type="image/svg+xml" href="data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 32 32'><rect width='32' height='32' rx='7' fill='%230c0c0c'/><polygon points='16,4 27,10 27,22 16,28 5,22 5,10' fill='%231e3a8a'/><polygon points='16,4 27,10 16,13 5,10' fill='%233b82f6'/><polygon points='27,10 27,22 16,28 16,13' fill='%232563eb'/><polygon points='5,10 16,13 16,28 5,22' fill='%231d4ed8'/><polygon points='16,4 22,8 16,10 10,8' fill='%2393c5fd' opacity='.7'/><polygon points='16,13 20,16 16,24 12,16' fill='white' opacity='.07'/></svg>">
<style>
*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
:root {
  --bg: #0c0c0c;
  --bg2: #141414;
  --bg3: #1e1e1e;
  --bg4: #282828;
  --txt: #f0f0f0;
  --txt2: #b8b8b8;
  --txt3: #888;
  --border: rgba(255,255,255,0.08);
  --border2: rgba(255,255,255,0.15);
  --blue: #3b82f6;
  --blue-txt: #93c5fd;
  --blue-bg: rgba(59,130,246,0.1);
  --green: #22c55e;
  --green-txt: #86efac;
  --green-bg: rgba(34,197,94,0.08);
  --amber-txt: #fcd34d;
  --amber-bg: rgba(245,158,11,0.1);
  --red-txt: #fca5a5;
  --red-bg: rgba(239,68,68,0.1);
  --rad: 7px;
  --rad-lg: 10px;
}
body {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Noto Sans KR', sans-serif;
  background: var(--bg);
  color: var(--txt);
  height: 100vh;
  overflow: hidden;
  display: flex;
  flex-direction: column;
  -webkit-font-smoothing: antialiased;
}
#global-list::-webkit-scrollbar,
.panel-right::-webkit-scrollbar { width: 4px; }
#global-list::-webkit-scrollbar-track,
.panel-right::-webkit-scrollbar-track { background: var(--bg3); border-radius: 4px; }
#global-list::-webkit-scrollbar-thumb,
.panel-right::-webkit-scrollbar-thumb { background: rgba(255,255,255,0.3); border-radius: 4px; }
#global-list::-webkit-scrollbar-thumb:hover,
.panel-right::-webkit-scrollbar-thumb:hover { background: rgba(255,255,255,0.55); }
.container { max-width: 1060px; margin: 0 auto; padding: 0.75rem 1.5rem; flex: 1; display: flex; flex-direction: column; overflow: hidden; min-height: 0; width: 100%; }

/* Header */
.app-header {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
  gap: 10px;
  margin-bottom: 0.6rem;
  padding-bottom: 0.6rem;
  border-bottom: 1px solid var(--border);
  flex-shrink: 0;
}
h1 { font-size: 20px; font-weight: 600; letter-spacing: -0.02em; }
.subtitle { font-size: 11px; color: var(--txt3); }

/* Two-column layout */
.layout { display: flex; align-items: stretch; gap: 0; flex: 1; min-height: 0; }
.panel-divider { width: 1px; background: var(--border); margin: 0 1.75rem; flex-shrink: 0; }
.panel-left { width: 320px; flex-shrink: 0; display: flex; flex-direction: column; overflow: hidden; }
.panel-right { flex: 1; min-width: 0; overflow-y: auto; }
#left-global { display: flex; flex-direction: column; flex: 1; min-height: 0; }
#global-list { overflow-y: auto; flex: 1; min-height: 0; }
#page-memorial { flex: 1; overflow: hidden; display: flex; flex-direction: column; min-height: 0; }
#page-artifact, #page-weight { flex: 1; overflow-y: auto; min-height: 0; }

/* Panel tabs */
.panel-tabs { display: flex; border-bottom: 1px solid var(--border); margin-bottom: 1.25rem; }
.tab {
  font-size: 12px; padding: 8px 15px; border: none; background: transparent;
  color: var(--txt2); cursor: pointer; transition: color .15s;
  border-bottom: 2px solid transparent; margin-bottom: -1px; white-space: nowrap;
}
.tab:hover { color: var(--txt); }
.tab.on { color: var(--txt); border-bottom-color: var(--blue); }

/* Memorial nav */
#mem-nav { margin-bottom: 1.25rem; padding-bottom: 1rem; border-bottom: 1px solid var(--border); }
#mem-groups { display: flex; flex-wrap: wrap; gap: 6px; margin-bottom: 8px; }
#mem-bottom { display: flex; gap: 8px; align-items: center; flex-wrap: wrap; min-height: 22px; }
#mem-types { display: flex; gap: 5px; flex-wrap: wrap; }
.mem-btn {
  font-size: 12px; padding: 5px 13px; border-radius: 20px;
  border: 1px solid var(--border2); cursor: pointer;
  background: transparent; color: var(--txt2); transition: all .15s; white-space: nowrap;
}
.mem-btn:hover:not(.on) { background: var(--bg3); color: var(--txt); }
.mem-btn.on { background: var(--blue); color: #fff; border-color: var(--blue); }
.mem-btn.sub { font-size: 11px; padding: 3px 10px; border-radius: var(--rad); }
.mem-btn.sub.on { background: var(--bg3); color: var(--txt); border-color: var(--border2); }
#type-badge { font-size: 10px; padding: 2px 8px; border-radius: 4px; background: var(--bg3); color: var(--txt2); border: 1px solid var(--border); }
#cost-lbl { font-size: 11px; color: var(--txt3); }

/* Card */
.card { background: var(--bg2); border: 1px solid var(--border); border-radius: var(--rad-lg); padding: 1.25rem; margin-bottom: 10px; }
.st { font-size: 10px; font-weight: 600; color: var(--txt3); text-transform: uppercase; letter-spacing: .08em; margin-bottom: 12px; }

/* Metrics */
.mg { display: grid; grid-template-columns: repeat(auto-fit, minmax(120px, 1fr)); gap: 8px; margin-bottom: 12px; }
.mc { background: var(--bg3); border-radius: var(--rad); padding: .9rem; border: 1px solid var(--border); }
.mc-l { font-size: 10px; color: var(--txt2); margin-bottom: 5px; }
.mc-v { font-size: 20px; font-weight: 600; letter-spacing: -0.03em; line-height: 1; }
.mc-s { font-size: 10px; color: var(--txt3); margin-top: 5px; }

/* Table */
.tbl { width: 100%; border-collapse: collapse; font-size: 13px; }
.tbl th { font-size: 10px; font-weight: 500; color: var(--txt3); text-align: center; padding: 7px 8px; border-bottom: 1px solid var(--border); }
.tbl td { padding: 8px 8px; border-bottom: 1px solid var(--border); color: var(--txt); vertical-align: middle; }
.tbl tr:last-child td { border-bottom: none; }
.tbl tr.hl td { background: var(--blue-bg); color: var(--blue-txt); }

/* Inputs */
.sel-opt { font-size: 12px; padding: 5px 7px; border-radius: var(--rad); border: 1px solid var(--border); background: var(--bg3); color: var(--txt); width: 100%; outline: none; }
.sel-opt:focus { border-color: var(--blue); }
.num-in { font-size: 12px; padding: 5px 7px; border-radius: var(--rad); border: 1px solid var(--border); background: var(--bg3); color: var(--txt); width: 80px; text-align: right; outline: none; -moz-appearance: textfield; appearance: textfield; }
.num-in:focus { border-color: var(--blue); }
.num-in::-webkit-inner-spin-button, .num-in::-webkit-outer-spin-button { -webkit-appearance: none; margin: 0; }
select { background: var(--bg3); color: var(--txt); }

/* Progress bar */
.bar-w { width: 100%; height: 3px; background: var(--bg4); border-radius: 2px; overflow: hidden; margin-top: 8px; }
.bar-f { height: 100%; border-radius: 2px; transition: width .3s; }

/* Row */
.row { display: flex; justify-content: space-between; align-items: center; padding: 9px 0; border-bottom: 1px solid var(--border); font-size: 13px; }
.row:last-child { border-bottom: none; }
.row > span:first-child { color: var(--txt2); }

/* Strategy cards */
.strat-card { border-radius: var(--rad); padding: 11px 13px; margin-bottom: 7px; border: 1px solid var(--border); background: var(--bg3); }
.strat-card.reroll { border-color: rgba(59,130,246,0.22); background: rgba(59,130,246,0.05); }
.strat-card.keep { background: var(--bg3); }
.strat-card.locked { background: rgba(34,197,94,0.05); border-color: rgba(34,197,94,0.2); }

/* Badges */
.badge { display: inline-block; font-size: 10px; padding: 2px 7px; border-radius: 4px; font-weight: 500; white-space: nowrap; }
.bg { background: var(--green-bg); color: var(--green-txt); }
.bw { background: var(--amber-bg); color: var(--amber-txt); }
.br { background: var(--red-bg); color: var(--red-txt); }
.bb { background: var(--blue-bg); color: var(--blue-txt); }

/* Rank */
.rank-num { width: 20px; height: 20px; border-radius: 50%; display: inline-flex; align-items: center; justify-content: center; font-size: 10px; font-weight: 600; background: var(--blue); color: #fff; flex-shrink: 0; }

/* Lock button */
.lock-btn { font-size: 11px; padding: 4px 10px; border-radius: var(--rad); border: 1px solid var(--border2); cursor: pointer; background: transparent; color: var(--txt2); white-space: nowrap; transition: all .15s; }
.lock-btn:hover { background: var(--bg4); color: var(--txt); }
.lock-btn.on { background: var(--green-bg); color: var(--green-txt); border-color: rgba(34,197,94,0.25); }

/* Weight grid */
.opt-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 6px; margin-bottom: 12px; }
.opt-item { background: var(--bg3); border-radius: var(--rad); padding: 8px 11px; display: flex; align-items: center; gap: 8px; font-size: 12px; border: 1px solid var(--border); }
.opt-item label { flex: 1; color: var(--txt2); }
.opt-item input[type=number] { width: 76px; font-size: 12px; padding: 3px 6px; border-radius: var(--rad); border: 1px solid var(--border); background: var(--bg4); color: var(--txt); text-align: right; outline: none; }
.opt-item input[type=number]:focus { border-color: var(--blue); }
.opt-item input[type=number]::-webkit-inner-spin-button, .opt-item input[type=number]::-webkit-outer-spin-button { -webkit-appearance: none; margin: 0; }
.opt-item input[type=number] { -moz-appearance: textfield; appearance: textfield; }

/* Info box */
.info-box { background: var(--bg3); border-radius: var(--rad); padding: 10px 12px; font-size: 12px; color: var(--txt2); line-height: 1.7; margin-top: 10px; border: 1px solid var(--border); }

/* Filter row (global strategy) */
.filter-row { display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; gap: 8px; margin-bottom: 12px; }

/* Page nav */
.page-nav { display: flex; gap: 0; border-bottom: 1px solid var(--border); margin-bottom: 0.75rem; flex-shrink: 0; }
.page-tab { font-size: 13px; font-weight: 500; padding: 9px 20px; border: none; background: transparent; color: var(--txt2); cursor: pointer; transition: color .15s; border-bottom: 2px solid transparent; margin-bottom: -1px; }
.page-tab:hover { color: var(--txt); }
.page-tab.on { color: var(--txt); border-bottom-color: var(--blue); }

/* Artifact grid inner scroll */
#art-grid { overflow-x: auto; scrollbar-color: rgba(59,130,246,0.8) var(--bg3); scrollbar-width: thin; padding-bottom: 30px; }
#art-grid table { min-width: 1440px; }
#art-grid::-webkit-scrollbar { height: 4px; }
#art-grid::-webkit-scrollbar-track { background: var(--bg3); border-radius: 2px; }
#art-grid::-webkit-scrollbar-thumb { background: rgba(59,130,246,0.8); border-radius: 2px; }

/* Weight page */
.weight-page { max-width: 700px; }
.weight-section { margin-bottom: 2rem; }
.weight-section-title { font-size: 11px; font-weight: 600; color: var(--txt3); text-transform: uppercase; letter-spacing: .08em; margin-bottom: 12px; padding-bottom: 8px; border-bottom: 1px solid var(--border); }

@media (max-width: 900px) {
  body { height: auto; overflow: auto; display: block; }
  .container { flex: none; overflow: visible; display: block; padding: 1.25rem 1rem; }
  .app-header { margin-bottom: 1rem; padding-bottom: 0.75rem; }
  .page-nav { margin-bottom: 1rem; }
  .layout { flex-direction: column; flex: none; min-height: auto; align-items: flex-start; }
  .panel-divider { display: none; }
  .panel-left { width: 100%; margin-bottom: 2rem; padding-bottom: 2rem; border-bottom: 1px solid var(--border); overflow: visible; height: auto !important; }
  .panel-right { overflow-y: visible; width: 100%; }
  #header-btns { margin-left: 0; width: 100%; }
  .range-hint { display: none !important; }
  .slot-tbl .col-val { width: 88px !important; }
  .slot-tbl .col-score { width: 58px !important; }
  .slot-tbl .col-eval { width: 62px !important; }
  #left-global { flex: none; overflow: visible; }
  #global-list { overflow-y: visible; flex: none; }
  #page-memorial { flex: none; overflow: visible; }
  #page-artifact, #page-weight { overflow-y: visible; flex: none; }
}
</style>
</head>
<body>
<div class="container">

  <div class="app-header">
    <h1>라테일 계산기</h1>
    <span class="subtitle">문의 : 테일스타</span>
    <a href="https://open.kakao.com/o/shJpJCyi" target="_blank" style="padding:3px 9px;border:1.5px solid #facc15;border-radius:6px;color:#facc15;font-size:9px;text-decoration:none;white-space:nowrap;align-self:center">오픈카톡</a>
    <div id="header-btns" style="display:flex;align-items:center;gap:8px;margin-left:auto">
      <button class="lock-btn" onclick="exportJSON()">내보내기</button>
      <label class="lock-btn" style="cursor:pointer">불러오기
        <input type="file" accept=".json" style="display:none" onchange="importJSON(this.files[0]);this.value=''">
      </label>
      <button class="lock-btn" style="color:var(--red-txt);border-color:rgba(239,68,68,0.3)" onclick="resetAllData()">전체 초기화</button>
    </div>
  </div>

  <div class="page-nav">
    <button class="page-tab on" onclick="setPageTab('memorial',this)">메모리얼</button>
    <button class="page-tab" onclick="setPageTab('artifact',this)">성물석</button>
    <button class="page-tab" onclick="setPageTab('weight',this)">환산치</button>
  </div>

  <!-- ── 메모리얼 페이지 ── -->
  <div id="page-memorial">
  <div class="layout">

    <!-- ── 좌측 패널: 전체 전략 + 환산치 ── -->
    <div class="panel panel-left">
      <div id="left-global">
        <!-- 전체 메모리얼 총 환산치 -->
        <div class="card" id="global-summary" style="margin-bottom:12px">
          <div class="st">전체 메모리얼 총 환산치</div>
          <div id="summary-total" style="font-size:32px;font-weight:600;letter-spacing:-0.03em;line-height:1">—</div>
          <div id="summary-sub" style="font-size:11px;color:var(--txt3);margin-top:6px"></div>
        </div>

        <div class="filter-row">
          <select id="global-sort" class="sel-opt" style="width:auto" onchange="renderGlobalStrategy()">
            <option value="cpPer0_1">조각 비용 효율 순</option>
            <option value="ccPer0_1">결정 비용 효율 순</option>
            <option value="remaining">잔여 잠재력 순</option>
            <option value="expectedRolls">개선 기대 횟수 순</option>
          </select>
          <label style="font-size:12px;display:flex;align-items:center;gap:5px;cursor:pointer;color:var(--txt2)">
            <input type="checkbox" id="global-show-empty" onchange="renderGlobalStrategy()">
            미입력 포함
          </label>
          <button class="lock-btn" style="color:var(--red-txt);border-color:rgba(239,68,68,0.3)" onclick="resetMemorial()">메모리얼 초기화</button>
        </div>
        <div id="global-list"></div>
      </div>

    </div>

    <div class="panel-divider"></div>

    <!-- ── 우측 패널: 메모리얼 관련 ── -->
    <div class="panel panel-right">
      <div class="panel-tabs">
        <button class="tab on" onclick="setTab('slots',this)">슬롯 입력</button>
        <button class="tab" onclick="setTab('strategy',this)" style="display:none">투자 전략</button>
      </div>

      <!-- 메모리얼 선택 -->
      <div id="mem-nav">
        <div id="mem-groups"></div>
        <div id="mem-bottom">
          <div id="mem-types"></div>
          <span id="type-badge" class="badge bb"></span>
          <span id="cost-lbl"></span>
        </div>
      </div>

      <!-- 슬롯 입력 -->
      <div id="tab-slots">
        <div class="card">
          <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:14px">
            <div class="st" style="margin:0">현재 슬롯 상태 입력</div>
            <button class="lock-btn" onclick="clearAll()">초기화</button>
          </div>
          <div style="overflow-x:auto">
            <table class="tbl slot-tbl" style="table-layout:fixed">
              <thead><tr>
                <th style="width:32px">#</th>
                <th>현재 옵션</th>
                <th class="col-val" style="width:148px">현재 값</th>
                <th class="col-score" style="width:68px">환산치</th>
                <th class="col-eval" style="width:72px">평가</th>
              </tr></thead>
              <tbody id="slot-tbody"></tbody>
            </table>
          </div>
        </div>
        <div class="mg" id="slot-metrics">
          <div class="mc"><div class="mc-l">현재 총 환산치</div><div class="mc-v" id="sm-total">—</div><div class="mc-s">전체 슬롯 합산</div></div>
        </div>
      </div>

      <!-- 투자 전략 -->
      <div id="tab-strategy" style="display:none">
        <div class="mg" id="strat-metrics"></div>
        <div class="card">
          <div class="st">슬롯별 투자 판단 — 환산치 기준 자동 분석</div>
          <div id="strat-list"></div>
        </div>
        <div class="card">
          <div class="st">전체 투자 요약</div>
          <div id="strat-cost"></div>
        </div>
      </div>

    </div>

  </div>
</div>

<!-- ── 성물석 페이지 ── -->
<div id="page-artifact" style="display:none">
  <div style="display:flex;align-items:center;gap:20px;margin-bottom:1.5rem;flex-wrap:wrap">
    <div style="display:flex;align-items:center;gap:8px">
      <span style="font-size:12px;color:var(--txt2)">시작 성물</span>
      <select id="art-start" class="sel-opt" style="width:auto" onchange="onArtSettingChange()">
        <option value="0">마아트</option>
        <option value="1">프리링</option>
        <option value="2">글레이프니르</option>
        <option value="3">타바숨</option>
        <option value="4">여우구슬</option>
        <option value="5">구름방망이</option>
      </select>
    </div>
    <div style="display:flex;align-items:center;gap:8px">
      <span style="font-size:12px;color:var(--txt2)">던전 시간</span>
      <input id="art-dungeon-min" class="num-in" type="number" min="1" max="120" step="1" value="10" style="width:60px" onchange="onArtSettingChange()">
      <span style="font-size:12px;color:var(--txt2)">분</span>
    </div>
    <span id="art-usage-display" style="font-size:11px;color:var(--txt3)"></span>
    <button class="lock-btn" style="color:var(--red-txt);border-color:rgba(239,68,68,0.3)" onclick="resetArtAll()">데이터 초기화</button>
    <span style="font-size:11px;color:var(--amber-txt);background:var(--amber-bg);border:1px solid rgba(245,158,11,0.2);border-radius:var(--rad);padding:3px 10px;margin-left:auto">⚠ 해당 프로그램은 성물 1440 만렙 기준으로 적용됩니다.</span>
  </div>

  <div id="art-grid"></div>
</div>

<!-- ── 환산치 페이지 ── -->
<div id="page-weight" style="display:none">
  <div style="max-width:800px">
    <div style="display:flex;justify-content:flex-end;margin-bottom:12px">
      <button class="lock-btn" style="color:var(--red-txt);border-color:rgba(239,68,68,0.3)" onclick="resetWeights()">기본값 복원</button>
    </div>
    <div class="card">
      <div class="st">메모리얼 환산치 — 수치 1당 가중치</div>
      <div id="wp-memorial-grid" class="opt-grid"></div>
      <button class="lock-btn" style="margin-top:10px" onclick="W={...WD};saveAll();renderWeightPage()">기본값 초기화</button>
    </div>
    <div class="card" style="margin-top:12px">
      <div class="st">공용석 환산치 — 수치 1당 가중치</div>
      <div id="wp-shared-grid" class="opt-grid"></div>
      <button class="lock-btn" style="margin-top:10px" onclick="WD2={...WD2_DEFAULT};saveAll();renderWeightPage()">기본값 초기화</button>
    </div>
  </div>
</div>

<script>
const WD = {
  "크리티컬 대미지":1.0,"근력/마법력":0.0016,"근마%":4.0,"올스탯":0.002,"올스탯%":5.0,
  "무공/속성력":0.25,"무공/속성력%":6.0,"고정 대미지":0.001,"고정 대미지%":1.0,
  "최대 대미지":0.55,"최소 대미지":0.55,"최소+최대":1.1,"최종 최소 대미지":30.0,
  "최종 최대 대미지":30.0,"최종 크리티컬 대미지":55.0,"보스 몬스터 지배력":20.0,
  "일반 몬스터 지배력":20.0,"백어택":0.4,
  "보스 몬스터 추가 대미지":0.0005,"일반 몬스터 추가 대미지":0.0005,"꽝":0
};

const MEM = [
  {name:"무웬",type:"개별",cp:1,cc:1,slots:9,opts:[
    {p:6,k:"근력/마법력",mn:10,mx:100},{p:5,k:"근력/마법력",mn:50,mx:200},{p:3.5,k:"근력/마법력",mn:100,mx:400},{p:1.5,k:"근력/마법력",mn:150,mx:700},{p:0.5,k:"근력/마법력",mn:200,mx:1500},
    {p:6,k:"올스탯",mn:7,mx:70},{p:5,k:"올스탯",mn:35,mx:140},{p:3.5,k:"올스탯",mn:70,mx:250},{p:1.5,k:"올스탯",mn:105,mx:500},{p:0.7,k:"올스탯",mn:140,mx:1000}
  ]},
  {name:"무웬 (세트)",type:"세트",cp:20,cc:3,opts:[
    {p:10,k:"근마%",mn:1,mx:2},{p:5,k:"근마%",mn:2,mx:4},{p:1.7,k:"근마%",mn:3,mx:6},
    {p:10,k:"올스탯%",mn:1,mx:1},{p:4,k:"올스탯%",mn:1,mx:3},{p:1,k:"올스탯%",mn:2,mx:5}
  ]},
  {name:"레비",type:"개별",cp:1,cc:1,slots:9,opts:[
    {p:6,k:"무공/속성력",mn:1,mx:4},{p:5,k:"무공/속성력",mn:2,mx:7},{p:3.5,k:"무공/속성력",mn:3,mx:11},{p:1.5,k:"무공/속성력",mn:4,mx:16},{p:0.7,k:"무공/속성력",mn:8,mx:40},
    {p:6,k:"최소 대미지",mn:1,mx:2},{p:5,k:"최소 대미지",mn:1,mx:4},{p:3.5,k:"최소 대미지",mn:2,mx:5},{p:1.5,k:"최소 대미지",mn:2,mx:8},{p:0.7,k:"최소 대미지",mn:4,mx:15},
    {p:6,k:"최대 대미지",mn:1,mx:2},{p:5,k:"최대 대미지",mn:1,mx:4},{p:3.5,k:"최대 대미지",mn:2,mx:5},{p:1.5,k:"최대 대미지",mn:2,mx:8},{p:0.7,k:"최대 대미지",mn:4,mx:15},
    {p:6,k:"크리티컬 대미지",mn:1,mx:2},{p:5,k:"크리티컬 대미지",mn:1,mx:4},{p:3.5,k:"크리티컬 대미지",mn:2,mx:5},{p:1.5,k:"크리티컬 대미지",mn:2,mx:8},{p:0.7,k:"크리티컬 대미지",mn:4,mx:15},
    {p:6,k:"백어택",mn:1,mx:3},{p:5,k:"백어택",mn:2,mx:6},{p:3.5,k:"백어택",mn:3,mx:8},{p:1.5,k:"백어택",mn:4,mx:12},{p:0.7,k:"백어택",mn:7,mx:25}
  ]},
  {name:"레비 (세트)",type:"세트",cp:20,cc:3,opts:[
    {p:5.1335,k:"고정 대미지%",mn:1,mx:1},{p:2.5667,k:"고정 대미지%",mn:2,mx:4},{p:0.8214,k:"고정 대미지%",mn:3,mx:8},
    {p:5.1335,k:"무공/속성력%",mn:1,mx:1},{p:2.5667,k:"무공/속성력%",mn:1,mx:3},{p:0.8214,k:"무공/속성력%",mn:2,mx:6},
    {p:5.1335,k:"최종 최소 대미지",mn:1,mx:1},{p:2.5667,k:"최종 최소 대미지",mn:1,mx:2},{p:0.8214,k:"최종 최소 대미지",mn:1,mx:3},
    {p:5.1335,k:"최종 최대 대미지",mn:1,mx:1},{p:2.5667,k:"최종 최대 대미지",mn:1,mx:2},{p:0.8214,k:"최종 최대 대미지",mn:1,mx:3},
    {p:5.1335,k:"최종 크리티컬 대미지",mn:1,mx:1},{p:2.0534,k:"최종 크리티컬 대미지",mn:1,mx:2},{p:0.616,k:"최종 크리티컬 대미지",mn:1,mx:3},
    {p:5.1335,k:"고정 대미지",mn:100,mx:1000},{p:2.5667,k:"고정 대미지",mn:500,mx:2000},{p:0.8214,k:"고정 대미지",mn:1000,mx:6000},
    {p:5.1335,k:"무공/속성력",mn:2,mx:15},{p:2.5667,k:"무공/속성력",mn:5,mx:30},{p:0.8214,k:"무공/속성력",mn:15,mx:80},
    {p:5.1335,k:"최소 대미지",mn:1,mx:5},{p:2.5667,k:"최소 대미지",mn:3,mx:15},{p:0.8214,k:"최소 대미지",mn:5,mx:30},
    {p:5.1335,k:"최대 대미지",mn:1,mx:5},{p:2.5667,k:"최대 대미지",mn:3,mx:15},{p:0.8214,k:"최대 대미지",mn:8,mx:30},
    {p:5.1335,k:"크리티컬 대미지",mn:1,mx:5},{p:2.0534,k:"크리티컬 대미지",mn:3,mx:15},{p:0.616,k:"크리티컬 대미지",mn:8,mx:30}
  ]},
  {name:"리리",type:"세트",cp:30,cc:3,opts:[
    {p:12.3457,k:"최소 대미지",mn:1,mx:5},{p:9.8765,k:"최소 대미지",mn:1,mx:10},{p:6.7901,k:"최소 대미지",mn:2,mx:15},{p:3.0864,k:"최소 대미지",mn:3,mx:20},{p:1.2346,k:"최소 대미지",mn:4,mx:25},
    {p:12.3457,k:"최대 대미지",mn:1,mx:5},{p:9.8765,k:"최대 대미지",mn:1,mx:10},{p:6.7901,k:"최대 대미지",mn:2,mx:15},{p:3.0864,k:"최대 대미지",mn:3,mx:20},{p:1.2346,k:"최대 대미지",mn:4,mx:25},
    {p:12.3457,k:"최소+최대",mn:1,mx:5},{p:9.8765,k:"최소+최대",mn:1,mx:10},{p:6.7901,k:"최소+최대",mn:2,mx:15},{p:3.0864,k:"최소+최대",mn:3,mx:20},{p:1.2346,k:"최소+최대",mn:4,mx:25}
  ]},
  {name:"제릴",type:"세트",cp:30,cc:3,opts:[
    {p:12.3457,k:"최소 대미지",mn:1,mx:5},{p:9.8765,k:"최소 대미지",mn:1,mx:10},{p:6.7901,k:"최소 대미지",mn:2,mx:15},{p:3.0864,k:"최소 대미지",mn:3,mx:20},{p:1.2346,k:"최소 대미지",mn:4,mx:25},
    {p:12.3457,k:"최대 대미지",mn:1,mx:5},{p:9.8765,k:"최대 대미지",mn:1,mx:10},{p:6.7901,k:"최대 대미지",mn:2,mx:15},{p:3.0864,k:"최대 대미지",mn:3,mx:20},{p:1.2346,k:"최대 대미지",mn:4,mx:25},
    {p:12.3457,k:"최소+최대",mn:1,mx:5},{p:9.8765,k:"최소+최대",mn:1,mx:10},{p:6.7901,k:"최소+최대",mn:2,mx:15},{p:3.0864,k:"최소+최대",mn:3,mx:20},{p:1.2346,k:"최소+최대",mn:4,mx:25}
  ]},
  {name:"판도라",type:"세트",cp:30,cc:3,opts:[
    {p:12.3457,k:"최소 대미지",mn:1,mx:5},{p:9.8765,k:"최소 대미지",mn:1,mx:10},{p:6.7901,k:"최소 대미지",mn:2,mx:15},{p:3.0864,k:"최소 대미지",mn:3,mx:20},{p:1.2346,k:"최소 대미지",mn:4,mx:25},
    {p:12.3457,k:"최대 대미지",mn:1,mx:5},{p:9.8765,k:"최대 대미지",mn:1,mx:10},{p:6.7901,k:"최대 대미지",mn:2,mx:15},{p:3.0864,k:"최대 대미지",mn:3,mx:20},{p:1.2346,k:"최대 대미지",mn:4,mx:25},
    {p:12.3457,k:"최소+최대",mn:1,mx:5},{p:9.8765,k:"최소+최대",mn:1,mx:10},{p:6.7901,k:"최소+최대",mn:2,mx:15},{p:3.0864,k:"최소+최대",mn:3,mx:20},{p:1.2346,k:"최소+최대",mn:4,mx:25}
  ]},
  {name:"아르케",type:"세트",cp:30,cc:3,opts:[
    {p:12.3457,k:"최소 대미지",mn:1,mx:5},{p:9.8765,k:"최소 대미지",mn:1,mx:10},{p:6.7901,k:"최소 대미지",mn:2,mx:15},{p:3.0864,k:"최소 대미지",mn:3,mx:20},{p:1.2346,k:"최소 대미지",mn:4,mx:25},
    {p:12.3457,k:"최대 대미지",mn:1,mx:5},{p:9.8765,k:"최대 대미지",mn:1,mx:10},{p:6.7901,k:"최대 대미지",mn:2,mx:15},{p:3.0864,k:"최대 대미지",mn:3,mx:20},{p:1.2346,k:"최대 대미지",mn:4,mx:25},
    {p:12.3457,k:"최소+최대",mn:1,mx:5},{p:9.8765,k:"최소+최대",mn:1,mx:10},{p:6.7901,k:"최소+최대",mn:2,mx:15},{p:3.0864,k:"최소+최대",mn:3,mx:20},{p:1.2346,k:"최소+최대",mn:4,mx:25}
  ]},
  {name:"흑월공주",type:"개별",cp:4,cc:1,slots:9,opts:[
    {p:6,k:"근력/마법력",mn:10,mx:150},{p:5,k:"근력/마법력",mn:50,mx:300},{p:3.5,k:"근력/마법력",mn:100,mx:600},{p:1.5,k:"근력/마법력",mn:150,mx:1050},{p:0.5,k:"근력/마법력",mn:200,mx:2250},
    {p:6,k:"올스탯",mn:7,mx:105},{p:5,k:"올스탯",mn:35,mx:210},{p:3.5,k:"올스탯",mn:70,mx:375},{p:1.5,k:"올스탯",mn:105,mx:750},{p:0.7,k:"올스탯",mn:140,mx:1500}
  ]},
  {name:"흑월공주 (세트)",type:"세트",cp:40,cc:3,opts:[
    {p:10,k:"근마%",mn:1,mx:3},{p:5,k:"근마%",mn:2,mx:6},{p:1.7,k:"근마%",mn:3,mx:9},
    {p:10,k:"올스탯%",mn:1,mx:1},{p:4,k:"올스탯%",mn:1,mx:4},{p:1,k:"올스탯%",mn:2,mx:7}
  ]},
  {name:"초엔팜",type:"개별",cp:4,cc:1,slots:9,opts:[
    {p:6,k:"무공/속성력",mn:1,mx:6},{p:5,k:"무공/속성력",mn:2,mx:10},{p:3.5,k:"무공/속성력",mn:3,mx:16},{p:1.5,k:"무공/속성력",mn:4,mx:24},{p:0.7,k:"무공/속성력",mn:8,mx:60},
    {p:6,k:"최소 대미지",mn:1,mx:3},{p:5,k:"최소 대미지",mn:1,mx:6},{p:3.5,k:"최소 대미지",mn:2,mx:7},{p:1.5,k:"최소 대미지",mn:2,mx:12},{p:0.7,k:"최소 대미지",mn:4,mx:22},
    {p:6,k:"최대 대미지",mn:1,mx:3},{p:5,k:"최대 대미지",mn:1,mx:6},{p:3.5,k:"최대 대미지",mn:2,mx:7},{p:1.5,k:"최대 대미지",mn:2,mx:12},{p:0.7,k:"최대 대미지",mn:4,mx:22},
    {p:6,k:"크리티컬 대미지",mn:1,mx:3},{p:5,k:"크리티컬 대미지",mn:1,mx:6},{p:3.5,k:"크리티컬 대미지",mn:2,mx:7},{p:1.5,k:"크리티컬 대미지",mn:2,mx:12},{p:0.7,k:"크리티컬 대미지",mn:4,mx:22},
    {p:6,k:"백어택",mn:1,mx:4},{p:5,k:"백어택",mn:2,mx:9},{p:3.5,k:"백어택",mn:3,mx:12},{p:1.5,k:"백어택",mn:4,mx:18},{p:0.7,k:"백어택",mn:7,mx:37}
  ]},
  {name:"초엔팜 (세트)",type:"세트",cp:40,cc:3,opts:[
    {p:5.1335,k:"고정 대미지%",mn:1,mx:1},{p:2.5667,k:"고정 대미지%",mn:2,mx:6},{p:0.8214,k:"고정 대미지%",mn:3,mx:12},
    {p:5.1335,k:"무공/속성력%",mn:1,mx:1},{p:2.5667,k:"무공/속성력%",mn:1,mx:4},{p:0.8214,k:"무공/속성력%",mn:2,mx:9},
    {p:5.1335,k:"최종 최소 대미지",mn:1,mx:1},{p:2.5667,k:"최종 최소 대미지",mn:1,mx:3},{p:0.8214,k:"최종 최소 대미지",mn:1,mx:4},
    {p:5.1335,k:"최종 최대 대미지",mn:1,mx:1},{p:2.5667,k:"최종 최대 대미지",mn:1,mx:3},{p:0.8214,k:"최종 최대 대미지",mn:1,mx:4},
    {p:5.1335,k:"최종 크리티컬 대미지",mn:1,mx:1},{p:2.0534,k:"최종 크리티컬 대미지",mn:1,mx:3},{p:0.616,k:"최종 크리티컬 대미지",mn:1,mx:4},
    {p:5.1335,k:"고정 대미지",mn:100,mx:1500},{p:2.5667,k:"고정 대미지",mn:500,mx:3000},{p:0.8214,k:"고정 대미지",mn:1000,mx:9000},
    {p:5.1335,k:"무공/속성력",mn:2,mx:22},{p:2.5667,k:"무공/속성력",mn:5,mx:45},{p:0.8214,k:"무공/속성력",mn:15,mx:120},
    {p:5.1335,k:"최소 대미지",mn:1,mx:7},{p:2.5667,k:"최소 대미지",mn:3,mx:22},{p:0.8214,k:"최소 대미지",mn:5,mx:45},
    {p:5.1335,k:"최대 대미지",mn:1,mx:7},{p:2.5667,k:"최대 대미지",mn:3,mx:22},{p:0.8214,k:"최대 대미지",mn:8,mx:45},
    {p:5.1335,k:"크리티컬 대미지",mn:1,mx:7},{p:2.0534,k:"크리티컬 대미지",mn:3,mx:22},{p:0.616,k:"크리티컬 대미지",mn:8,mx:45}
  ]},
  {name:"게네페",type:"세트",cp:40,cc:3,opts:[
    {p:19.8413,k:"최소+최대",mn:1,mx:7},{p:9.9206,k:"최소+최대",mn:3,mx:22},{p:3.1746,k:"최소+최대",mn:8,mx:45},
    {p:19.8413,k:"일반 몬스터 지배력",mn:0.1,mx:0.5},{p:9.9206,k:"일반 몬스터 지배력",mn:0.2,mx:1.2},{p:3.1746,k:"일반 몬스터 지배력",mn:0.3,mx:3},
    {p:19.8413,k:"보스 몬스터 지배력",mn:0.1,mx:0.5},{p:9.9206,k:"보스 몬스터 지배력",mn:0.2,mx:1.2},{p:3.1746,k:"보스 몬스터 지배력",mn:0.3,mx:3},
    {p:9.8765,k:"최대 대미지",mn:1,mx:10},{p:6.7901,k:"최대 대미지",mn:2,mx:15},{p:3.0864,k:"최대 대미지",mn:3,mx:20},{p:1.2346,k:"최대 대미지",mn:4,mx:25},
    {p:12.3457,k:"최소+최대",mn:1,mx:5},{p:9.8765,k:"최소+최대",mn:1,mx:10},{p:6.7901,k:"최소+최대",mn:2,mx:15},{p:3.0864,k:"최소+최대",mn:3,mx:20},{p:1.2346,k:"최소+최대",mn:4,mx:25}
  ]}
];

const SET_SP = [{s:1,p:.3},{s:2,p:.3},{s:3,p:.3},{s:4,p:.1}];
const SK = 'latale_memorial_v4';

const WD2_DEFAULT = {
  "올스탯":0.002,"근력/마법력":0.0016,"무공/속성력":0.25,
  "백어택 대미지":0.3,"고정 대미지":0.001,
  "보스 몬스터 추가 대미지":0.0005,"일반 몬스터 추가 대미지":0.0005,
  "체력":0,"최대 HP":0,"명중률":0
};
const WD2_MAX = {
  "올스탯":2400,"근력/마법력":3000,"무공/속성력":20,
  "백어택 대미지":20,"고정 대미지":5000,
  "보스 몬스터 추가 대미지":10000,"일반 몬스터 추가 대미지":10000,
  "체력":3000,"최대 HP":10000,"명중률":5
};
let WD2 = {...WD2_DEFAULT};

const ARTIFACTS = [
  {name:"마아트",      ded:[{k:"근력/마법력%",mn:1,mx:5},    {k:"쿨타임 감소",mn:0.1,mx:5}],       syn:{di:0,affects:["근력/마법력","올스탯"]}},
  {name:"프리링",      ded:[{k:"최대HP%",mn:1,mx:5},         {k:"대미지 감소",mn:1,mx:4000}],       syn:null},
  {name:"글레이프니르",ded:[{k:"최소 대미지",mn:1,mx:50},    {k:"최대 대미지",mn:1,mx:50}],         syn:null},
  {name:"타바숨",      ded:[{k:"무공/속성력%",mn:1,mx:5},    {k:"이동속도",mn:1,mx:30}],            syn:{di:0,affects:["무공/속성력"]}},
  {name:"여우구슬",    ded:[{k:"일반 몬스터 지배력",mn:0.1,mx:1},{k:"보스 몬스터 지배력",mn:0.1,mx:1}],syn:null},
  {name:"구름방망이",  ded:[{k:"크리티컬 확률",mn:1,mx:5},   {k:"크리티컬 대미지",mn:1,mx:50}],    syn:null}
];

function initArtSD() {
  return {
    ded: ARTIFACTS.map(() => ["",""]),
    shared: ARTIFACTS.map(() => [
      Array(4).fill(null).map(() => ({opt:"",val:""})),
      Array(4).fill(null).map(() => ({opt:"",val:""}))
    ])
  };
}
function initArtNew() { return Array(4).fill(null).map(() => ({opt:"",val:""})); }

let ART_SD = initArtSD();
let ART_NEW = initArtNew();
let artDungeonMin = 10;
let artStartIdx = 0;

let W = {...WD};
let SD = {};
let MI = 0;
let curTab = 'slots';
let leftTab = 'global';
let curPageTab = 'memorial';

function saveAll() {
  try {
    localStorage.setItem(SK, JSON.stringify({W, WD2, SD, MI, ART_SD, ART_NEW, artDungeonMin, artStartIdx}));
  } catch(e) {
  }
  if (leftTab === 'global' && document.getElementById('global-list')) requestAnimationFrame(() => renderGlobalStrategy());
}
function saveState() {
  try {
    localStorage.setItem(SK, JSON.stringify({W, WD2, SD, MI, ART_SD, ART_NEW, artDungeonMin, artStartIdx}));
  } catch(e) {
  }
}
function loadAll() {
  try {
    const raw = localStorage.getItem(SK);
    if (raw) {
      const d = JSON.parse(raw);
      if (d.W) W = {...WD, ...d.W};
      if (d.WD2) WD2 = {...WD2_DEFAULT, ...d.WD2};
      if (d.SD) SD = d.SD;
      if (typeof d.MI === 'number') MI = d.MI;
      if (d.ART_SD) ART_SD = d.ART_SD;
      if (d.ART_NEW) ART_NEW = d.ART_NEW;
      if (typeof d.artDungeonMin === 'number') artDungeonMin = d.artDungeonMin;
      if (typeof d.artStartIdx === 'number') artStartIdx = d.artStartIdx;
    }
  } catch(e) {}
}

function gw(k) { return W[k] ?? 0; }
function mid(a, b) { return (a + b) / 2; }
function calcScore(opt, val) { if (!opt || opt === '꽝') return 0; return parseFloat(val || 0) * gw(opt); }
function slotKey(mi, si) { return `${mi}_${si}`; }
function getSlot(si) { const s = SD[slotKey(MI, si)] || {opt:'', val:''}; return s.opt === '꽝' ? {...s, opt:'', val:''} : s; }
function setSlot(si, obj) { SD[slotKey(MI, si)] = {...getSlot(si), ...obj}; saveAll(); }
function slotCount() { return MEM[MI].type === '개별' ? MEM[MI].slots : 4; }
function getOptKeys() { return [...new Set(MEM[MI].opts.map(o => o.k))]; }

function getOptRange(optKey) {
  if (!optKey || optKey === '꽝') return null;
  const opts = MEM[MI].opts.filter(o => o.k === optKey);
  if (!opts.length) return null;
  return { min: Math.min(...opts.map(o => o.mn)), max: Math.max(...opts.map(o => o.mx)) };
}

function calcAbsMaxScore(mem) {
  return mem.opts.reduce((mx, o) => Math.max(mx, o.mx * gw(o.k)), 0);
}

function calcProbBeatScore(mem, currentScore) {
  let p = 0;
  for (const o of mem.opts) {
    const w = gw(o.k);
    if (w <= 0) continue;
    if (currentScore <= 0) { p += o.p / 100; continue; }
    const threshold = currentScore / w;
    if (threshold >= o.mx) continue;
    const lo = Math.ceil(threshold + 1e-9);
    if (lo < o.mn) { p += o.p / 100; continue; }
    const totalVals = o.mx - o.mn + 1;
    const above = o.mx - lo + 1;
    p += (o.p / 100) * (above / totalVals);
  }
  return Math.min(1, p);
}

function drawOneSlotScore(mem) {
  const r = Math.random() * 100;
  let cum = 0;
  for (const o of mem.opts) {
    cum += o.p;
    if (r < cum) return (o.mn + Math.floor(Math.random() * (o.mx - o.mn + 1))) * gw(o.k);
  }
  return 0;
}

function calcExpectedGainPerRoll(mem, currentScore) {
  // E[max(0, newScore - currentScore)] — 현재 값 기준 기대 상승분
  let gain = 0;
  for (const o of mem.opts) {
    const w = gw(o.k);
    if (w <= 0) continue;
    if (o.mx * w <= currentScore) continue;
    if (currentScore <= 0 || o.mn * w > currentScore) {
      gain += (o.p / 100) * (mid(o.mn, o.mx) * w - Math.max(0, currentScore));
    } else {
      const lo = Math.ceil(currentScore / w + 1e-9);
      if (lo > o.mx) continue;
      const totalVals = o.mx - o.mn + 1;
      const aboveVals = o.mx - lo + 1;
      gain += (o.p / 100) * (aboveVals / totalVals) * ((lo + o.mx) / 2 * w - currentScore);
    }
  }
  return gain;
}

function calcSetMetrics(mem, currentTotal) {
  // 몬테카를로 — pBeat(개선 확률)과 eGain(기대 상승분) 동시 계산
  const N = 2000;
  let beats = 0, gainSum = 0;
  for (let i = 0; i < N; i++) {
    const r = Math.random();
    let n = 1, cum = 0;
    for (const sp of SET_SP) { cum += sp.p; if (r < cum) { n = sp.s; break; } }
    let total = 0;
    for (let j = 0; j < n; j++) total += drawOneSlotScore(mem);
    if (total > currentTotal) { beats++; gainSum += total - currentTotal; }
  }
  return { pBeat: beats / N, eGain: gainSum / N };
}

function _mb32(seed) {
  let s = seed | 0;
  return function() {
    s = s + 0x6D2B79F5 | 0;
    let t = Math.imul(s ^ s >>> 15, 1 | s);
    t = t + Math.imul(t ^ t >>> 7, 61 | t) ^ t;
    return ((t ^ t >>> 14) >>> 0) / 4294967296;
  };
}
function calcSetMetricsDet(mem, currentTotal, mi) {
  // 시드 고정 Monte Carlo — 입력값이 같으면 결과가 항상 동일
  const N = 8000;
  const rand = _mb32((mi * 999983 + Math.round(currentTotal * 1000)) | 0);
  let beats = 0, gainSum = 0;
  for (let i = 0; i < N; i++) {
    const r = rand();
    let n = 1, cum = 0;
    for (const sp of SET_SP) { cum += sp.p; if (r < cum) { n = sp.s; break; } }
    let total = 0;
    for (let j = 0; j < n; j++) {
      const r2 = rand() * 100;
      let cum2 = 0;
      for (const o of mem.opts) {
        cum2 += o.p;
        if (r2 < cum2) { total += (o.mn + Math.floor(rand() * (o.mx - o.mn + 1))) * gw(o.k); break; }
      }
    }
    if (total > currentTotal) { beats++; gainSum += total - currentTotal; }
  }
  return { pBeat: beats / N, eGain: gainSum / N };
}

function calcRemainingPotential(mem, currentScore) {
  return Math.max(0, calcAbsMaxScore(mem) - currentScore);
}

const EVAL_THRESHOLDS = {
  '무웬':            {novice:0.5,  near:1.2,  end:2 },
  '레비':            {novice:5,    near:8,    end:13  },
  '흑월공주':        {novice:0.7,  near:2,  end:2.5 },
  '초엔팜':          {novice:8,    near:12,   end:17  },
  '무웬 (세트)':     {novice:10,   near:22,   end:30  },
  '레비 (세트)':     {novice:90,   near:150,  end:200 },
  '흑월공주 (세트)': {novice:20,   near:30,   end:40  },
  '초엔팜 (세트)':   {novice:140,  near:200,  end:250 },
  '리리':            {novice:12,   near:19,   end:25  },
  '제릴':            {novice:12,   near:19,   end:25  },
  '판도라':          {novice:12,   near:19,   end:25  },
  '아르케':          {novice:12,   near:19,   end:25  },
  '게네페':          {novice:50,   near:70,   end:100  },
};
function getEvalTier(mem, score) {
  const th = EVAL_THRESHOLDS[mem.name];
  if (!th) return {label:'—', color:'var(--txt3)', bg:'transparent'};
  if (score >= th.end)    return {label:'종결',   color:'var(--green-txt)', bg:'rgba(34,197,94,0.15)'};
  if (score >= th.near)   return {label:'준종결', color:'#a78bfa',          bg:'rgba(167,139,250,0.15)'};
  if (score >= th.novice) return {label:'뉴비',   color:'var(--blue-txt)',  bg:'var(--blue-bg)'};
  return {label:'미달', color:'var(--red-txt)', bg:'var(--red-bg)'};
}

function calcSlotTopFraction(mem, score) {
  // 메모리얼 전체 최고 환산치 기준 상위 비율 — (maxScore - score) / maxScore
  const maxScore = calcAbsMaxScore(mem);
  if (maxScore <= 0) return 1;
  return Math.max(0, Math.min(1, (maxScore - score) / maxScore));
}

function calcProbBeatSet(mem, currentTotal) {
  const N = 300;
  let beats = 0;
  for (let i = 0; i < N; i++) {
    const r = Math.random();
    let n = 1, cum = 0;
    for (const sp of SET_SP) { cum += sp.p; if (r < cum) { n = sp.s; break; } }
    let total = 0;
    for (let j = 0; j < n; j++) total += drawOneSlotScore(mem);
    if (total > currentTotal) beats++;
  }
  return beats / N;
}

function resetMemorial() {
  if (!confirm('메모리얼 슬롯 데이터를 초기화합니다. 계속하시겠습니까?')) return;
  SD = {};
  MI = 0;
  saveAll();
  renderAll();
  renderGlobalStrategy();
}

function resetAllData() {
  if (!confirm('모든 데이터(메모리얼 + 성물석)를 초기화합니다. 계속하시겠습니까?')) return;
  SD = {};
  MI = 0;
  ART_SD = initArtSD();
  ART_NEW = initArtNew();
  saveAll();
  renderAll();
  renderGlobalStrategy();
  if (curPageTab === 'artifact') renderArtGrid();
}

function exportJSON() {
  const blob = new Blob([JSON.stringify({W, WD2, SD, MI, ART_SD, ART_NEW, artDungeonMin, artStartIdx}, null, 2)], {type:'application/json'});
  const a = document.createElement('a');
  a.href = URL.createObjectURL(blob);
  a.download = 'memorial_data.json';
  a.click();
  URL.revokeObjectURL(a.href);
}

function importJSON(file) {
  if (!file) return;
  const reader = new FileReader();
  reader.onload = e => {
    try {
      const d = JSON.parse(e.target.result);
      if (d.W) W = {...WD, ...d.W};
      if (d.WD2) WD2 = {...WD2_DEFAULT, ...d.WD2};
      if (d.SD) SD = d.SD;
      if (typeof d.MI === 'number') MI = d.MI;
      if (d.ART_SD) ART_SD = d.ART_SD;
      if (d.ART_NEW) ART_NEW = d.ART_NEW;
      if (typeof d.artDungeonMin === 'number') artDungeonMin = d.artDungeonMin;
      if (typeof d.artStartIdx === 'number') artStartIdx = d.artStartIdx;
      saveAll();
      renderAll();
      if (curPageTab === 'artifact') renderArtPage();
      else if (curPageTab === 'weight') renderWeightPage();
      else if (leftTab === 'global') renderGlobalStrategy();
    } catch(err) { alert('파일 형식이 올바르지 않습니다.'); }
  };
  reader.readAsText(file);
}

function calcTotalEVFor(mem) {
  let ev = mem.opts.reduce((s, o) => s + (o.p/100) * mid(o.mn, o.mx) * gw(o.k), 0);
  if (mem.type === '세트') ev *= SET_SP.reduce((s, r) => s + r.s * r.p, 0);
  return ev;
}
function calcExpectedEV() { return calcTotalEVFor(MEM[MI]); }

// ── 슬롯 렌더링 ──
function renderSlots() {
  const sy = window.scrollY;
  const keys = getOptKeys();
  const c = slotCount();
  const mem = MEM[MI];
  const isSet = mem.type === '세트';

  // 세트: 환산치(합산)·평가 셀 미리 계산 (rowspan)
  let setScoreCell = '', setEvalCell = '';
  if (isSet) {
    const allSlots = Array.from({length:c}, (_, i) => getSlot(i));
    const total = allSlots.reduce((s, sl) => s + calcScore(sl.opt, sl.val), 0);
    setScoreCell = `<td id="set-sc" rowspan="${c}" style="text-align:center;vertical-align:middle;font-size:13px;font-weight:600">${total > 0 ? total.toFixed(2) : '<span style="color:var(--txt3);font-weight:400">—</span>'}</td>`;
    if (total > 0) {
      const tier = getEvalTier(mem, total);
      setEvalCell = `<td id="set-ev" rowspan="${c}" style="text-align:center;vertical-align:middle"><span style="font-size:10px;padding:2px 8px;border-radius:4px;background:${tier.bg};color:${tier.color};font-weight:500">${tier.label}</span></td>`;
    } else {
      setEvalCell = `<td id="set-ev" rowspan="${c}" style="text-align:center;vertical-align:middle;color:var(--txt3)">—</td>`;
    }
  }

  let html = '';
  for (let i = 0; i < c; i++) {
    const s = getSlot(i);
    const score = calcScore(s.opt, s.val);
    const range = getOptRange(s.opt);
    const maxAttr = range ? `max="${range.max}"` : '';
    const rangeSpan = `<span class="range-hint" style="font-size:10px;color:var(--txt3);white-space:nowrap;display:inline-block;min-width:40px">${range ? `${range.min}~${range.max}` : ''}</span>`;

    let scoreCell = '', evalCell = '';
    if (!isSet) {
      scoreCell = `<td id="sc-${i}" style="font-size:12px;font-weight:600;text-align:center;white-space:nowrap">${score > 0 ? score.toFixed(2) : '<span style="color:var(--txt3);font-weight:400">—</span>'}</td>`;
      if (score > 0 && s.opt) {
        const tier = getEvalTier(mem, score);
        evalCell = `<td id="ev-${i}" style="text-align:center"><span style="font-size:10px;padding:2px 7px;border-radius:4px;background:${tier.bg};color:${tier.color};font-weight:500">${tier.label}</span></td>`;
      } else {
        evalCell = `<td id="ev-${i}" style="text-align:center"></td>`;
      }
    }

    html += `<tr>
      <td style="color:var(--txt3);font-size:12px">${i+1}</td>
      <td><select class="sel-opt" onchange="onSlotOpt(${i},this.value)">
        <option value="">— 미입력 —</option>
        ${keys.map(k=>`<option value="${k}"${s.opt===k?' selected':''}>${k}</option>`).join('')}
      </select></td>
      <td id="vc-${i}"><div style="display:flex;align-items:center;gap:6px">
        <input class="num-in" type="number" min="0" ${maxAttr} step="0.1" value="${s.val}" placeholder="0"
          oninput="const m=parseFloat(this.max);if(!isNaN(m)&&parseFloat(this.value)>m)this.value=m"
          onchange="onSlotVal(${i},this.value)">
        ${rangeSpan}
      </div></td>
      ${isSet ? (i === 0 ? setScoreCell : '') : scoreCell}
      ${isSet ? (i === 0 ? setEvalCell : '') : evalCell}
    </tr>`;
  }
  document.getElementById('slot-tbody').innerHTML = html;
  renderSlotMetrics();
}

function renderSlotMetrics() {
  const c = slotCount();
  const slots = Array.from({length:c}, (_, i) => getSlot(i));
  const total = slots.reduce((s, sl) => s + calcScore(sl.opt, sl.val), 0);
  const smTotal = document.getElementById('sm-total');
  if (smTotal) smTotal.textContent = total.toFixed(2);
}

function onSlotVal(i, val) {
  setSlot(i, {val});
  const mem = MEM[MI];
  if (mem.type === '세트') {
    const c = slotCount();
    const total = Array.from({length:c}, (_, j) => getSlot(j)).reduce((s, sl) => s + calcScore(sl.opt, sl.val), 0);
    const scEl = document.getElementById('set-sc');
    const evEl = document.getElementById('set-ev');
    if (scEl) scEl.innerHTML = total > 0 ? `<div style="font-size:15px;font-weight:600;letter-spacing:-0.02em">${total.toFixed(2)}</div>` : '<span style="color:var(--txt3)">—</span>';
    if (evEl) {
      if (total > 0) {
        const tier = getEvalTier(mem, total);
        evEl.innerHTML = `<span style="font-size:10px;padding:2px 8px;border-radius:4px;background:${tier.bg};color:${tier.color};font-weight:500">${tier.label}</span>`;
      } else { evEl.innerHTML = '—'; }
    }
  } else {
    const s = getSlot(i);
    const score = calcScore(s.opt, val);
    const scEl = document.getElementById(`sc-${i}`);
    const evEl = document.getElementById(`ev-${i}`);
    if (scEl) scEl.innerHTML = score > 0 ? score.toFixed(2) : '<span style="color:var(--txt3);font-weight:400">—</span>';
    if (evEl) {
      if (score > 0 && s.opt) {
        const tier = getEvalTier(mem, score);
        evEl.innerHTML = `<span style="font-size:10px;padding:2px 7px;border-radius:4px;background:${tier.bg};color:${tier.color};font-weight:500">${tier.label}</span>`;
      } else { evEl.innerHTML = ''; }
    }
  }
  renderSlotMetrics();
}

function onSlotOpt(i, newOpt) {
  const s = getSlot(i);
  let val = s.val;
  if (newOpt) {
    const r = getOptRange(newOpt);
    if (r && val && parseFloat(val) > r.max) val = String(r.max);
  } else { val = ''; }
  setSlot(i, {opt: newOpt, val});

  // 값 셀 업데이트
  const range = newOpt ? getOptRange(newOpt) : null;
  const maxAttr = range ? `max="${range.max}"` : '';
  const rangeSpan = range ? `<span class="range-hint" style="font-size:10px;color:var(--txt3);white-space:nowrap">${range.min}~${range.max}</span>` : '';
  const vcEl = document.getElementById(`vc-${i}`);
  if (vcEl) vcEl.innerHTML = `<div style="display:flex;align-items:center;gap:6px">
    <input class="num-in" type="number" min="0" ${maxAttr} step="0.1" value="${val}" placeholder="0"
      oninput="const m=parseFloat(this.max);if(!isNaN(m)&&parseFloat(this.value)>m)this.value=m"
      onchange="onSlotVal(${i},this.value)">
    ${rangeSpan}
  </div>`;

  // 점수·평가 셀 업데이트
  const mem = MEM[MI];
  const score = calcScore(newOpt, val);
  if (mem.type === '세트') {
    const c = slotCount();
    const total = Array.from({length:c}, (_, j) => getSlot(j)).reduce((s2, sl) => s2 + calcScore(sl.opt, sl.val), 0);
    const scEl = document.getElementById('set-sc');
    const evEl = document.getElementById('set-ev');
    if (scEl) scEl.innerHTML = total > 0 ? `<div style="font-size:15px;font-weight:600;letter-spacing:-0.02em">${total.toFixed(2)}</div>` : '<span style="color:var(--txt3)">—</span>';
    if (evEl) {
      if (total > 0) { const tier = getEvalTier(mem, total); evEl.innerHTML = `<span style="font-size:10px;padding:2px 8px;border-radius:4px;background:${tier.bg};color:${tier.color};font-weight:500">${tier.label}</span>`; }
      else evEl.innerHTML = '—';
    }
  } else {
    const scEl = document.getElementById(`sc-${i}`);
    const evEl = document.getElementById(`ev-${i}`);
    if (scEl) scEl.innerHTML = score > 0 ? score.toFixed(2) : '<span style="color:var(--txt3);font-weight:400">—</span>';
    if (evEl) {
      if (score > 0 && newOpt) { const tier = getEvalTier(mem, score); evEl.innerHTML = `<span style="font-size:10px;padding:2px 7px;border-radius:4px;background:${tier.bg};color:${tier.color};font-weight:500">${tier.label}</span>`; }
      else evEl.innerHTML = '';
    }
  }
  renderSlotMetrics();
}

function clearAll() { const c=slotCount(); for(let i=0;i<c;i++){SD[slotKey(MI,i)]={opt:'',val:''};} saveAll(); renderSlots(); }

// ── 투자 전략 렌더링 ──
function renderStrategy() {
  const m = MEM[MI];
  const c = slotCount();
  const evTotal = calcExpectedEV();
  const infos = Array.from({length:c}, (_, i) => { const s=getSlot(i); return {i,s,cur:calcScore(s.opt,s.val)}; });
  const totalCur = infos.reduce((s,x) => s+x.cur, 0);
  const anyInput = infos.some(x => x.s.opt);

  if (m.type === '세트') {
    const totalGain = evTotal - totalCur;
    const shouldReset = totalGain > 0;
    const evPerSlot = evTotal / SET_SP.reduce((s,r) => s+r.s*r.p, 0);
    document.getElementById('strat-metrics').innerHTML = `
      <div class="mc"><div class="mc-l">현재 총 환산치</div><div class="mc-v">${totalCur.toFixed(2)}</div><div class="mc-s">전체 슬롯 합산</div></div>
      <div class="mc"><div class="mc-l">초기화 기댓값</div><div class="mc-v">${evTotal.toFixed(3)}</div><div class="mc-s">슬롯당 EV × 2.2</div></div>
      <div class="mc"><div class="mc-l">판단</div><div class="mc-v" style="color:${shouldReset?'var(--blue-txt)':'var(--green-txt)'}">${shouldReset?'초기화':'유지'}</div><div class="mc-s">${shouldReset?`+${totalGain.toFixed(3)}`:'기댓값 초과'}</div></div>
      <div class="mc"><div class="mc-l">슬롯당 EV</div><div class="mc-v">${evPerSlot.toFixed(3)}</div><div class="mc-s">참고</div></div>`;
    let html = '';
    if (!anyInput) {
      html = '<div style="padding:16px 0;color:var(--txt2);font-size:13px">슬롯 입력 탭에서 현재 옵션과 값을 먼저 입력해주세요.</div>';
    } else {
      if (shouldReset) {
        const pct = Math.min(100, totalCur/evTotal*100);
        html += `<div class="strat-card reroll"><div style="display:flex;align-items:center;gap:8px;margin-bottom:8px"><span class="badge bb">세트 초기화 추천</span><span style="margin-left:auto;font-size:12px;color:var(--blue-txt)">+${totalGain.toFixed(3)} 기대 이득</span></div><div style="font-size:12px;color:var(--txt2);margin-bottom:6px">현재 합산 <strong style="color:var(--txt)">${totalCur.toFixed(2)}</strong> &lt; 기댓값 <strong style="color:var(--txt)">${evTotal.toFixed(3)}</strong></div><div class="bar-w"><div class="bar-f" style="width:${pct.toFixed(1)}%;background:var(--blue)"></div></div></div>`;
      } else {
        html += `<div class="strat-card locked"><div style="display:flex;align-items:center;gap:8px"><span class="badge bg">세트 유지 추천</span><span style="font-size:12px;color:var(--green-txt);margin-left:8px">합산 ${totalCur.toFixed(2)} ≥ 기댓값 ${evTotal.toFixed(3)}</span></div></div>`;
      }
      html += '<div class="st" style="margin-top:16px;margin-bottom:10px">슬롯별 현황</div>';
      infos.forEach(x => {
        const isGood = x.cur >= evPerSlot;
        html += `<div class="strat-card ${isGood?'keep':'reroll'}" style="margin-bottom:6px"><div style="display:flex;align-items:center;justify-content:space-between;font-size:12px;gap:8px"><span style="color:var(--txt3);flex-shrink:0">슬롯 ${x.i+1}</span><span style="flex:1;color:var(--txt2)">${x.s.opt||'미입력'}${x.s.val?' '+x.s.val:''}</span><span style="color:var(--txt)"><strong>${x.cur.toFixed(2)}</strong><span style="color:var(--txt3)"> / ${evPerSlot.toFixed(2)}</span></span><span class="badge ${isGood?'bg':'bb'}">${isGood?'양호':'미달'}</span></div></div>`;
      });
    }
    document.getElementById('strat-list').innerHTML = html;
    document.getElementById('strat-cost').innerHTML = `
      <div class="row"><span>초기화 비용</span><span>조각 ${m.cp}개 · 결정 ${m.cc}개</span></div>
      <div class="row"><span>기대 슬롯 수</span><span>평균 2.2개</span></div>
      <div class="info-box">세트 메모리얼은 전체 슬롯이 한 번에 초기화됩니다. 현재 전체 합산이 초기화 기댓값보다 낮을 때 초기화를 권장합니다.</div>`;
    return;
  }

  const ev = evTotal;
  const withFlags = infos.map(x => ({...x, ev, gain:ev-x.cur, reroll:(ev-x.cur)>0}));
  const rerolls = withFlags.filter(x => x.reroll).sort((a,b) => b.gain-a.gain);
  const keeps = withFlags.filter(x => !x.reroll);
  const totalAfter = withFlags.reduce((s,x) => s+(x.reroll?ev:x.cur), 0);
  document.getElementById('strat-metrics').innerHTML = `
    <div class="mc"><div class="mc-l">현재 총 환산치</div><div class="mc-v">${totalCur.toFixed(2)}</div><div class="mc-s">전체 슬롯</div></div>
    <div class="mc"><div class="mc-l">목표 총 환산치</div><div class="mc-v" style="color:var(--green-txt)">${totalAfter.toFixed(2)}</div><div class="mc-s">초기화 후 기댓값</div></div>
    <div class="mc"><div class="mc-l">초기화 추천</div><div class="mc-v" style="color:var(--blue-txt)">${rerolls.length}</div><div class="mc-s">슬롯</div></div>
    <div class="mc"><div class="mc-l">유지</div><div class="mc-v" style="color:var(--green-txt)">${keeps.length}</div><div class="mc-s">슬롯</div></div>`;
  let html = '';
  if (!anyInput) {
    html = '<div style="padding:16px 0;color:var(--txt2);font-size:13px">슬롯 입력 탭에서 현재 옵션과 값을 먼저 입력해주세요.</div>';
  } else {
    rerolls.forEach((x, rank) => {
      const pct = Math.min(100, (x.gain/ev)*100);
      html += `<div class="strat-card reroll"><div style="display:flex;align-items:center;gap:6px;margin-bottom:7px"><span class="rank-num">${rank+1}</span><span style="font-weight:500;font-size:13px">슬롯 ${x.i+1}</span><span class="badge bb" style="margin-left:2px">초기화 추천</span><span style="margin-left:auto;font-size:12px;color:var(--blue-txt)">+${x.gain.toFixed(2)}</span></div><div style="font-size:12px;color:var(--txt2);margin-bottom:6px">현재: <strong style="color:var(--txt)">${x.s.opt||'미입력'} ${x.s.val||0}</strong> (${x.cur.toFixed(2)}) → 기댓값 <strong style="color:var(--txt)">${ev.toFixed(3)}</strong></div><div class="bar-w"><div class="bar-f" style="width:${pct.toFixed(1)}%;background:var(--blue)"></div></div></div>`;
    });
    keeps.forEach(x => {
      html += `<div class="strat-card keep"><div style="display:flex;align-items:center;gap:6px;flex-wrap:wrap"><span style="font-size:13px;color:var(--txt2)">슬롯 ${x.i+1}</span><span class="badge bg">유지</span><span style="font-size:12px;color:var(--txt2)">${x.s.opt||'미입력'} ${x.s.val||0} (${x.cur.toFixed(2)}) ≥ ${ev.toFixed(3)}</span></div></div>`;
    });
  }
  document.getElementById('strat-list').innerHTML = html;
  const tp=rerolls.length*m.cp, tc=rerolls.length*m.cc;
  document.getElementById('strat-cost').innerHTML = `
    <div class="row"><span>초기화 대상 슬롯</span><span>${rerolls.length}개</span></div>
    <div class="row"><span>슬롯당 초기화 비용</span><span>조각 ${m.cp}개 · 결정 ${m.cc}개</span></div>
    <div class="row"><span>1회 총 비용</span><span>조각 ${tp}개 · 결정 ${tc}개</span></div>`;
}


// ── 환산치 설정 ──
function renderWeightPage() {
  const memEl = document.getElementById('wp-memorial-grid');
  const artEl = document.getElementById('wp-shared-grid');
  if (memEl) memEl.innerHTML = Object.keys(WD).filter(k=>k!=='꽝').map(k=>`
    <div class="opt-item"><label>${k}</label>
    <input type="number" step="0.0001" value="${W[k]??0}"
      onchange="W['${k}']=parseFloat(this.value)||0;saveAll()"></div>`).join('');
  if (artEl) artEl.innerHTML = Object.keys(WD2_DEFAULT).map(k=>`
    <div class="opt-item"><label>${k}</label>
    <input type="number" step="0.0001" value="${WD2[k]??0}"
      onchange="WD2['${k}']=parseFloat(this.value)||0;saveAll()"></div>`).join('');
}
function renderWeights() { renderWeightPage(); }
function resetWeights() { W={...WD}; WD2={...WD2_DEFAULT}; saveAll(); renderWeightPage(); }

// ── 전체 환산치 합산 ──
function renderGlobalSummary() {
  let total = 0, filled = 0;
  MEM.forEach((mem, mi) => {
    const c = mem.type === '개별' ? mem.slots : 4;
    Array.from({length:c}, (_, si) => SD[`${mi}_${si}`] || {opt:'',val:'',locked:false}).forEach(s => {
      if (s.opt) { total += calcScore(s.opt, s.val); filled++; }
    });
  });
  document.getElementById('summary-total').textContent = total.toFixed(2);
  document.getElementById('summary-sub').textContent = filled ? `입력된 슬롯 ${filled}개 합산` : '입력된 슬롯 없음';
}

// ── 전체 투자전략 ──
function renderGlobalStrategy() {
  const sortBy = document.getElementById('global-sort')?.value||'cpPer0_1';
  const showEmpty = document.getElementById('global-show-empty')?.checked||false;
  const items = [];
  MEM.forEach((mem,mi) => {
    const c = mem.type==='개별'?mem.slots:4;
    const ev = calcTotalEVFor(mem);
    if (mem.type==='세트') {
      const slots = Array.from({length:c},(_,si)=>SD[`${mi}_${si}`]||{opt:'',val:'',locked:false});
      const totalCur = slots.reduce((s,sl)=>s+calcScore(sl.opt,sl.val),0);
      const hasInput = slots.some(sl=>sl.opt && sl.opt !== '꽝');
      if (!hasInput&&!showEmpty) return;
      const gain=ev-totalCur;
      const maxTotal = 4 * calcAbsMaxScore(mem);
      const remaining=Math.max(0,maxTotal-totalCur);
      const {pBeat:pBeatSet,eGain:eGainSet}=calcSetMetricsDet(mem,totalCur,mi);
      const expectedRolls=pBeatSet>0?Math.round(1/pBeatSet):null;
      const cpPer0_1=eGainSet>0?mem.cp/eGainSet*0.1:Infinity;
      const ccPer0_1=eGainSet>0?mem.cc/eGainSet*0.1:Infinity;
      items.push({mi,mem,isSet:true,cur:totalCur,ev,gain,hasInput,label:mem.name,slotLabel:'세트',remaining,cpPer0_1,ccPer0_1,expectedRolls});
    } else {
      for (let si=0;si<c;si++) {
        const s=SD[`${mi}_${si}`]||{opt:'',val:'',locked:false};
        if ((!s.opt || s.opt === '꽝') && !showEmpty) continue;
        const cur=calcScore(s.opt,s.val), gain=ev-cur;
        const remaining=calcRemainingPotential(mem,cur);
        const pBeat=calcProbBeatScore(mem,cur);
        const expectedRolls=pBeat>0?Math.round(1/pBeat):null;
        const eGain=calcExpectedGainPerRoll(mem,cur);
        const cpPer0_1=eGain>0?mem.cp/eGain*0.1:Infinity;
        const ccPer0_1=eGain>0?mem.cc/eGain*0.1:Infinity;
        items.push({mi,mem,si,isSet:false,s,cur,ev,gain,hasInput:!!s.opt&&s.opt!=='꽝',label:mem.name,slotLabel:`슬롯 ${si+1}`,remaining,cpPer0_1,ccPer0_1,gainPerCc:gain/mem.cc,gainPerCp:gain/mem.cp,expectedRolls});
      }
    }
  });
  renderGlobalSummary();
  if (!items.length) {
    document.getElementById('global-list').innerHTML='<div style="padding:20px 0;color:var(--txt2);font-size:12px;text-align:center;line-height:2">입력된 슬롯 데이터가 없습니다.<br>메모리얼을 선택해 슬롯을 입력하거나<br>"미입력 포함"을 체크하세요.</div>';
    return;
  }
  const sfMain = sortBy === 'remaining'
    ? (a,b) => b.remaining - a.remaining
    : sortBy === 'expectedRolls'
    ? (a,b) => { const ar = a.expectedRolls ?? Infinity, br = b.expectedRolls ?? Infinity; return ar !== br ? ar - br : b.remaining - a.remaining; }
    : sortBy === 'ccPer0_1'
    ? (a,b) => { const d = a.ccPer0_1 - b.ccPer0_1; return Math.abs(d) > 1e-9 ? d : b.remaining - a.remaining; }
    : (a,b) => { const d = a.cpPer0_1 - b.cpPer0_1; return Math.abs(d) > 1e-9 ? d : b.remaining - a.remaining; };

  // 최대치 미달인 슬롯 전부 효율 순으로 — gain > 0 여부 무관
  const improvable = items.filter(x => x.remaining > 0).sort(sfMain);
  const maxed = items.filter(x => x.remaining <= 0);

  let html = '';

  if (improvable.length) {
    improvable.forEach((x, i) => {
      const rank = i + 1;
      const maxScore = x.cur + x.remaining;
      const pct = maxScore > 0 ? Math.min(100, x.cur / maxScore * 100) : 0;
      const stat = sortBy === 'ccPer0_1'
        ? `결정 ${x.ccPer0_1.toFixed(3)}개당 0.1환산치`
        : `조각 ${x.cpPer0_1.toFixed(3)}개당 0.1환산치`;
      const curTxt = x.isSet ? `합산 ${x.cur.toFixed(2)}`
                   : (x.s?.opt ? `${x.s.opt} ${x.s.val} (${x.cur.toFixed(2)})` : '미입력');
      const rollSpan = x.expectedRolls != null
        ? `<span style="color:var(--txt3)">개선 기대 ~${x.expectedRolls.toLocaleString()}회</span>` : '';
      html += `<div class="strat-card reroll" style="margin-bottom:7px">
        <div style="display:flex;align-items:center;gap:5px;margin-bottom:5px;flex-wrap:wrap">
          <span class="rank-num">${rank}</span>
          <span style="font-weight:500;font-size:12px">${x.label}</span>
          <span style="font-size:10px;color:var(--txt3);background:var(--bg4);padding:2px 7px;border-radius:4px">${x.slotLabel}</span>
          <span class="badge ${x.isSet?'bw':'bb'}">${x.mem.type}</span>
          <span style="margin-left:auto;font-size:11px;color:var(--blue-txt);font-weight:500">${stat}</span>
        </div>
        <div style="display:flex;gap:10px;font-size:11px;color:var(--txt2);flex-wrap:wrap;margin-bottom:4px">
          <span>현재: <strong style="color:var(--txt)">${curTxt}</strong></span>
          <span>잔여: <strong style="color:var(--amber-txt)">+${x.remaining.toFixed(2)}</strong></span>
          <span style="color:var(--txt3)">조각 ${x.mem.cp} · 결정 ${x.mem.cc}</span>
        </div>
        <div style="display:flex;gap:12px;font-size:11px;flex-wrap:wrap;margin-bottom:6px">
          <span style="color:var(--amber-txt)">잔여 +${x.remaining.toFixed(2)}</span>
          ${rollSpan}
        </div>
        <div class="bar-w"><div class="bar-f" style="width:${pct.toFixed(1)}%;background:var(--blue)"></div></div>
      </div>`;
    });
  } else {
    html += `<div style="padding:14px 0;font-size:12px;color:var(--txt2)">개선 가능한 슬롯이 없습니다.</div>`;
  }

  document.getElementById('global-list').innerHTML = html;
}

// ── 메모리얼 네비게이션 ──
function getGroups() {
  const order=[], map={};
  MEM.forEach((m,i)=>{ const bn=m.name.replace(' (세트)',''); if(!map[bn]){map[bn]=[];order.push(bn);} map[bn].push(i); });
  return order.map(n=>({name:n,indices:map[n]}));
}
function renderMemNav() {
  const groups=getGroups(), curBase=MEM[MI].name.replace(' (세트)','');
  document.getElementById('mem-groups').innerHTML=groups.map(g=>`<button class="mem-btn${g.name===curBase?' on':''}" onclick="selectGroup('${g.name}')">${g.name}</button>`).join('');
  const cg=groups.find(g=>g.name===curBase);
  document.getElementById('mem-types').innerHTML=(cg&&cg.indices.length>1)?cg.indices.map(i=>`<button class="mem-btn sub${i===MI?' on':''}" onclick="selectMem(${i})">${MEM[i].type}</button>`).join(''):'';
}
function selectGroup(name) {
  const g=getGroups().find(g=>g.name===name);
  if(!g) return;
  const curBase=MEM[MI].name.replace(' (세트)','');
  if(g.name!==curBase||!g.indices.includes(MI)) MI=g.indices[0];
  saveState(); renderAll();
}
function selectMem(i) { MI=i; saveState(); renderAll(); }

// ── 탭 전환 ──
function setLeftTab(t, el) {
  leftTab=t;
  document.getElementById('left-global').style.display=t==='global'?'':'none';
  document.querySelectorAll('.panel-left .tab').forEach(b=>b.classList.remove('on'));
  if (el) el.classList.add('on');
  if(t==='global') renderGlobalStrategy();
}
function setTab(t, el) {
  curTab=t;
  ['slots','strategy'].forEach(id=>document.getElementById('tab-'+id).style.display=id===t?'':'none');
  document.querySelectorAll('.panel-right .tab').forEach(b=>b.classList.remove('on'));
  el.classList.add('on');
  if(t==='slots') renderSlots();
  else if(t==='strategy') renderStrategy();
}
function renderAll() {
  const m=MEM[MI];
  renderMemNav();
  document.getElementById('type-badge').textContent=m.type;
  document.getElementById('cost-lbl').textContent=`초기화: 조각 ${m.cp}개 · 결정 ${m.cc}개`;
  if(curTab==='slots') renderSlots();
  else if(curTab==='strategy') renderStrategy();
}

// ── 페이지 탭 전환 ──
function setPageTab(t, el) {
  curPageTab = t;
  ['memorial','artifact','weight'].forEach(id => {
    const p = document.getElementById('page-' + id);
    if (p) p.style.display = id === t ? '' : 'none';
  });
  document.querySelectorAll('.page-tab').forEach(b => b.classList.remove('on'));
  el.classList.add('on');
  document.querySelector('.container').style.maxWidth = t === 'artifact' ? '1600px' : '';
  if (t === 'artifact') renderArtPage();
  else if (t === 'weight') renderWeightPage();
}

// ── 성물석 계산 ──
function gw2(k) { return WD2[k] ?? 0; }

function getArtWeight(ai, optKey) {
  const w = gw2(optKey);
  if (!w) return 0;
  const art = ARTIFACTS[ai];
  if (!art.syn) return w;
  const synVal = parseFloat(ART_SD.ded[ai][art.syn.di]) || 0;
  if (synVal > 0 && art.syn.affects.includes(optKey)) return w * (1 + synVal * 0.5);
  return w;
}

function getSynMult(ai, optKey) {
  const art = ARTIFACTS[ai];
  if (!art.syn || !art.syn.affects.includes(optKey)) return 1;
  const synVal = parseFloat(ART_SD.ded[ai][art.syn.di]) || 0;
  return synVal > 0 ? 1 + synVal * 0.5 : 1;
}

function calcArtUsage(dungeonSec, startIdx) {
  const total = 5 + Math.floor(dungeonSec / 125);
  const u = [0,0,0,0,0,0];
  for (let i = 0; i < total; i++) u[(startIdx + i) % 6]++;
  return u;
}

function calcStoneFullScore(opts, ai, T, useCnt) {
  return opts.reduce((s, ov) => {
    const v = parseFloat(ov.val || 0);
    if (!v || !ov.opt) return s;
    const wg = gw2(ov.opt);
    const wa = getArtWeight(ai, ov.opt);
    return s + v * (wg * T + wa * 50 * useCnt * 30);
  }, 0);
}

function calcStoneDisplayScore(opts) {
  return opts.reduce((s, ov) => s + parseFloat(ov.val || 0) * gw2(ov.opt), 0);
}

function computeRanking() {
  const T = artDungeonMin * 60;
  const usage = calcArtUsage(T, artStartIdx);
  const newOpts = ART_NEW.filter(ov => ov.opt && parseFloat(ov.val || 0) > 0);
  if (!newOpts.length) return [];
  const res = [];
  for (let ai = 0; ai < 6; ai++) {
    for (let si = 0; si < 2; si++) {
      const oldOpts = ART_SD.shared[ai][si].filter(ov => ov.opt && parseFloat(ov.val || 0) > 0);
      const gain = calcStoneFullScore(newOpts, ai, T, usage[ai]) - calcStoneFullScore(oldOpts, ai, T, usage[ai]);
      res.push({ai, si, gain});
    }
  }
  res.sort((a, b) => b.gain - a.gain);
  return res;
}

// ── 성물석 렌더링 ──
function onArtSettingChange() {
  const startEl = document.getElementById('art-start');
  const minEl = document.getElementById('art-dungeon-min');
  if (startEl) artStartIdx = parseInt(startEl.value) || 0;
  if (minEl) artDungeonMin = Math.max(1, parseInt(minEl.value) || 10);
  saveAll();
  renderArtGrid();
}

function renderArtGrid() {
  const T = artDungeonMin * 60;
  const usage = calcArtUsage(T, artStartIdx);
  const ranking = computeRanking();
  const keys = Object.keys(WD2_DEFAULT);
  const r1 = ranking[0] ?? null;
  const r2 = ranking[1] ?? null;
  const hasNew = ART_NEW.some(ov => ov.opt && parseFloat(ov.val||0) > 0);

  const totalUse = 5 + Math.floor(T / 125);
  const usageEl = document.getElementById('art-usage-display');
  if (usageEl) usageEl.textContent = `총 ${totalUse}회 사용 (충전 공유)`;

  // ── NEW 카드 HTML ──
  let newOptsHtml = `<div style="display:flex;justify-content:flex-end;margin-bottom:7px">
    <button class="lock-btn" style="font-size:10px;padding:2px 8px" onclick="resetArtNew()">초기화</button>
  </div>`;
  for (let j = 0; j < 4; j++) {
    const ov = ART_NEW[j];
    newOptsHtml += `<div style="display:flex;gap:4px;align-items:center;margin-bottom:5px">
      <select class="sel-opt" style="flex:1;min-width:0;font-size:11px" onchange="ART_NEW[${j}].opt=this.value;saveAll();renderArtGrid()">
        <option value="">—</option>
        ${keys.map(k => `<option value="${k}"${ov.opt===k?' selected':''}>${k}</option>`).join('')}
      </select>
      <input class="num-in" type="number" min="0" max="${WD2_MAX[ov.opt]||''}" step="1" value="${ov.val}" placeholder="0" style="width:62px;font-size:11px"
        oninput="const m=parseFloat(this.max);if(!isNaN(m)&&parseFloat(this.value)>m)this.value=m"
        onchange="ART_NEW[${j}].val=this.value;saveAll();renderArtGrid()">
    </div>`;
  }
  const newScore = calcStoneDisplayScore(ART_NEW);
  newOptsHtml += `<div style="padding-top:8px;border-top:1px solid var(--border);display:flex;justify-content:space-between;align-items:center;margin-top:3px;margin-bottom:10px">
    <span style="font-size:10px;color:var(--txt3)">환산치</span>
    <span style="font-size:16px;font-weight:600;color:var(--red-txt)">${newScore>0?newScore.toFixed(3):'—'}</span>
  </div>
  <div style="display:flex;gap:6px">
    <button id="btn-replace-1" class="lock-btn" style="flex:1;color:var(--amber-txt);border-color:rgba(251,191,36,0.3)" onclick="execReplace(0)" ${!hasNew||!r1?'disabled':''}>1순위 교체</button>
    <button id="btn-replace-2" class="lock-btn" style="flex:1" onclick="execReplace(1)" ${!hasNew||!r2?'disabled':''}>2순위 교체</button>
  </div>`;

  // ── 테이블 ──
  let html = `<table style="border-collapse:separate;border-spacing:6px 0;width:100%;table-layout:fixed">`;

  // 헤더 행
  html += `<tr>
    <th style="text-align:center;padding-bottom:10px;vertical-align:bottom;width:17.5%">
      <span style="font-size:15px;font-weight:800;color:var(--red-txt);letter-spacing:.06em">NEW</span>
    </th>`;
  ARTIFACTS.forEach((art, ai) => {
    html += `<th style="text-align:center;padding-bottom:10px;vertical-align:bottom;width:13.75%">
      <div style="font-size:12px;font-weight:600">${art.name}</div>
      <div style="font-size:10px;color:var(--txt3);margin-top:1px">${usage[ai]}회 사용</div>
    </th>`;
  });
  html += `</tr>`;

  // 전용석 행 (NEW 카드 rowspan=3)
  html += `<tr>
    <td rowspan="3" style="vertical-align:top;padding-bottom:6px">
      <div style="background:rgba(239,68,68,0.05);border:1px solid rgba(239,68,68,0.3);border-radius:var(--rad-lg);padding:12px">
        ${newOptsHtml}
      </div>
    </td>`;
  ARTIFACTS.forEach((art, ai) => {
    let dedHtml = `<div style="background:rgba(245,158,11,0.07);border:1px solid rgba(245,158,11,0.2);border-radius:var(--rad);padding:7px">
      <div style="font-size:9px;font-weight:600;color:rgba(245,158,11,0.65);text-transform:uppercase;letter-spacing:.06em;margin-bottom:6px">전용석</div>`;
    art.ded.forEach((d, di) => {
      const val = ART_SD.ded[ai][di];
      dedHtml += `<div style="margin-bottom:5px">
        <div style="font-size:9px;color:var(--txt2);margin-bottom:3px">${d.k} <span style="color:var(--txt3)">${d.mn}~${d.mx}</span></div>
        <input class="num-in" type="number" min="${d.mn}" max="${d.mx}" step="0.1" value="${val}" placeholder="0" style="width:100%;font-size:11px"
          oninput="const m=parseFloat(this.max);if(!isNaN(m)&&parseFloat(this.value)>m)this.value=m"
          onchange="ART_SD.ded[${ai}][${di}]=this.value;saveAll();renderArtGrid()">
      </div>`;
    });
    dedHtml += `</div>`;
    html += `<td style="vertical-align:top;padding-bottom:6px">${dedHtml}</td>`;
  });
  html += `</tr>`;

  // 공용석 행 2개
  for (let si = 0; si < 2; si++) {
    html += `<tr>`;
    ARTIFACTS.forEach((art, ai) => {
      const isR1 = r1 && r1.ai===ai && r1.si===si;
      const isR2 = r2 && r2.ai===ai && r2.si===si;
      const border = isR1 ? '2px solid #fbbf24' : isR2 ? '2px solid #94a3b8' : '1px solid rgba(59,130,246,0.2)';
      const bg     = isR1 ? 'rgba(251,191,36,0.07)' : isR2 ? 'rgba(148,163,184,0.06)' : 'rgba(59,130,246,0.05)';
      const shadow = isR1 ? '0 0 14px rgba(251,191,36,0.35)' : isR2 ? '0 0 8px rgba(148,163,184,0.25)' : '';
      const slotOpts = ART_SD.shared[ai][si];
      const displayScore = slotOpts.reduce((s,ov) => s+parseFloat(ov.val||0)*getArtWeight(ai,ov.opt), 0);
      const hasSyn = slotOpts.some(ov => ov.opt && getSynMult(ai,ov.opt)>1);
      const rankBadge = isR1
        ? `<span style="font-size:9px;padding:1px 5px;border-radius:3px;background:#fbbf24;color:#000;font-weight:700">1순위</span>`
        : isR2
        ? `<span style="font-size:9px;padding:1px 5px;border-radius:3px;background:#94a3b8;color:#000;font-weight:700">2순위</span>`
        : '';
      const newDS = ART_NEW.reduce((s,ov) => s+parseFloat(ov.val||0)*getArtWeight(ai,ov.opt), 0);
      const gain = newDS - displayScore;
      const gainTxt = (isR1||isR2) && gain!==0
        ? `<span style="font-size:9px;color:${gain>0?'var(--green-txt)':'var(--red-txt)'}">${gain>0?'+':''}${gain.toFixed(3)}</span>`
        : '';
      let sharedHtml = `<div style="background:${bg};border:${border};border-radius:var(--rad);padding:7px;box-shadow:${shadow};transition:all .25s">
        <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:6px;flex-wrap:wrap;gap:3px">
          <span style="font-size:9px;font-weight:600;color:rgba(59,130,246,0.65);text-transform:uppercase;letter-spacing:.06em">공용석 ${si+1}</span>
          <div style="display:flex;align-items:center;gap:4px">
            ${hasSyn?`<span style="font-size:9px;color:var(--amber-txt)">★</span>`:''}
            <span style="font-size:11px;font-weight:600">${displayScore>0?displayScore.toFixed(3):'—'}</span>
            ${rankBadge}${gainTxt}
          </div>
        </div>`;
      for (let j = 0; j < 4; j++) {
        const ov = slotOpts[j];
        sharedHtml += `<div style="display:flex;gap:3px;align-items:center;margin-bottom:3px">
          <select class="sel-opt" style="flex:1;min-width:0;font-size:10px;padding:3px 4px"
            onchange="ART_SD.shared[${ai}][${si}][${j}].opt=this.value;saveAll();renderArtGrid()">
            <option value="">—</option>
            ${keys.map(k=>`<option value="${k}"${ov.opt===k?' selected':''}>${k}</option>`).join('')}
          </select>
          <input class="num-in" type="number" min="0" max="${WD2_MAX[ov.opt]||''}" step="1" value="${ov.val}" placeholder="0" style="width:52px;font-size:10px"
            oninput="const m=parseFloat(this.max);if(!isNaN(m)&&parseFloat(this.value)>m)this.value=m"
            onchange="ART_SD.shared[${ai}][${si}][${j}].val=this.value;saveAll();renderArtGrid()">
        </div>`;
      }
      sharedHtml += `</div>`;
      html += `<td style="vertical-align:top;padding-bottom:6px">${sharedHtml}</td>`;
    });
    html += `</tr>`;
  }

  html += `</table>`;
  const gridEl = document.getElementById('art-grid');
  if (gridEl) gridEl.innerHTML = html;
}

function resetArtNew() {
  ART_NEW = initArtNew();
  saveAll();
  renderArtGrid();
}

function resetArtAll() {
  if (!confirm('성물석 데이터를 모두 초기화합니다. 계속하시겠습니까?')) return;
  ART_SD = initArtSD();
  ART_NEW = initArtNew();
  saveAll();
  renderArtGrid();
}

function execReplace(rank) {
  const ranking = computeRanking();
  if (ranking.length <= rank) return;
  const {ai, si} = ranking[rank];
  const artName = ARTIFACTS[ai].name;
  if (!confirm(`${artName} 공용석 ${si + 1}번을 교체할 공용석으로 교체합니다.`)) return;
  ART_SD.shared[ai][si] = ART_NEW.map(ov => ({...ov}));
  ART_NEW = initArtNew();
  saveAll();
  renderArtGrid();
}

function renderArtPage() {
  const startEl = document.getElementById('art-start');
  const minEl = document.getElementById('art-dungeon-min');
  if (startEl) startEl.value = artStartIdx;
  if (minEl) minEl.value = artDungeonMin;
  renderArtGrid();
}

function init() {
  loadAll();
  renderAll();
  renderGlobalStrategy();
}
init();
</script>
</body>
</html>
