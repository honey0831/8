<!DOCTYPE html>
<html lang="zh-CN">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>班级全能管理系统 - 终极版</title>
<style>
:root{--blue:#2563eb;--blue-d:#1d4ed8;--blue-l:#eff6ff;--bg:#f8fafc;--card:#fff;--line:#e2e8f0;--text:#0f172a;--muted:#64748b;--green:#10b981;--red:#ef4444;--shadow:0 4px 20px rgba(37,99,235,.06)}
*{margin:0;padding:0;box-sizing:border-box}
body{font-family:"PingFang SC","Microsoft YaHei",system-ui,sans-serif;background:var(--bg);color:var(--text);font-size:14px;line-height:1.6;-webkit-font-smoothing:antialiased}
button{font-family:inherit;cursor:pointer;border:none;background:none;font-size:14px;transition:all .2s}
input,select,textarea{font-family:inherit;font-size:15px;color:var(--text);outline:none}
.hidden{display:none!important}

/* 登录页 */
.login-wrap{min-height:100vh;display:flex;align-items:center;justify-content:center;background:linear-gradient(135deg,#eff6ff,#fff);padding:24px 16px}
.login-card{width:100%;max-width:420px;background:#fff;border-radius:20px;padding:36px 32px;box-shadow:0 12px 50px rgba(37,99,235,.1);border:1px solid #f1f5f9}
.login-title{font-size:24px;font-weight:700;margin-bottom:8px;display:flex;align-items:center;gap:12px;color:var(--blue)}
.login-sub{color:var(--muted);font-size:13.5px;margin-bottom:28px}
.field{margin-bottom:18px}
.field label{display:block;font-size:13.5px;color:var(--muted);margin-bottom:8px}
.field input{width:100%;height:48px;border:1.5px solid var(--line);border-radius:12px;padding:0 16px;background:#f8fafc}
.field input:focus{border-color:var(--blue);background:#fff;box-shadow:0 0 0 4px rgba(37,99,235,.1)}
.login-btn{width:100%;height:48px;border-radius:12px;background:var(--blue);color:#fff;font-size:16px;font-weight:600;margin-top:10px;box-shadow:0 6px 16px rgba(37,99,235,.3)}
.login-switch{text-align:center;margin-top:20px;font-size:13.5px;color:var(--muted)}
.login-switch b{color:var(--blue);cursor:pointer}

/* 欢迎遮罩（全屏覆盖） */
.welcome-mask{position:fixed;inset:0;z-index:9000;display:flex;align-items:center;justify-content:center;background:rgba(15,23,42,.55);backdrop-filter:blur(8px);opacity:0;pointer-events:none;transition:opacity .35s ease;padding:24px}
.welcome-mask.show{opacity:1;pointer-events:auto}
.welcome-card{width:min(600px,92vw);max-height:86vh;background:#fff;border-radius:26px;padding:52px 40px;text-align:center;box-shadow:0 30px 90px rgba(0,0,0,.28);transform:scale(.88);transition:transform .45s cubic-bezier(0.175,0.885,0.32,1.275)}
.welcome-mask.show .welcome-card{transform:scale(1)}
.welcome-emoji{font-size:52px;line-height:1;margin-bottom:18px}
.welcome-title{font-size:30px;font-weight:800;letter-spacing:3px;color:#0f172a;margin-bottom:14px}
.welcome-line{width:60px;height:3px;background:linear-gradient(90deg,#60a5fa,#2563eb);border-radius:2px;margin:0 auto 18px}
.welcome-sub{font-size:15px;font-weight:500;color:#64748b;letter-spacing:6px}
.welcome-tip{margin-top:26px;font-size:13px;color:#94a3b8}

/* 顶部栏 */
.topbar{min-height:64px;background:#fff;border-bottom:1px solid var(--line);display:flex;align-items:center;justify-content:space-between;padding:10px 24px;position:sticky;top:0;z-index:20;gap:12px;flex-wrap:wrap}
.brand{display:flex;align-items:center;gap:12px}
.brand .mark{width:38px;height:38px;border-radius:10px;background:linear-gradient(135deg,#60a5fa,#2563eb);display:flex;align-items:center;justify-content:center;box-shadow:0 4px 12px rgba(37,99,235,.3)}
.brand .mark svg{width:22px;height:22px;fill:#fff}
.brand-txt .t{font-size:19px;font-weight:800;color:var(--text);letter-spacing:.5px}
.brand-txt .s{font-size:12.5px;color:var(--muted);display:flex;align-items:center;gap:6px;margin-top:2px}
.dot{width:8px;height:8px;border-radius:50%;background:var(--green);display:inline-block;box-shadow:0 0 8px rgba(16,185,129,.5)}
.top-actions{display:flex;gap:10px;flex-wrap:wrap}
.tbtn{height:38px;padding:0 16px;border-radius:10px;color:#fff;font-size:13.5px;font-weight:600;display:inline-flex;align-items:center;gap:6px;box-shadow:0 2px 6px rgba(0,0,0,.05)}
.tbtn:hover{filter:brightness(1.05);transform:translateY(-2px);box-shadow:0 6px 16px rgba(0,0,0,.1)}
.tbtn.sync{background:#3b82f6}.tbtn.export{background:#10b981}.tbtn.profile{background:#f1f5f9;color:#475569}
.tbtn.lucky{background:linear-gradient(135deg,#8b5cf6,#6366f1)}
.tbtn.notice{background:#f59e0b}.tbtn.timer{background:#0ea5e9}

/* 布局与侧边栏 */
.layout{display:flex;gap:20px;padding:24px;max-width:1600px;margin:0 auto;align-items:flex-start}
.sidebar{width:280px;flex:none;display:flex;flex-direction:column;gap:16px;position:sticky;top:88px}
.card{background:var(--card);border-radius:16px;box-shadow:var(--shadow);border:1px solid #f1f5f9;overflow:hidden}
.card-hd{padding:16px 20px;border-bottom:1px solid #f1f5f9;font-size:15px;font-weight:700;color:#1e293b;display:flex;justify-content:space-between;align-items:center}
.card-bd{padding:20px}
.stat-row{display:grid;grid-template-columns:1fr 1fr;gap:12px;padding:16px}
.stat{background:#f8fafc;border-radius:12px;padding:16px;border:1px solid #e2e8f0;text-align:center}
.stat .k{font-size:13px;color:var(--muted);font-weight:500;margin-bottom:4px}
.stat .v{font-size:28px;font-weight:800;color:var(--blue)}
.stat.alt .v{color:var(--green)}
.today-row{display:flex;justify-content:space-between;padding:0 4px 12px;font-size:13px;color:#64748b}
.today-row b{color:#2563eb;font-weight:700}

/* 主区域 */
.main{flex:1;min-width:0}
.tabs{display:flex;background:#fff;border-radius:16px;padding:6px;gap:6px;box-shadow:var(--shadow);margin-bottom:20px;overflow-x:auto}
.tab{flex:1;min-width:100px;height:44px;border-radius:12px;font-size:14.5px;font-weight:600;color:#64748b;display:flex;align-items:center;justify-content:center;gap:6px;white-space:nowrap}
.tab:hover{background:#f8fafc;color:var(--blue)}
.tab.on{background:var(--blue);color:#fff;box-shadow:0 4px 12px rgba(37,99,235,.25)}
.panel{background:#fff;border-radius:16px;box-shadow:var(--shadow);padding:24px;border:1px solid #f1f5f9}

/* 公告横幅 */
.notice-bar{display:flex;align-items:flex-start;gap:10px;background:#fffbeb;border:1px solid #fde68a;border-radius:12px;padding:12px 16px;margin-bottom:16px;font-size:14px;color:#92400e}
.notice-bar .ico{font-size:16px;line-height:1.4}

/* 表格美化 */
.tbl-scroll{width:100%;overflow-x:auto}
table{width:100%;border-collapse:collapse;min-width:700px}
th{text-align:left;font-size:13px;color:#64748b;font-weight:600;padding:14px 16px;background:#f8fafc;white-space:nowrap;border-bottom:2px solid #e2e8f0}
td{padding:14px 16px;border-bottom:1px solid #f1f5f9;font-size:14px;vertical-align:middle}
tr:hover td{background:#f8fafc}

/* 组件样式 */
.name-cell{display:flex;align-items:center;gap:10px}
.avatar{width:32px;height:32px;border-radius:50%;flex:none;display:flex;align-items:center;justify-content:center;font-size:14px;font-weight:600;color:#fff;background:#cbd5e1}
.avatar.g1{background:#60a5fa}.avatar.g2{background:#34d399}.avatar.g3{background:#f87171}.avatar.g4{background:#a78bfa}.avatar.g5{background:#fbbf24}.avatar.g6{background:#38bdf8}.avatar.g7{background:#4ade80}.avatar.g8{background:#fb7185}.avatar.g9{background:#94a3b8}
.score-num{font-weight:700;color:var(--blue);font-size:16px}
.tag-group{display:inline-block;padding:4px 10px;border-radius:6px;background:var(--blue-l);color:var(--blue);font-size:12.5px;font-weight:500}
.acts{display:flex;gap:6px;flex-wrap:wrap}
.act{height:30px;padding:0 10px;border-radius:6px;font-size:13px;font-weight:500;display:inline-flex;align-items:center}
.act.plus{background:#ecfdf5;color:#059669}.act.minus{background:#fef2f2;color:#dc2626}.act.plain{background:#f1f5f9;color:#475569}.act.del{background:#fef2f2;color:#dc2626}
.act.edit{background:#eef2ff;color:#4f46e5}
.text-red{color:#ef4444!important;font-weight:700}
.empty{padding:40px 16px;text-align:center;color:#94a3b8;font-size:14px}

/* 弹窗与提示 */
.modal-back{position:fixed;inset:0;background:rgba(15,23,42,.4);z-index:100;display:flex;align-items:flex-start;justify-content:center;padding:60px 16px 30px;overflow-y:auto;backdrop-filter:blur(3px)}
.modal{width:100%;max-width:480px;background:#fff;border-radius:16px;box-shadow:0 24px 60px rgba(15,23,42,.2);overflow:hidden;animation:popIn .3s cubic-bezier(0.175, 0.885, 0.32, 1.275)}
@keyframes popIn{0%{transform:scale(.95);opacity:0}100%{transform:scale(1);opacity:1}}
.m-hd{display:flex;align-items:center;justify-content:space-between;padding:20px 24px 10px}
.m-hd h3{font-size:18px;font-weight:700}
.m-close{width:32px;height:32px;border-radius:8px;color:#94a3b8;font-size:22px;display:flex;align-items:center;justify-content:center;background:#f1f5f9;cursor:pointer}
.m-bd{padding:10px 24px}
.m-ft{display:flex;justify-content:flex-end;gap:12px;padding:20px 24px 24px;flex-wrap:wrap}
.btn-line{height:40px;padding:0 24px;border-radius:10px;background:#f1f5f9;color:#475569;font-size:14.5px;font-weight:500;cursor:pointer}
.btn-solid{height:40px;padding:0 28px;border-radius:10px;background:var(--blue);color:#fff;font-size:14.5px;font-weight:600;cursor:pointer}
.btn-danger{background:#fff6f6;color:#e0454c}
.hist-list{max-height:400px;overflow-y:auto;padding-right:6px}
.hist-item{display:flex;justify-content:space-between;gap:12px;padding:14px 0;border-bottom:1px solid #f1f5f9;align-items:center}
.h-num.up{color:var(--green);font-weight:700}.h-num.down{color:var(--red);font-weight:700}

/* 表单通用（弹窗内） */
.f{margin-bottom:12px}
.f label{display:block;font-size:13px;color:#64748b;margin-bottom:6px}
.f input,.f select{width:100%;height:40px;border:1px solid #e2e8f0;border-radius:8px;padding:0 12px;background:#fff}
.f input:focus,.f select:focus{border-color:var(--blue)}

/* 倒计时浮层与提示 */
.timer-overlay{position:fixed;inset:0;background:#fff;z-index:500;display:flex;flex-direction:column;align-items:center;justify-content:center}
.timer-time{font-size:140px;font-weight:800;font-family:monospace;color:var(--blue);margin-bottom:40px;letter-spacing:-4px}
.timer-btn{height:44px;padding:0 18px;border-radius:10px;background:#f1f5f9;color:#475569;font-weight:600;font-size:15px}
.toast{position:fixed;left:50%;bottom:40px;transform:translateX(-50%) translateY(10px);background:rgba(15,23,42,.9);color:#fff;padding:12px 24px;border-radius:12px;font-size:14px;opacity:0;transition:.3s;z-index:9999;pointer-events:none;max-width:80vw;text-align:center}
.toast.show{opacity:1;transform:translateX(-50%) translateY(0)}
/* 作业白板 */
.hw-board{display:grid;grid-template-columns:repeat(auto-fill,minmax(280px,1fr));gap:16px}
.hw-card{background:#fff;border-radius:12px;padding:20px;box-shadow:0 4px 12px rgba(0,0,0,.05);border:1px solid #f1f5f9;position:relative;padding-bottom:44px}
.hw-card .hw-sub{font-size:16px;font-weight:700;color:#1e293b;margin-bottom:8px;display:flex;justify-content:space-between;align-items:center}

/* 二级标签 & 小组可点击行 */
.subtab{height:36px;padding:0 18px;border-radius:9px;font-size:14px;font-weight:600;color:#64748b;background:transparent}
.subtab.on{background:#fff;color:var(--blue);box-shadow:0 2px 8px rgba(37,99,235,.15)}
.group-row{cursor:pointer}
.group-row:hover td{background:#eff6ff!important}
.group-name-cell{display:flex;align-items:center;gap:8px;color:#2563eb;font-weight:600}
.group-name-cell .chev{font-size:12px;color:#94a3b8;font-weight:400}

/* 响应式 */
@media (max-width:900px){
  .layout{flex-direction:column;padding:16px}
  .sidebar{width:100%;position:static}
  .topbar{padding:10px 16px}
  .timer-time{font-size:80px}
  .panel{padding:16px}
  .welcome-card{padding:36px 24px}
  .welcome-title{font-size:21px;letter-spacing:2px}
  .welcome-sub{font-size:13px;letter-spacing:3px}
  .welcome-emoji{font-size:40px}
}
</style>
</head>
<body>

<div class="login-wrap" id="loginView">
  <div class="login-card">
    <div class="login-title" style="display:flex;align-items:center;gap:10px">班级全能管理系统</div>
    <p class="login-sub">登录后数据自动同步到云端，换电脑登录同一账号即可查看</p>
    <div class="field"><label>账号</label><input id="loginUser" type="text" placeholder="请输入账号"></div>
    <div class="field"><label>密码</label><input id="loginPass" type="password" placeholder="请输入密码"></div>
    <div class="field hidden" id="regPassWrap"><label>确认密码</label><input id="loginPass2" type="password" placeholder="再次输入密码"></div>
    <div class="login-err" id="loginErr" style="color:#ef4444;font-size:13px;min-height:20px;margin-top:8px"></div>
    <button class="login-btn" id="loginBtn">登录</button>
    <div class="login-switch" id="loginSwitch">还没有账号？<b>立即注册</b></div>
  </div>
</div>

<!-- 全屏欢迎遮罩：点击登录后才出现 -->
<div class="welcome-mask hidden" id="welcomeMask">
  <div class="welcome-card">
    <div class="welcome-emoji">🎉</div>
    <div class="welcome-title">欢迎进入班级全能管理系统</div>
    <div class="welcome-line"></div>
    <div class="welcome-sub">一班英才 星辉满怀 书山利剑 决胜未来</div>
    <div class="welcome-tip">正在为你加载班级数据…</div>
  </div>
</div>

<div id="appView" class="hidden">
  <header class="topbar">
    <div class="brand">
      <div class="mark"><svg viewBox="0 0 24 24"><rect x="3" y="13" width="4" height="8" rx="1"/><rect x="10" y="9" width="4" height="12" rx="1"/><rect x="17" y="4" width="4" height="17" rx="1"/></svg></div>
      <div class="brand-txt"><div class="t">班级全能终端</div><div class="s"><span class="dot"></span><span id="curUser">—</span> · <span id="syncStatus">云端已连接</span></div></div>
    </div>
    <div class="top-actions">
      <button class="tbtn notice" id="btnNotice">📢 班级公告</button>
      <button class="tbtn timer" id="btnTimer">⏰ 倒计时</button>
      <button class="tbtn lucky" id="btnLucky">🎲 抽人</button>
      <button class="tbtn export" id="btnExport">导出报表</button>
      <button class="tbtn profile" id="btnProfile">个人中心</button>
    </div>
  </header>

  <div class="layout">
    <aside class="sidebar">
      <div class="card">
        <div class="stat-row">
          <div class="stat"><div class="k">学生总数</div><div class="v" id="statStu">0</div></div>
          <div class="stat alt"><div class="k">全班总积分</div><div class="v" id="statTotalScore">0</div></div>
        </div>
        <div class="card-bd" style="padding-top:0">
          <div class="today-row"><span>今日加分</span><b id="todayPlus">0 次</b></div>
          <div class="today-row"><span>今日扣分</span><b id="todayMinus">0 次</b></div>
          <div class="today-row" style="padding-bottom:0"><span>今日净变化</span><b id="todayNet">0</b></div>
        </div>
      </div>

      <div class="card" style="background:linear-gradient(135deg,#eff6ff,#dbeafe);border:none;box-shadow:none">
        <div class="card-bd" style="text-align:center;padding:24px 16px">
          <div style="font-size:14px;color:#475569;font-weight:600;margin-bottom:8px">距离 <span id="examName" contenteditable="true" style="border-bottom:1px dashed #93c5fd;cursor:text;outline:none">期末考试</span> 还有</div>
          <div style="font-size:40px;font-weight:800;color:#2563eb;line-height:1.1;cursor:pointer" id="examCountdown" title="点击设置考试日期">--</div>
          <div style="font-size:12px;color:#94a3b8;margin-top:8px">文字可改名 · 数字可设置日期</div>
        </div>
      </div>

      <div class="card">
        <div class="card-hd">快捷操作</div>
        <div class="card-bd" style="display:flex;flex-direction:column;gap:12px">
          <button class="tbtn sync" id="btnOpenAddStu" style="justify-content:center;width:100%">+ 新增学生</button>
          <button class="tbtn export" id="btnOpenCsv" style="justify-content:center;width:100%">📁 批量导入名单</button>
        </div>
      </div>
    </aside>

    <main class="main">
      <nav class="tabs" id="tabs">
        <button class="tab on" data-tab="students">👨‍🎓 学生榜</button>
        <button class="tab" data-tab="groups">👥 小组榜</button>
        <button class="tab" data-tab="exam">📊 成绩大榜</button>
        <button class="tab" data-tab="homework">📝 作业白板</button>
        <button class="tab" data-tab="shop">🎁 商城</button>
        <button class="tab" data-tab="feeds">📢 动态墙</button>
        <button class="tab" data-tab="attendance">📋 考勤</button>
      </nav>

      <section class="panel" id="panel-students">
        <div class="notice-bar hidden" id="noticeBar">
          <span class="ico">📢</span>
          <div id="noticeText" style="flex:1;white-space:pre-wrap"></div>
        </div>

        <div style="background:#f8fafc;border:1px solid #e2e8f0;border-radius:12px;padding:16px 20px;margin-bottom:20px;display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;gap:16px">
          <div>
            <div style="font-size:15px;font-weight:700;color:#1e293b">📊 学期积分数据汇总</div>
            <div style="font-size:13px;color:#64748b;margin-top:4px">全班累计共产生 <b id="sumLogs" style="color:#2563eb">0</b> 次加减分记录</div>
          </div>
          <div style="display:flex;gap:24px;text-align:right;flex-wrap:wrap">
            <div><div style="font-size:12px;color:#94a3b8">全班总积分</div><div style="font-size:20px;font-weight:800;color:#2563eb" id="sumTotalScore">0</div></div>
            <div><div style="font-size:12px;color:#94a3b8">班级人均分</div><div style="font-size:20px;font-weight:800;color:#10b981" id="sumAvgScore">0</div></div>
          </div>
        </div>

        <div class="toolbar" style="display:flex;gap:12px;margin-bottom:16px;flex-wrap:wrap">
          <input id="searchStu" placeholder="搜索学生姓名 / 小组..." style="flex:1;min-width:180px;height:42px;border:1.5px solid #e2e8f0;border-radius:10px;padding:0 14px">
          <select id="filterGroup" style="height:42px;border:1.5px solid #e2e8f0;border-radius:10px;padding:0 12px;background:#fff;min-width:130px">
            <option value="">全部小组</option>
          </select>
          <button style="background:#f59e0b;color:#fff;padding:0 16px;height:42px;border-radius:10px;font-weight:600" id="btnBatchStu">批量加减</button>
        </div>

        <div class="tbl-scroll">
          <table>
            <thead><tr><th>排名</th><th>姓名</th><th>小组</th><th>职务</th><th>积分</th><th>操作</th></tr></thead>
            <tbody id="tbodyStu"></tbody>
          </table>
        </div>
      </section>

      <section class="panel hidden" id="panel-groups">
        <div class="tbl-scroll">
          <table><thead><tr><th>排名</th><th>小组名称</th><th>人数</th><th>总积分</th><th>人均积分</th></tr></thead><tbody id="tbodyGrp"></tbody></table>
        </div>
      </section>

      <section class="panel hidden" id="panel-exam">
        <div class="toolbar" style="display:flex;gap:12px;margin-bottom:16px;flex-wrap:wrap">
          <input id="searchExam" placeholder="搜索学生姓名..." style="flex:1;min-width:180px;height:42px;border:1.5px solid #e2e8f0;border-radius:10px;padding:0 14px">
          <button style="background:#3b82f6;color:#fff;padding:0 16px;height:42px;border-radius:10px;font-weight:600" id="btnAddExam">+ 录入/修改成绩</button>
        </div>
        <div id="examStats" style="display:flex;gap:16px;flex-wrap:wrap;background:#f8fafc;padding:12px 16px;border-radius:10px;font-size:13px;color:#475569;margin-bottom:16px"></div>
        <div style="font-size:12.5px;color:#94a3b8;margin-bottom:8px">💡 「学年榜」这一列可以直接点单元格填写，填完自动保存</div>
        <div class="tbl-scroll">
          <table>
            <thead><tr>
              <th style="color:#7c3aed">学年榜 ✎</th>
              <th>总分排</th>
              <th>姓名</th>
              <th>语文</th><th>数学</th><th>英语</th><th>物理</th><th>化学</th><th>生物</th>
              <th>总分</th>
            </tr></thead>
            <tbody id="tbodyExam"></tbody>
          </table>
        </div>
      </section>

      <section class="panel hidden" id="panel-homework">
        <div class="toolbar" style="display:flex;justify-content:space-between;align-items:center;margin-bottom:16px;gap:12px;flex-wrap:wrap">
          <div style="font-size:14px;color:#64748b">今日作业白板</div>
          <button style="background:var(--blue);color:#fff;padding:0 20px;height:40px;border-radius:10px;font-weight:600" id="btnAddHomework">+ 布置新作业</button>
        </div>
        <div class="hw-board" id="hwBoard"></div>
      </section>

      <section class="panel hidden" id="panel-shop">
        <div class="toolbar" style="margin-bottom:16px;display:flex;gap:12px;flex-wrap:wrap;align-items:center">
          <button style="background:var(--blue);color:#fff;padding:0 20px;height:40px;border-radius:10px;font-weight:600" id="btnAddGoods">+ 添加奖品</button>
          <span id="redeemTip" style="font-size:13px;color:#94a3b8"></span>
        </div>
        <div class="shop-grid" id="shopGrid" style="display:grid;grid-template-columns:repeat(auto-fill,minmax(220px,1fr));gap:16px"></div>
      </section>

      <section class="panel hidden" id="panel-feeds">
        <div class="toolbar" style="display:flex;gap:12px;margin-bottom:16px;flex-wrap:wrap">
          <input id="searchFeeds" placeholder="搜索姓名 / 原因..." style="flex:1;min-width:180px;height:42px;border:1.5px solid #e2e8f0;border-radius:10px;padding:0 14px">
          <div style="font-size:13px;color:#94a3b8;display:flex;align-items:center">共 <span id="feedsCount" style="margin:0 4px;color:#2563eb;font-weight:700">0</span> 条记录</div>
        </div>
        <div class="hist-list" id="allFeedsList" style="max-height:600px"></div>
      </section>

      <section class="panel hidden" id="panel-attendance">
        <div class="toolbar" style="margin-bottom:16px;display:flex;gap:12px;flex-wrap:wrap;align-items:center">
          <button class="act plain" style="height:38px;padding:0 16px;background:#ecfdf5;color:#059669;font-weight:600" id="btnAllNormal">✅ 全部设为正常</button>
          <span style="font-size:13px;color:#94a3b8">迟到 -1分 · 旷课 -2分 · 请假需填写理由</span>
        </div>
        <div class="tbl-scroll">
          <table><thead><tr><th>姓名</th><th>今日状态</th><th>考勤操作</th></tr></thead><tbody id="tbodyAttendance"></tbody></table>
        </div>
      </section>
    </main>
  </div>
</div>

<div id="modalBack" class="modal-back hidden"><div class="modal" id="modalBox"></div></div>
<div class="toast" id="toast"></div>

<script>
const CONFIG = { APP_KEY: '6816F27B16D39A008D8E5E7948C43F71', API_DOMAIN: 'https://api.yesapi.net/', TABLE: 'score_list' };

document.addEventListener('DOMContentLoaded', function(){
  const $ = id => document.getElementById(id);
  const loginView = $('loginView'), appView = $('appView');
  const curUser = $('curUser'), syncStatus = $('syncStatus');
  let isLoginMode = true, currentUser = '', saveTimer = null, countdownTimer = null;
  let students = [], shopGoods = [], redeemLogs = [], homeworks = [], notices = '';

  /* ================= 通用工具 ================= */
  function toast(msg){
    const t = $('toast'); if(!t) return;
    t.textContent = msg;
    t.classList.add('show');
    clearTimeout(t._timer);
    t._timer = setTimeout(()=>t.classList.remove('show'), 2200);
  }
  function openModal(){ $('modalBack').classList.remove('hidden'); }
  function closeModal(){ $('modalBack').classList.add('hidden'); }
  function nowStr(){ return new Date().toLocaleString(); }
  function isToday(str){
    if(!str) return false;
    const d = new Date(str);
    if(isNaN(d.getTime())) return false;
    const n = new Date();
    return d.getFullYear()===n.getFullYear() && d.getMonth()===n.getMonth() && d.getDate()===n.getDate();
  }

  /* ================= 欢迎遮罩 ================= */
  function showWelcome(){
    const m = $('welcomeMask');
    m.classList.remove('hidden');
    requestAnimationFrame(()=>{ m.classList.add('show'); });
  }
  function hideWelcome(){
    const m = $('welcomeMask');
    m.classList.remove('show');
    setTimeout(()=>{ m.classList.add('hidden'); }, 400);
  }

  /* ================= 云端同步 ================= */
  async function apiRequest(service, params){
    const body = new URLSearchParams();
    body.append('app_key', CONFIG.APP_KEY);
    body.append('yesapi_allow_origin', '1');
    for(const k in params){ body.append(k, typeof params[k] === 'string' ? params[k] : JSON.stringify(params[k])); }
    try{
      const res = await fetch(CONFIG.API_DOMAIN + '?s=' + service, { method:'POST', body });
      return await res.json();
    }catch(e){ console.warn('API请求失败', e); return null; }
  }

  async function pullFromCloud(){
    syncStatus.textContent = '正在加载...';
    const localData = localStorage.getItem('class_backup_' + currentUser);
    if(localData){
      try{
        const obj = JSON.parse(localData);
        students = obj.students || [];
        shopGoods = obj.shopGoods || [];
        redeemLogs = obj.redeemLogs || [];
        homeworks = obj.homeworks || [];
        notices = obj.notices || '';
        renderAll();
      }catch(e){ console.warn('本地备份解析失败', e); }
    }
    try{
      const r = await apiRequest('App.Table.Get', { model_name: CONFIG.TABLE, where: JSON.stringify([['用户ID', '=', currentUser]]) });
      let row = null;
      if(r && r.data && r.data.data){ row = Array.isArray(r.data.data) ? r.data.data[0] : r.data.data; }
      if(row && row['数据']){
        const cloudData = JSON.parse(row['数据']);
        if(Array.isArray(cloudData)){ students = cloudData; }
        else{
          students = cloudData.students || [];
          shopGoods = cloudData.shopGoods || [];
          redeemLogs = cloudData.redeemLogs || [];
          homeworks = cloudData.homeworks || [];
          notices = cloudData.notices || '';
        }
        renderAll();
      }
      syncStatus.textContent = '云端已连接';
    }catch(e){
      syncStatus.textContent = '本地模式运行中';
    }
  }

  async function pushToCloud(){
    if(!currentUser) return;
    syncStatus.textContent = '正在保存...';
    const payload = JSON.stringify({ students, shopGoods, redeemLogs, homeworks, notices });
    const q = await apiRequest('App.Table.Get', { model_name: CONFIG.TABLE, where: JSON.stringify([['用户ID', '=', currentUser]]) });
    let existId = null;
    if(q && q.data && q.data.data){
      const row = Array.isArray(q.data.data) ? q.data.data[0] : q.data.data;
      if(row && row.id) existId = row.id;
    }
    const dataObj = {
      '用户ID': currentUser,
      '学生姓名': '班级完整数据',
      '积分': students.reduce((n,s)=>n+(s.score||0),0),
      '数据': payload
    };
    try{
      if(existId) await apiRequest('App.Table.Update', { model_name: CONFIG.TABLE, id: existId, data: JSON.stringify(dataObj) });
      else await apiRequest('App.Table.Create', { model_name: CONFIG.TABLE, data: JSON.stringify(dataObj) });
      syncStatus.textContent = '云端已保存 ' + new Date().toLocaleTimeString();
    }catch(e){
      syncStatus.textContent = '云端保存失败(已存本地)';
    }
  }

  function scheduleSave(){
    try{
      localStorage.setItem('class_backup_' + currentUser, JSON.stringify({ students, shopGoods, redeemLogs, homeworks, notices }));
    }catch(e){ console.warn('本地保存失败', e); }
    clearTimeout(saveTimer);
    saveTimer = setTimeout(()=>{
      pushToCloud().catch(()=>{ syncStatus.textContent = '云端保存失败(已存本地)'; });
    }, 1500);
  }

  /* ================= 登录 / 注册 ================= */
  function switchMode(login){
    isLoginMode = login;
    $('loginErr').textContent = '';
    if(login){
      $('loginBtn').textContent = '登录';
      $('loginSwitch').innerHTML = '还没有账号？<b>立即注册</b>';
      $('regPassWrap').classList.add('hidden');
    }else{
      $('loginBtn').textContent = '注册';
      $('loginSwitch').innerHTML = '已有账号？<b>返回登录</b>';
      $('regPassWrap').classList.remove('hidden');
    }
  }

  async function doLogin(){
    $('loginErr').textContent = '';
    const u = $('loginUser').value.trim();
    const p = $('loginPass').value.trim();
    if(!u || !p){ $('loginErr').textContent = '账号和密码不能为空'; return; }

    if(isLoginMode){
      const saved = localStorage.getItem('class_user_' + u);
      if(!saved){ $('loginErr').textContent = '账号不存在，请先注册'; return; }
      let pwd = '';
      try{ pwd = JSON.parse(saved).pwd; }catch(e){ $('loginErr').textContent = '账号数据损坏，请重新注册'; return; }
      if(pwd !== p){ $('loginErr').textContent = '密码错误'; return; }

      currentUser = u;
      curUser.textContent = u;
      // 校验通过后才弹出全屏欢迎遮罩
      showWelcome();

      const t0 = Date.now();
      try{ await pullFromCloud(); }catch(e){}
      renderAll();

      const wait = Math.max(0, 1700 - (Date.now() - t0));
      setTimeout(()=>{
        hideWelcome();
        setTimeout(()=>{
          loginView.classList.add('hidden');
          appView.classList.remove('hidden');
          initCountdown();
        }, 220);
      }, wait);
    }else{
      const p2 = $('loginPass2').value.trim();
      if(!p2){ $('loginErr').textContent = '请输入确认密码'; return; }
      if(p !== p2){ $('loginErr').textContent = '两次密码不一致'; return; }
      if(localStorage.getItem('class_user_' + u)){ $('loginErr').textContent = '账号已存在'; return; }
      localStorage.setItem('class_user_' + u, JSON.stringify({ pwd: p }));
      toast('注册成功，请登录');
      switchMode(true);
    }
  }

  $('loginBtn').addEventListener('click', doLogin);
  $('loginSwitch').addEventListener('click', ()=>switchMode(!isLoginMode));
  $('loginPass').addEventListener('keydown', e=>{ if(e.key === 'Enter') doLogin(); });

  /* ================= 小组 ================= */
  const GROUPS = ['第1组','第2组','第3组','第4组','第5组','第6组','第7组','第8组','第9组'];

  function groupOptionsHtml(current){
    let arr = GROUPS.slice();
    if(current && arr.indexOf(current) < 0) arr.push(current);
    let html = '<option value="">未分组</option>';
    html += arr.map(g=>'<option value="'+g+'"'+(g===current?' selected':'')+'>'+g+'</option>').join('');
    return html;
  }

  function renderGroupFilter(){
    const sel = $('filterGroup'); if(!sel) return;
    const keep = sel.value;
    const all = {};
    students.forEach(s=>{ all[s.group || '未分组'] = true; });
    let html = '<option value="">全部小组</option>';
    Object.keys(all).sort().forEach(g=>{ html += '<option value="'+g+'">'+g+'</option>'; });
    sel.innerHTML = html;
    if(keep){ sel.value = keep; if(!sel.value) sel.value = ''; }
  }

  /* ================= 渲染 ================= */
  function renderAll(){
    renderNotice();
    renderStats();
    renderGroupFilter();
    renderStudentList();
    renderGroups();
    renderExam();
    renderHomework();
    renderShop();
    renderFeeds();
    renderAttendance();
  }

  function renderNotice(){
    const bar = $('noticeBar'); if(!bar) return;
    if(notices && notices.trim()){
      bar.classList.remove('hidden');
      $('noticeText').textContent = notices;
    }else{
      bar.classList.add('hidden');
    }
  }

  function renderStats(){
    const totalScore = students.reduce((n,s)=>n+(s.score||0),0);
    const totalLogs = students.reduce((n,s)=>n+((s.logs&&s.logs.length)||0),0);
    if($('statStu')) $('statStu').textContent = students.length;
    if($('statTotalScore')) $('statTotalScore').textContent = totalScore;
    if($('sumLogs')) $('sumLogs').textContent = totalLogs;
    if($('sumTotalScore')) $('sumTotalScore').textContent = totalScore;
    if($('sumAvgScore')) $('sumAvgScore').textContent = students.length ? (totalScore/students.length).toFixed(1) : 0;

    let plus = 0, minus = 0, net = 0;
    students.forEach(s=>{
      (s.logs||[]).forEach(l=>{
        if(!isToday(l.time)) return;
        if(l.delta > 0) plus++;
        else if(l.delta < 0) minus++;
        net += (l.delta||0);
      });
    });
    if($('todayPlus')) $('todayPlus').textContent = plus + ' 次';
    if($('todayMinus')) $('todayMinus').textContent = minus + ' 次';
    if($('todayNet')) $('todayNet').textContent = (net>0?'+':'') + net;
  }

  function renderStudentList(){
    const tbody = $('tbodyStu'); if(!tbody) return;
    let list = [...students];
    const kw = ($('searchStu').value || '').trim();
    const fg = $('filterGroup') ? $('filterGroup').value : '';
    if(kw) list = list.filter(s=>(s.name||'').includes(kw) || (s.group||'').includes(kw));
    if(fg) list = list.filter(s=> (s.group || '未分组') === fg);
    list.sort((a,b)=>(b.score||0)-(a.score||0));

    if(list.length === 0){
      tbody.innerHTML = '<tr><td colspan="6"><div class="empty">暂无学生，点击左侧「+ 新增学生」添加</div></td></tr>';
      return;
    }

    tbody.innerHTML = list.map((s,i)=>{
      const medal = i===0 ? '👑' : (i===1 ? '🥈' : (i===2 ? '🥉' : ((s.score||0)>=100 ? '⭐' : '')));
      const avatarClass = (s.group && /组/.test(s.group)) ? 'g' + (s.group.replace(/[^0-9]/g,'') || '9') : '';
      return '<tr>' +
        '<td>'+ (i+1) +'</td>' +
        '<td><div class="name-cell"><div class="avatar '+avatarClass+'">'+ ((s.name||'?').charAt(0)) +'</div><span>'+ s.name +' '+ medal +'</span></div></td>' +
        '<td>'+ (s.group || '未分组') +'</td>' +
        '<td>'+ (s.duty || '-') +'</td>' +
        '<td><span class="score-num">'+ (s.score||0) +'</span></td>' +
        '<td><div class="acts">' +
          '<button class="act plus" onclick="openScoreModal('+s.id+',\'add\')">加分</button>' +
          '<button class="act minus" onclick="openScoreModal('+s.id+',\'minus\')">减分</button>' +
          '<button class="act edit" onclick="openEditStudent('+s.id+')">编辑</button>' +
          '<button class="act plain" onclick="openHistoryModal('+s.id+')">历史</button>' +
        '</div></td>' +
      '</tr>';
    }).join('');
  }

  function renderGroups(){
    const tbody = $('tbodyGrp'); if(!tbody) return;
    const map = {};
    students.forEach(s=>{
      const g = s.group || '未分组';
      if(!map[g]) map[g] = { count:0, total:0 };
      map[g].count++;
      map[g].total += (s.score||0);
    });
    const arr = Object.keys(map).map(name=>({ name:name, count:map[name].count, total:map[name].total, avg: map[name].count ? (map[name].total/map[name].count).toFixed(1) : '0' }))
      .sort((a,b)=>b.total-a.total);

    if(arr.length === 0){ tbody.innerHTML = '<tr><td colspan="5"><div class="empty">暂无小组数据</div></td></tr>'; return; }
    const maxScore = Math.max.apply(null, arr.map(g=>Math.abs(g.total)).concat([1]));

    tbody.innerHTML = arr.map((g,i)=>{
      const color = i===0 ? '#fbbf24' : (i===1 ? '#60a5fa' : (i===2 ? '#94a3b8' : '#cbd5e1'));
      const percent = maxScore === 0 ? 0 : (Math.abs(g.total)/maxScore)*100;
      const key = String(g.name).replace(/\\/g,'\\\\').replace(/'/g,'&#39;');
      return '<tr class="group-row" onclick="openGroupModal(\''+ key +'\')">' +
        '<td>'+ (i+1) +'</td>' +
        '<td><div class="group-name-cell">'+ g.name +'<span class="chev">点击查看成员 ›</span></div></td>' +
        '<td>'+ g.count +'</td>' +
        '<td><span class="score-num">'+ g.total +'</span>' +
        '<div style="height:8px;background:#e2e8f0;border-radius:4px;margin-top:6px"><div style="height:100%;width:'+percent+'%;background:'+color+';border-radius:4px"></div></div></td>' +
        '<td>'+ g.avg +'</td></tr>';
    }).join('');
  }

  function examTotal(e){
    if(!e) return 0;
    return (e.ch||0)+(e.ma||0)+(e.en||0)+(e.ph||0)+(e.chm||0)+(e.bio||0);
  }

  function renderExam(){
    const tbody = $('tbodyExam'); if(!tbody) return;
    students.forEach(s=>{ if(!s.exam) s.exam = { ch:0, ma:0, en:0, ph:0, chm:0, bio:0 }; });

    const subjects = ['ch','ma','en','ph','chm','bio'];
    const rankDict = {};
    subjects.forEach(sub=>{
      const valid = students.map(s=>({ id:s.id, score:(s.exam[sub]||0) })).filter(x=>x.score>0).sort((a,b)=>b.score-a.score);
      rankDict[sub] = {};
      valid.forEach((x,idx)=>{ rankDict[sub][x.id] = idx+1; });
    });

    const validTotals = students.map(s=>({ id:s.id, score:examTotal(s.exam) })).filter(x=>x.score>0).sort((a,b)=>b.score-a.score);
    const totalRankDict = {};
    validTotals.forEach((x,idx)=>{ totalRankDict[x.id] = idx+1; });

    let list = [...students];
    const kw = ($('searchExam').value || '').trim();
    if(kw) list = list.filter(s=>(s.name||'').includes(kw));
    list.sort((a,b)=>examTotal(b.exam)-examTotal(a.exam));

    let totalAll = 0, passCnt = 0, excellentCnt = 0;
    list.forEach(s=>{
      const t = examTotal(s.exam);
      totalAll += t;
      if(t >= 60*6*0.6) passCnt++;
      if(t >= 60*6*0.85) excellentCnt++;
    });
    if($('examStats')){
      $('examStats').innerHTML = '当前人数: <b>'+list.length+'</b> &nbsp;|&nbsp; 均分: <b>'+
        (list.length ? (totalAll/list.length).toFixed(1) : 0) +'</b> &nbsp;|&nbsp; 及格: <b>'+passCnt+
        '</b> &nbsp;|&nbsp; 优秀: <b>'+excellentCnt+'</b>';
    }

    if(list.length === 0){
      tbody.innerHTML = '<tr><td colspan="10"><div class="empty">暂无学生</div></td></tr>';
      return;
    }

    tbody.innerHTML = list.map((s,i)=>{
      const e = s.exam;
      const total = examTotal(e);
      const rankStr = sub => (e[sub]||0)>0 ? '<span style="font-size:12px;color:#94a3b8;margin-left:4px">(第'+(rankDict[sub][s.id]||'-')+'名)</span>' : '';
      const cls = v => (v<60 && v>0) ? 'text-red' : '';
      const totalRank = totalRankDict[s.id];
      const totalRankColor = (totalRank && totalRank<=3) ? '#d97706' : '#94a3b8';
      const yearVal = (s.year === null || s.year === undefined || s.year === '') ? '-' : s.year;
      return '<tr>' +
        '<td onclick="setYearScore('+s.id+')" title="点击填写学年榜分数" style="cursor:pointer;color:#7c3aed;font-weight:700;background:#faf5ff">'+ yearVal +'</td>' +
        '<td style="color:'+totalRankColor+'">'+ (totalRank || '-') +'</td>' +
        '<td><b>'+ s.name +'</b></td>' +
        '<td class="'+cls(e.ch)+'">'+ (e.ch||'-') +' '+rankStr('ch')+'</td>' +
        '<td class="'+cls(e.ma)+'">'+ (e.ma||'-') +' '+rankStr('ma')+'</td>' +
        '<td class="'+cls(e.en)+'">'+ (e.en||'-') +' '+rankStr('en')+'</td>' +
        '<td class="'+cls(e.ph)+'">'+ (e.ph||'-') +' '+rankStr('ph')+'</td>' +
        '<td class="'+cls(e.chm)+'">'+ (e.chm||'-') +' '+rankStr('chm')+'</td>' +
        '<td class="'+cls(e.bio)+'">'+ (e.bio||'-') +' '+rankStr('bio')+'</td>' +
        '<td><span class="score-num" style="font-size:16px">'+ (total||'-') +'</span></td>' +
      '</tr>';
    }).join('');
  }

  /* ---------- 小组详情弹窗 ---------- */
  window.openGroupModal = function(groupName){
    const members = students.filter(s=>(s.group || '未分组') === groupName).sort((a,b)=>(b.score||0)-(a.score||0));
    const total = members.reduce((n,s)=>n+(s.score||0),0);
    const avg = members.length ? (total/members.length).toFixed(1) : '0';

    const box = $('modalBox');
    box.innerHTML =
      '<div class="m-hd"><h3>👥 '+ groupName +'</h3><button class="m-close" id="mClose">×</button></div>' +
      '<div class="m-bd">' +
        '<div style="display:flex;gap:20px;background:#f8fafc;border:1px solid #e2e8f0;border-radius:10px;padding:12px 16px;margin-bottom:14px;font-size:13px;color:#64748b">' +
          '<div>人数 <b style="color:#2563eb">'+ members.length +'</b></div>' +
          '<div>总积分 <b style="color:#2563eb">'+ total +'</b></div>' +
          '<div>人均 <b style="color:#10b981">'+ avg +'</b></div>' +
        '</div>' +
        (members.length === 0
          ? '<div class="empty">该小组暂无成员</div>'
          : members.map((s,i)=>{
              const medal = i===0 ? '👑' : (i===1 ? '🥈' : (i===2 ? '🥉' : ''));
              return '<div style="display:flex;align-items:center;gap:10px;padding:10px 0;border-bottom:1px solid #f1f5f9">' +
                '<div style="width:22px;color:#94a3b8;font-weight:600">'+ (i+1) +'</div>' +
                '<div class="avatar '+(s.group && /组/.test(s.group) ? 'g'+(s.group.replace(/[^0-9]/g,'')||'9') : '')+'">'+ ((s.name||'?').charAt(0)) +'</div>' +
                '<div style="flex:1;min-width:0">' +
                  '<div style="font-weight:600;white-space:nowrap;overflow:hidden;text-overflow:ellipsis">'+ s.name +' '+ medal +'</div>' +
                  '<div style="font-size:12px;color:#94a3b8">'+ (s.duty || '无职务') +'</div>' +
                '</div>' +
                '<div class="score-num" style="margin-right:6px">'+ (s.score||0) +'</div>' +
                '<button class="act plus" onclick="openScoreModal('+s.id+',\'add\')">加分</button>' +
                '<button class="act minus" onclick="openScoreModal('+s.id+',\'minus\')">减分</button>' +
              '</div>';
            }).join('')
        ) +
      '</div>' +
      '<div class="m-ft"><button class="btn-line" id="mCloseBtn">关闭</button></div>';

    openModal();
    $('mClose').onclick = $('mCloseBtn').onclick = closeModal;
  };

  /* ---------- 年级/学年榜：点击单元格填写 ---------- */
  window.setYearScore = function(id){
    const s = students.find(x=>x.id === id);
    if(!s) return;
    const cur = (s.year === null || s.year === undefined || s.year === '') ? '' : String(s.year);
    const input = prompt('请输入【' + s.name + '】的学年榜分数（留空则清除）：', cur);
    if(input === null) return;
    const v = (input || '').trim();
    if(v === ''){
      s.year = null;
    }else{
      const n = Number(v);
      if(isNaN(n)){ toast('请输入数字'); return; }
      s.year = n;
    }
    renderExam();
    scheduleSave();
    toast('已保存');
  };

  function renderHomework(){
    const board = $('hwBoard'); if(!board) return;
    if(homeworks.length === 0){
      board.innerHTML = '<div class="empty" style="grid-column:1/-1">暂无作业，点击右上角「+ 布置新作业」</div>';
      return;
    }
    const colorOf = sub => sub==='语文' ? '#f87171' : sub==='数学' ? '#60a5fa' : sub==='英语' ? '#34d399' : sub==='物理' ? '#a78bfa' : sub==='化学' ? '#fbbf24' : '#94a3b8';
    board.innerHTML = homeworks.map((h,i)=>{
      return '<div class="hw-card" style="border-top:4px solid '+colorOf(h.subject)+'">' +
        '<div class="hw-sub">'+ h.subject +'<span style="font-size:12px;color:#94a3b8;font-weight:500">'+ (h.date||'') +'</span></div>' +
        '<div style="font-size:14px;color:#475569;line-height:1.7;margin-bottom:12px;min-height:44px;white-space:pre-wrap">'+ (h.content||'') +'</div>' +
        '<div style="position:absolute;bottom:12px;right:12px;font-size:12px;color:#ef4444;cursor:pointer" onclick="delHomework('+i+')">✖ 删除</div>' +
      '</div>';
    }).join('');
  }

  function renderShop(){
    const grid = $('shopGrid'); if(!grid) return;
    if($('redeemTip')) $('redeemTip').textContent = redeemLogs.length ? ('已完成 ' + redeemLogs.length + ' 次兑换') : '';
    if(shopGoods.length === 0){
      grid.innerHTML = '<div class="empty" style="grid-column:1/-1">暂无商品，点击上方「+ 添加奖品」</div>';
      return;
    }
    grid.innerHTML = shopGoods.map((g,i)=>{
      const soldOut = g.stock <= 0;
      return '<div style="border:1px solid #e2e8f0;border-radius:12px;padding:16px;display:flex;flex-direction:column;gap:10px">' +
        '<div style="font-size:15px;font-weight:600">'+ g.name +'</div>' +
        '<div style="font-size:13px;color:#64748b;display:flex;justify-content:space-between">' +
          '<span style="color:#d97706;font-weight:700">'+ g.cost +' 积分</span><span>库存 '+ g.stock +'</span></div>' +
        '<button style="height:36px;border-radius:8px;background:#eff6ff;color:#2563eb;font-weight:600;'+(soldOut?'opacity:.5;cursor:not-allowed;':'')+'" ' +
          (soldOut ? 'disabled' : 'onclick="openRedeemModal('+i+')"') + '>兑换</button>' +
        '<div style="display:flex;justify-content:flex-end;gap:12px;font-size:12px">' +
          '<span style="color:#4f46e5;cursor:pointer" onclick="openEditGoods('+i+')">编辑</span>' +
          '<span style="color:#ef4444;cursor:pointer" onclick="delGoods('+i+')">删除</span>' +
        '</div>' +
      '</div>';
    }).join('');
  }

  function renderFeeds(){
    const box = $('allFeedsList'); if(!box) return;
    const kw = ($('searchFeeds') && $('searchFeeds').value) ? $('searchFeeds').value.trim() : '';
    let all = [];
    students.forEach(s=>{
      (s.logs||[]).forEach((l,idx)=>{
        all.push({ sid:s.id, name:s.name, idx:idx, time:l.time, delta:l.delta, reason:l.reason, group:(s.group||'未分组') });
      });
    });
    all.sort((a,b)=> new Date(a.time).getTime() - new Date(b.time).getTime());
    all.reverse();

    let show = all;
    if(kw) show = all.filter(x=> (x.name||'').indexOf(kw)>=0 || (x.reason||'').indexOf(kw)>=0);
    if($('feedsCount')) $('feedsCount').textContent = all.length;

    if(show.length === 0){
      box.innerHTML = '<div class="empty">' + (all.length === 0 ? '暂无动态' : '没有匹配的记录') + '</div>';
      return;
    }
    box.innerHTML = show.slice(0,200).map(l=>
      '<div class="hist-item">' +
        '<div><div style="font-size:12px;color:#94a3b8">'+ l.time +' · '+ l.group +'</div>' +
        '<div style="font-weight:500"><b style="color:#2563eb">'+ l.name +'</b> · '+ (l.reason||'') +'</div></div>' +
        '<div style="display:flex;align-items:center;gap:10px">' +
          '<div class="h-num '+(l.delta>0?'up':(l.delta<0?'down':''))+'">'+ (l.delta>0?'+':'') + l.delta +'</div>' +
          '<button class="act del" onclick="undoLog('+l.sid+','+l.idx+')">撤销</button>' +
        '</div>' +
      '</div>'
    ).join('');
  }

  function renderAttendance(){
    const tbody = $('tbodyAttendance'); if(!tbody) return;
    if(students.length === 0){ tbody.innerHTML = '<tr><td colspan="3"><div class="empty">暂无学生</div></td></tr>'; return; }
    tbody.innerHTML = students.map(s=>{
      const st = s.attend || '正常';
      const color = st==='迟到' ? '#f39c12' : (st.indexOf('请假')>=0 ? '#3498db' : (st==='旷课' ? '#e0454c' : '#18a86b'));
      return '<tr><td>'+ s.name +'</td><td><span style="color:'+color+';font-weight:600">'+ st +'</span></td>' +
        '<td><div class="acts">' +
          '<button class="act plain" onclick="setAttend('+s.id+',\'迟到\')">迟到</button>' +
          '<button class="act plain" onclick="setAttend('+s.id+',\'请假\')">请假</button>' +
          '<button class="act plain" onclick="setAttend('+s.id+',\'旷课\')">旷课</button>' +
          '<button class="act plain" onclick="setAttend('+s.id+',\'正常\')">正常</button>' +
        '</div></td></tr>';
    }).join('');
  }

  /* ================= 加减分弹窗 ================= */
  window.openScoreModal = function(id, type){
    const stu = students.find(x=>x.id === id);
    if(!stu){ toast('学生不存在'); return; }

    let isAdd = (type === 'add' || type === 'plus');

    const reasonsAdd = ["按时交作业","课堂发言","作业优秀","成绩进步","互助讲题","课前预习","错题订正","主动提问","背诵过关","竞赛获奖","守纪自律","文明有礼","拾金上交","课间守序","安静自习","服从安排","值日到位","整理公物","主动保洁","垃圾分类","摆放桌椅","积极参赛","协助班级","好人好事","板报出力","志愿服务"];
    const reasonsSub = ["迟交作业","缺交作业","课堂走神","扰乱课堂","抄袭作业","背诵未过","追逐打闹","出言不逊","迟到早退","无故旷课","乱扔杂物","喧哗吵闹","值日偷懒","卫生不合格","破坏公物","桌面脏乱","未带学具","弄虚作假"];

    const tagHtml = t => '<span class="reason-tag" style="display:inline-block;padding:4px 10px;margin:4px;font-size:12.5px;border-radius:6px;background:#f1f5f9;color:#475569;cursor:pointer;border:1px solid transparent;">'+t+'</span>';

    const box = $('modalBox');
    box.innerHTML =
      '<div class="m-hd"><h3 id="scTitle">'+ (isAdd ? '+ 加分' : '- 减分') +'</h3><button class="m-close" id="mClose">×</button></div>' +
      '<div class="m-bd">' +
        '<div style="margin-bottom:12px;font-size:14px;color:#64748b">学生：<b>'+ stu.name +'</b>（'+ (stu.group || '未分组') +' · 当前 '+ (stu.score||0) +' 分）</div>' +
        '<div style="display:flex;gap:10px;margin-bottom:16px">' +
          '<button id="opAdd" style="flex:1;height:40px;border-radius:8px;border:1px solid '+(isAdd?'#10b981':'#e2e8f0')+';background:'+(isAdd?'#ecfdf5':'#fff')+';color:'+(isAdd?'#10b981':'#475569')+';font-weight:600">+ 加分</button>' +
          '<button id="opSub" style="flex:1;height:40px;border-radius:8px;border:1px solid '+(!isAdd?'#ef4444':'#e2e8f0')+';background:'+(!isAdd?'#fef2f2':'#fff')+';color:'+(!isAdd?'#ef4444':'#475569')+';font-weight:600">- 减分</button>' +
        '</div>' +
        '<div style="display:grid;grid-template-columns:repeat(4,1fr);gap:8px;margin-bottom:16px">' +
          [1,2,3,5,10,20,50,100].map(v=>'<button class="quick" data-v="'+v+'" style="height:36px;border:1px solid #e2e8f0;border-radius:8px;background:#fff;color:#0f172a">'+v+'</button>').join('') +
        '</div>' +
        '<input type="number" id="scVal" placeholder="输入自定义分数" style="width:100%;height:40px;border:1px solid #e2e8f0;border-radius:8px;padding:0 12px;margin-bottom:16px;font-size:15px">' +
        '<div style="max-height:120px;overflow-y:auto;margin-bottom:12px;padding:4px;border:1px dashed #e2e8f0;border-radius:8px" id="reasonTags">' +
          (isAdd ? reasonsAdd : reasonsSub).map(tagHtml).join('') +
        '</div>' +
        '<textarea id="scReason" placeholder="原因（必填，可点上方标签自动填入）" style="width:100%;height:60px;border:1px solid #e2e8f0;border-radius:8px;padding:10px;resize:none;font-size:15px"></textarea>' +
      '</div>' +
      '<div class="m-ft"><button class="btn-line" id="mCancel">取消</button><button class="btn-solid" id="mSave">确认</button></div>';

    openModal();
    const textArea = $('scReason');

    function bindTags(){
      const tags = box.querySelectorAll('.reason-tag');
      tags.forEach(tag=>{
        tag.onclick = function(){
          tags.forEach(t=>{ t.style.background='#f1f5f9'; t.style.color='#475569'; t.style.borderColor='transparent'; });
          this.style.background = isAdd ? '#ecfdf5' : '#fef2f2';
          this.style.color = isAdd ? '#10b981' : '#ef4444';
          this.style.borderColor = isAdd ? '#10b981' : '#ef4444';
          textArea.value = this.innerText;
        };
      });
    }
    bindTags();

    $('opAdd').onclick = function(){
      isAdd = true;
      $('scTitle').textContent = '+ 加分';
      this.style.cssText = 'flex:1;height:40px;border-radius:8px;border:1px solid #10b981;background:#ecfdf5;color:#10b981;font-weight:600';
      $('opSub').style.cssText = 'flex:1;height:40px;border-radius:8px;border:1px solid #e2e8f0;background:#fff;color:#475569;font-weight:600';
      $('reasonTags').innerHTML = reasonsAdd.map(tagHtml).join('');
      bindTags();
    };
    $('opSub').onclick = function(){
      isAdd = false;
      $('scTitle').textContent = '- 减分';
      this.style.cssText = 'flex:1;height:40px;border-radius:8px;border:1px solid #ef4444;background:#fef2f2;color:#ef4444;font-weight:600';
      $('opAdd').style.cssText = 'flex:1;height:40px;border-radius:8px;border:1px solid #e2e8f0;background:#fff;color:#475569;font-weight:600';
      $('reasonTags').innerHTML = reasonsSub.map(tagHtml).join('');
      bindTags();
    };

    box.querySelectorAll('.quick').forEach(btn=>{
      btn.onclick = function(){
        box.querySelectorAll('.quick').forEach(b=>{ b.style.background='#fff'; b.style.color='#0f172a'; });
        this.style.background = isAdd ? '#eff6ff' : '#fef2f2';
        this.style.color = isAdd ? '#2563eb' : '#ef4444';
        $('scVal').value = this.dataset.v;
      };
    });

    $('mClose').onclick = $('mCancel').onclick = closeModal;
    $('mSave').onclick = function(){
      const val = Math.abs(Number($('scVal').value));
      const reason = $('scReason').value.trim();
      if(!val){ toast('请输入分数'); return; }
      if(!reason){ toast('请填写原因'); return; }
      const finalVal = isAdd ? val : -val;
      stu.score = (stu.score||0) + finalVal;
      if(!stu.logs) stu.logs = [];
      stu.logs.push({ time: nowStr(), delta: finalVal, reason: reason });
      closeModal();
      renderAll();
      scheduleSave();
      toast((isAdd?'加分':'减分') + '成功');
    };
  };

  /* ================= 历史记录 ================= */
  window.openHistoryModal = function(id){
    const stu = students.find(x=>x.id === id);
    if(!stu) return;
    const logs = [...(stu.logs||[])].reverse();
    const box = $('modalBox');
    box.innerHTML =
      '<div class="m-hd"><h3>'+ stu.name +' · 积分历史</h3><button class="m-close" id="mClose">×</button></div>' +
      '<div class="m-bd"><div class="hist-list">' +
        (logs.length===0 ? '<div class="empty">暂无记录</div>' : logs.map(l=>
          '<div class="hist-item"><div><div style="font-size:12px;color:#94a3b8">'+ l.time +'</div>' +
          '<div style="font-weight:500">'+ (l.reason||'') +'</div></div>' +
          '<div class="h-num '+(l.delta>0?'up':(l.delta<0?'down':''))+'">'+ (l.delta>0?'+':'') + l.delta +'</div></div>'
        ).join('')) +
      '</div></div>' +
      '<div class="m-ft"><button class="btn-line" id="mCloseBtn">关闭</button></div>';
    openModal();
    $('mClose').onclick = $('mCloseBtn').onclick = closeModal;
  };

  /* ================= 编辑学生 ================= */
  window.openEditStudent = function(id){
    const s = students.find(x=>x.id === id);
    if(!s){ toast('学生不存在'); return; }
    const box = $('modalBox');
    box.innerHTML =
      '<div class="m-hd"><h3>编辑学生信息</h3><button class="m-close" id="mClose">×</button></div>' +
      '<div class="m-bd">' +
        '<div class="f"><label>姓名</label><input id="edName" value="'+ (s.name||'').replace(/"/g,'&quot;') +'"></div>' +
        '<div style="display:flex;gap:12px">' +
          '<div class="f" style="flex:1"><label>小组</label><select id="edGroup">'+ groupOptionsHtml(s.group) +'</select></div>' +
          '<div class="f" style="flex:1"><label>性别</label><select id="edGender">' +
            '<option value=""'+(s.gender?'':' selected')+'>未填写</option>' +
            '<option value="男"'+(s.gender==='男'?' selected':'')+'>男</option>' +
            '<option value="女"'+(s.gender==='女'?' selected':'')+'>女</option>' +
          '</select></div>' +
        '</div>' +
        '<div class="f"><label>职务</label><input id="edDuty" value="'+ (s.duty||'').replace(/"/g,'&quot;') +'" placeholder="如：班长"></div>' +
        '<div class="f"><label>积分（手动修正，会生成一条记录）</label><input id="edScore" type="number" value="'+ (s.score||0) +'"></div>' +
        '<div style="font-size:12.5px;color:#94a3b8">已产生 ' + ((s.logs||[]).length) + ' 条加减分记录</div>' +
      '</div>' +
      '<div class="m-ft" style="justify-content:space-between">' +
        '<button class="btn-line btn-danger" id="edDel" style="margin-right:auto">删除该学生</button>' +
        '<button class="btn-line" id="mCancel">取消</button>' +
        '<button class="btn-solid" id="mSave">保存</button>' +
      '</div>';
    openModal();
    $('mClose').onclick = $('mCancel').onclick = closeModal;

    $('mSave').onclick = function(){
      const name = ($('edName').value || '').trim();
      if(!name){ toast('姓名不能为空'); return; }
      const newScore = Number($('edScore').value);
      const oldScore = (s.score||0);
      s.name = name;
      s.group = $('edGroup').value;
      s.gender = $('edGender').value;
      s.duty = ($('edDuty').value || '').trim();
      if(!isNaN(newScore) && newScore !== oldScore){
        if(!s.logs) s.logs = [];
        s.logs.push({ time: nowStr(), delta: newScore - oldScore, reason: '手动修正积分：' + oldScore + ' → ' + newScore });
        s.score = newScore;
      }
      closeModal();
      renderAll();
      scheduleSave();
      toast('已保存');
    };

    $('edDel').onclick = function(){
      if(!confirm('确定删除学生【' + s.name + '】？该学生的所有加减分记录也会一并删除，且不可恢复。')) return;
      students = students.filter(x=>x.id !== s.id);
      closeModal();
      renderAll();
      scheduleSave();
      toast('已删除');
    };
  };

  /* ================= 撤销记录 ================= */
  window.undoLog = function(sid, idx){
    const stu = students.find(x=>x.id === sid);
    if(!stu || !stu.logs || !stu.logs[idx]){ toast('记录不存在'); return; }
    const l = stu.logs[idx];
    const tip = l.delta === 0 ? '这条考勤记录将被删除' : ('将回退 ' + (l.delta>0?'+':'') + l.delta + ' 分');
    if(!confirm('撤销【' + (l.reason||'') + '】？\n' + tip)) return;
    stu.score = (stu.score||0) - (l.delta||0);
    stu.logs.splice(idx, 1);
    renderAll();
    scheduleSave();
    toast('已撤销');
  };

  /* ================= 新增学生 ================= */
  $('btnOpenAddStu').onclick = function(){
    const box = $('modalBox');
    box.innerHTML =
      '<div class="m-hd"><h3>新增学生</h3><button class="m-close" id="mClose">×</button></div>' +
      '<div class="m-bd">' +
        '<div class="f"><label>学生姓名</label><input id="inName" placeholder="姓名"></div>' +
        '<div style="display:flex;gap:12px">' +
          '<div class="f" style="flex:1"><label>小组</label><select id="inGroup">'+ groupOptionsHtml('') +'</select></div>' +
          '<div class="f" style="flex:1"><label>性别</label><select id="inGender"><option value="">未填写</option><option value="男">男</option><option value="女">女</option></select></div>' +
        '</div>' +
        '<div class="f"><label>职务</label><input id="inDuty" placeholder="如：班长"></div>' +
        '<div class="f"><label>初始积分</label><input id="inScore" type="number" value="0"></div>' +
      '</div>' +
      '<div class="m-ft"><button class="btn-line" id="mCancel">取消</button><button class="btn-solid" id="mSave">添加</button></div>';
    openModal();
    $('mClose').onclick = $('mCancel').onclick = closeModal;
    $('mSave').onclick = function(){
      const name = ($('inName').value || '').trim();
      if(!name){ toast('请填写姓名'); return; }
      students.push({
        id: Date.now(),
        name: name,
        group: $('inGroup').value,
        gender: $('inGender').value,
        duty: ($('inDuty').value || '').trim(),
        score: Number($('inScore').value) || 0,
        logs: [],
        exam: { ch:0, ma:0, en:0, ph:0, chm:0, bio:0 },
        attend: ''
      });
      closeModal();
      renderAll();
      scheduleSave();
      toast('已添加 ' + name);
    };
  };

  /* ================= 成绩录入 ================= */
  $('btnAddExam').onclick = function(){
    if(students.length === 0){ toast('请先添加学生'); return; }
    const box = $('modalBox');
    box.innerHTML =
      '<div class="m-hd"><h3>录入 / 修改成绩</h3><button class="m-close" id="mClose">×</button></div>' +
      '<div class="m-bd">' +
        '<div class="f"><label>选择学生</label><select id="exStu">' +
          students.map(s=>'<option value="'+s.id+'">'+s.name+'</option>').join('') +
        '</select></div>' +
        '<div style="display:flex;gap:10px">' +
          '<div class="f" style="flex:1"><label>语文</label><input id="exCh" type="number" placeholder="0"></div>' +
          '<div class="f" style="flex:1"><label>数学</label><input id="exMa" type="number" placeholder="0"></div>' +
          '<div class="f" style="flex:1"><label>英语</label><input id="exEn" type="number" placeholder="0"></div>' +
        '</div>' +
        '<div style="display:flex;gap:10px">' +
          '<div class="f" style="flex:1"><label>物理</label><input id="exPh" type="number" placeholder="0"></div>' +
          '<div class="f" style="flex:1"><label>化学</label><input id="exChm" type="number" placeholder="0"></div>' +
          '<div class="f" style="flex:1"><label>生物</label><input id="exBio" type="number" placeholder="0"></div>' +
        '</div>' +
        '<div class="f"><label>学年榜（可不填）</label><input id="exYear" type="number" placeholder="学年榜分数"></div>' +
      '</div>' +
      '<div class="m-ft"><button class="btn-line" id="mCancel">取消</button><button class="btn-solid" id="mSave">保存</button></div>';
    openModal();

    function fill(){
      const s = students.find(x=>x.id === Number($('exStu').value));
      if(!s) return;
      if(!s.exam) s.exam = { ch:0, ma:0, en:0, ph:0, chm:0, bio:0 };
      $('exCh').value = s.exam.ch || '';
      $('exMa').value = s.exam.ma || '';
      $('exEn').value = s.exam.en || '';
      $('exPh').value = s.exam.ph || '';
      $('exChm').value = s.exam.chm || '';
      $('exBio').value = s.exam.bio || '';
      $('exYear').value = (s.year === null || s.year === undefined || s.year === '') ? '' : s.year;
    }
    $('exStu').onchange = fill;
    fill();

    $('mClose').onclick = $('mCancel').onclick = closeModal;
    $('mSave').onclick = function(){
      const s = students.find(x=>x.id === Number($('exStu').value));
      if(!s){ toast('学生不存在'); return; }
      s.exam = {
        ch: Number($('exCh').value) || 0,
        ma: Number($('exMa').value) || 0,
        en: Number($('exEn').value) || 0,
        ph: Number($('exPh').value) || 0,
        chm: Number($('exChm').value) || 0,
        bio: Number($('exBio').value) || 0
      };
      const yv = ($('exYear').value || '').trim();
      s.year = yv === '' ? null : Number(yv);
      closeModal();
      renderAll();
      scheduleSave();
      toast('成绩已保存');
    };
  };

  /* ================= 作业 ================= */
  window.delHomework = function(idx){
    if(!homeworks[idx]) return;
    if(confirm('确定删除这项作业？')){
      homeworks.splice(idx, 1);
      renderHomework();
      scheduleSave();
      toast('已删除');
    }
  };

  $('btnAddHomework').onclick = function(){
    const box = $('modalBox');
    box.innerHTML =
      '<div class="m-hd"><h3>布置作业</h3><button class="m-close" id="mClose">×</button></div>' +
      '<div class="m-bd">' +
        '<div style="display:flex;gap:10px">' +
          '<div class="f" style="flex:1"><label>学科</label><select id="hwSub">' +
            ['语文','数学','英语','物理','化学','生物'].map(v=>'<option value="'+v+'">'+v+'</option>').join('') +
          '</select></div>' +
          '<div class="f" style="flex:1"><label>日期</label><input id="hwDate" type="date"></div>' +
        '</div>' +
        '<div class="f"><label>内容</label><textarea id="hwCon" placeholder="作业内容" style="width:100%;height:80px;border:1px solid #e2e8f0;border-radius:8px;padding:10px;resize:none;font-size:15px"></textarea></div>' +
      '</div>' +
      '<div class="m-ft"><button class="btn-line" id="mCancel">取消</button><button class="btn-solid" id="mSave">布置</button></div>';
    openModal();
    const d = new Date();
    $('hwDate').value = d.getFullYear() + '-' + String(d.getMonth()+1).padStart(2,'0') + '-' + String(d.getDate()).padStart(2,'0');

    $('mClose').onclick = $('mCancel').onclick = closeModal;
    $('mSave').onclick = function(){
      const content = ($('hwCon').value || '').trim();
      if(!content){ toast('请填写作业内容'); return; }
      homeworks.unshift({ date: $('hwDate').value, subject: $('hwSub').value, content: content });
      closeModal();
      renderHomework();
      scheduleSave();
      toast('已布置');
    };
  };

  /* ================= 商城 ================= */
  $('btnAddGoods').onclick = function(){
    const box = $('modalBox');
    box.innerHTML =
      '<div class="m-hd"><h3>添加奖品</h3><button class="m-close" id="mClose">×</button></div>' +
      '<div class="m-bd">' +
        '<div class="f"><label>奖品名称</label><input id="gdName" placeholder="奖品名"></div>' +
        '<div style="display:flex;gap:10px">' +
          '<div class="f" style="flex:1"><label>消耗积分</label><input id="gdCost" type="number" value="50"></div>' +
          '<div class="f" style="flex:1"><label>库存</label><input id="gdStock" type="number" value="10"></div>' +
        '</div>' +
      '</div>' +
      '<div class="m-ft"><button class="btn-line" id="mCancel">取消</button><button class="btn-solid" id="mSave">添加</button></div>';
    openModal();
    $('mClose').onclick = $('mCancel').onclick = closeModal;
    $('mSave').onclick = function(){
      const name = ($('gdName').value || '').trim();
      const cost = Number($('gdCost').value);
      const stock = Number($('gdStock').value);
      if(!name){ toast('请填写奖品名称'); return; }
      if(!cost || cost <= 0){ toast('请填写正确的积分'); return; }
      if(isNaN(stock) || stock < 0){ toast('请填写正确的库存'); return; }
      shopGoods.push({ name: name, cost: cost, stock: stock });
      closeModal();
      renderShop();
      scheduleSave();
      toast('已添加');
    };
  };

  window.openEditGoods = function(idx){
    const g = shopGoods[idx]; if(!g) return;
    const box = $('modalBox');
    box.innerHTML =
      '<div class="m-hd"><h3>编辑奖品</h3><button class="m-close" id="mClose">×</button></div>' +
      '<div class="m-bd">' +
        '<div class="f"><label>奖品名称</label><input id="egName" value="'+ (g.name||'').replace(/"/g,'&quot;') +'"></div>' +
        '<div style="display:flex;gap:10px">' +
          '<div class="f" style="flex:1"><label>消耗积分</label><input id="egCost" type="number" value="'+ (g.cost||0) +'"></div>' +
          '<div class="f" style="flex:1"><label>库存</label><input id="egStock" type="number" value="'+ (g.stock||0) +'"></div>' +
        '</div>' +
      '</div>' +
      '<div class="m-ft"><button class="btn-line" id="mCancel">取消</button><button class="btn-solid" id="mSave">保存</button></div>';
    openModal();
    $('mClose').onclick = $('mCancel').onclick = closeModal;
    $('mSave').onclick = function(){
      const name = ($('egName').value || '').trim();
      if(!name){ toast('名称不能为空'); return; }
      g.name = name;
      g.cost = Number($('egCost').value) || 0;
      g.stock = Number($('egStock').value) || 0;
      closeModal();
      renderShop();
      scheduleSave();
      toast('已保存');
    };
  };

  window.delGoods = function(idx){
    if(!shopGoods[idx]) return;
    if(!confirm('删除奖品【' + shopGoods[idx].name + '】？')) return;
    shopGoods.splice(idx, 1);
    renderShop();
    scheduleSave();
    toast('已删除');
  };

  window.openRedeemModal = function(idx){
    const goods = shopGoods[idx];
    if(!goods) return;
    const sorted = [...students].sort((a,b)=>(b.score||0)-(a.score||0));
    if(sorted.length === 0){ toast('还没有学生'); return; }
    const box = $('modalBox');
    box.innerHTML =
      '<div class="m-hd"><h3>兑换：'+ goods.name +'</h3><button class="m-close" id="mClose">×</button></div>' +
      '<div class="m-bd">' +
        '<div class="f"><label>选择学生（消耗 '+ goods.cost +' 积分）</label><select id="rdStu">' +
          sorted.map(s=>'<option value="'+s.id+'" '+(s.score < goods.cost ? 'disabled' : '')+'>'+ s.name +'（'+ (s.score||0) +'分）'+(s.score < goods.cost ? ' - 积分不足' : '')+'</option>').join('') +
        '</select></div>' +
      '</div>' +
      '<div class="m-ft"><button class="btn-line" id="mCancel">取消</button><button class="btn-solid" id="mSave">确认兑换</button></div>';
    openModal();
    $('mClose').onclick = $('mCancel').onclick = closeModal;
    $('mSave').onclick = function(){
      const stu = students.find(s=>s.id === Number($('rdStu').value));
      if(!stu){ toast('请选择学生'); return; }
      if((stu.score||0) < goods.cost){ toast('积分不足'); return; }
      stu.score -= goods.cost;
      if(!stu.logs) stu.logs = [];
      stu.logs.push({ time: nowStr(), delta: -goods.cost, reason: '兑换：' + goods.name });
      goods.stock = Math.max(0, goods.stock - 1);
      redeemLogs.unshift({ time: nowStr(), name: stu.name, goods: goods.name, cost: goods.cost });
      closeModal();
      renderAll();
      scheduleSave();
      toast('兑换成功');
    };
  };

  /* ================= 考勤 ================= */
  window.setAttend = function(id, status){
    const stu = students.find(s=>s.id === id);
    if(!stu) return;
    if(status === '请假'){
      const reason = prompt('请输入【' + stu.name + '】的请假理由：');
      if(reason === null) return;
      stu.attend = '请假(' + ((reason||'').trim() || '未说明') + ')';
      if(!stu.logs) stu.logs = [];
      stu.logs.push({ time: nowStr(), delta: 0, reason: '考勤：请假 - ' + ((reason||'').trim() || '未说明') });
    }else if(status === '旷课'){
      stu.attend = '旷课';
      stu.score = (stu.score||0) - 2;
      if(!stu.logs) stu.logs = [];
      stu.logs.push({ time: nowStr(), delta: -2, reason: '考勤：旷课' });
    }else if(status === '迟到'){
      stu.attend = '迟到';
      stu.score = (stu.score||0) - 1;
      if(!stu.logs) stu.logs = [];
      stu.logs.push({ time: nowStr(), delta: -1, reason: '考勤：迟到' });
    }else{
      stu.attend = '';
    }
    renderAll();
    scheduleSave();
  };

  $('btnAllNormal').onclick = function(){
    if(students.length === 0){ toast('还没有学生'); return; }
    students.forEach(s=>{ s.attend = ''; });
    renderAll();
    scheduleSave();
    toast('已全部设为正常');
  };

  /* ================= 搜索 & 标签切换 ================= */
  $('searchStu').addEventListener('input', renderStudentList);
  $('searchExam').addEventListener('input', renderExam);
  $('searchFeeds').addEventListener('input', renderFeeds);
  $('filterGroup').addEventListener('change', renderStudentList);

  document.querySelectorAll('.tab').forEach(tab=>{
    tab.addEventListener('click', function(){
      document.querySelectorAll('.tab').forEach(t=>t.classList.remove('on'));
      this.classList.add('on');
      document.querySelectorAll('.panel').forEach(p=>p.classList.add('hidden'));
      const target = $('panel-' + this.dataset.tab);
      if(target) target.classList.remove('hidden');
    });
  });

  /* ================= 全屏计时器 ================= */
  $('btnTimer').onclick = function(){
    if($('timerOverlay')) return;
    const div = document.createElement('div');
    div.className = 'timer-overlay';
    div.id = 'timerOverlay';
    div.innerHTML =
      '<div style="text-align:center;padding:0 16px">' +
        '<div class="timer-time" id="timerDisp">15:00</div>' +
        '<div style="margin-bottom:30px;display:flex;gap:10px;justify-content:center;flex-wrap:wrap">' +
          [1,3,5,15,40,45].map(m=>'<button class="timer-btn" data-min="'+m+'">'+m+' 分钟</button>').join('') +
        '</div>' +
        '<div style="display:flex;justify-content:center;gap:20px">' +
          '<button class="timer-btn" id="tStart" style="background:#2563eb;color:#fff">开始</button>' +
          '<button class="timer-btn" id="tClose">关闭</button>' +
        '</div>' +
      '</div>';
    document.body.appendChild(div);

    let time = 15 * 60, tick = null, isRunning = false;
    const disp = $('timerDisp');

    function update(){
      const m = String(Math.floor(time/60)).padStart(2,'0');
      const s = String(time%60).padStart(2,'0');
      disp.textContent = m + ':' + s;
    }

    div.querySelectorAll('[data-min]').forEach(btn=>{
      btn.onclick = function(){
        if(isRunning) return;
        time = parseInt(this.dataset.min, 10) * 60;
        update();
        div.querySelectorAll('[data-min]').forEach(b=>{ b.style.background='#f1f5f9'; b.style.color='#475569'; });
        this.style.background = '#e0f2fe';
        this.style.color = '#0284c7';
      };
    });

    $('tStart').onclick = function(){
      if(isRunning){
        clearInterval(tick);
        isRunning = false;
        this.textContent = '继续';
        return;
      }
      isRunning = true;
      this.textContent = '暂停';
      tick = setInterval(()=>{
        if(time <= 0){
          clearInterval(tick);
          isRunning = false;
          disp.textContent = '00:00';
          try{ alert('⏰ 时间到！'); }catch(e){}
          return;
        }
        time--;
        update();
      }, 1000);
    };

    $('tClose').onclick = function(){
      clearInterval(tick);
      div.remove();
    };

    update();
  };

  /* ================= 随机抽人 ================= */
  $('btnLucky').onclick = function(){
    if(students.length === 0){ toast('还没有学生哦'); return; }
    const box = $('modalBox');
    box.innerHTML =
      '<div class="m-hd" style="justify-content:center;padding-top:24px"><h3 style="font-size:20px;color:#2563eb">🎲 随机抽人</h3></div>' +
      '<div class="m-bd" style="text-align:center;padding:40px 20px">' +
        '<div id="luckyName" style="font-size:42px;font-weight:800;color:#2563eb;margin-bottom:20px">准备...</div>' +
        '<button class="btn-solid" id="btnStartLucky" style="font-size:18px;height:48px;border-radius:24px">开始</button>' +
        '<button class="btn-solid" id="btnStopLucky" style="display:none;font-size:18px;height:48px;background:#ef4444;border-radius:24px">停止</button>' +
      '</div>';
    openModal();

    let rolling = null;
    const nameEl = $('luckyName');

    $('btnStartLucky').onclick = function(){
      this.style.display = 'none';
      $('btnStopLucky').style.display = 'inline-block';
      nameEl.style.color = '#2563eb';
      rolling = setInterval(()=>{
        nameEl.textContent = students[Math.floor(Math.random()*students.length)].name;
      }, 50);
    };

    $('btnStopLucky').onclick = function(){
      clearInterval(rolling);
      this.style.display = 'none';
      const lucky = students[Math.floor(Math.random()*students.length)];
      nameEl.textContent = lucky.name;
      nameEl.style.color = '#e0454c';
      setTimeout(()=>{
        closeModal();
        openScoreModal(lucky.id, 'add');
      }, 900);
    };
  };

  /* ================= 批量加减 ================= */
  $('btnBatchStu').onclick = function(){
    if(students.length === 0){ toast('还没有学生'); return; }
    const box = $('modalBox');
    box.innerHTML =
      '<div class="m-hd"><h3>批量加减（全班）</h3><button class="m-close" id="mClose">×</button></div>' +
      '<div class="m-bd">' +
        '<div class="f"><label>分值（正数加分，负数减分）</label><input id="btScore" type="number" value="1"></div>' +
        '<div class="f"><label>原因</label><input id="btReason" placeholder="如：全勤、班会表现"></div>' +
        '<div style="font-size:13px;color:#94a3b8">将作用于全部 '+ students.length +' 名学生</div>' +
      '</div>' +
      '<div class="m-ft"><button class="btn-line" id="mCancel">取消</button><button class="btn-solid" id="mSave">确定</button></div>';
    openModal();
    $('mClose').onclick = $('mCancel').onclick = closeModal;
    $('mSave').onclick = function(){
      const val = Number($('btScore').value);
      const reason = ($('btReason').value || '').trim() || '批量操作';
      if(!val){ toast('请输入分值'); return; }
      students.forEach(s=>{
        s.score = (s.score||0) + val;
        if(!s.logs) s.logs = [];
        s.logs.push({ time: nowStr(), delta: val, reason: reason });
      });
      closeModal();
      renderAll();
      scheduleSave();
      toast('批量操作完成');
    };
  };

  /* ================= 班级公告 ================= */
  $('btnNotice').onclick = function(){
    const box = $('modalBox');
    box.innerHTML =
      '<div class="m-hd"><h3>班级公告</h3><button class="m-close" id="mClose">×</button></div>' +
      '<div class="m-bd">' +
        '<div class="f"><label>公告内容（保存后显示在学生榜顶部，留空则隐藏）</label><textarea id="ntText" style="width:100%;height:120px;border:1px solid #e2e8f0;border-radius:8px;padding:10px;resize:none;font-size:15px" placeholder="输入要发布的班级公告"></textarea></div>' +
      '</div>' +
      '<div class="m-ft"><button class="btn-line" id="mClear">清空</button><button class="btn-line" id="mCancel">取消</button><button class="btn-solid" id="mSave">保存公告</button></div>';
    openModal();
    $('ntText').value = notices || '';
    $('mClose').onclick = $('mCancel').onclick = closeModal;
    $('mClear').onclick = function(){ $('ntText').value = ''; };
    $('mSave').onclick = function(){
      notices = ($('ntText').value || '').trim();
      closeModal();
      renderNotice();
      scheduleSave();
      toast('公告已保存');
    };
  };

  /* ================= 个人中心 ================= */
  $('btnProfile').onclick = function(){
    const box = $('modalBox');
    box.innerHTML =
      '<div class="m-hd"><h3>个人中心</h3><button class="m-close" id="mClose">×</button></div>' +
      '<div class="m-bd">' +
        '<div class="f"><label>当前账号</label><b style="font-size:16px">'+ currentUser +'</b></div>' +
        '<div style="font-size:13px;color:#64748b;margin-bottom:16px">学生 '+ students.length +' 人 · 记录 '+
          students.reduce((n,s)=>n+((s.logs&&s.logs.length)||0),0) +' 条 · 奖品 '+ shopGoods.length +' 件</div>' +
        '<div style="display:flex;flex-direction:column;gap:8px">' +
          '<button class="btn-line" id="pfPwd">修改密码</button>' +
          '<button class="btn-line" id="pfBackup">导出数据备份（JSON）</button>' +
          '<button class="btn-line" id="pfRestore">导入数据备份（JSON）</button>' +
          '<button class="btn-line" style="color:#e0454c;background:#fff6f6" id="pfClear">清空本账号数据</button>' +
          '<button class="btn-line" id="pfLogout">退出登录</button>' +
        '</div>' +
      '</div>' +
      '<div class="m-ft"><button class="btn-line" id="mCloseBtn">关闭</button></div>';
    openModal();
    $('mClose').onclick = $('mCloseBtn').onclick = closeModal;

    $('pfPwd').onclick = function(){
      const np = prompt('请输入新密码：');
      if(np && np.trim()){
        localStorage.setItem('class_user_' + currentUser, JSON.stringify({ pwd: np.trim() }));
        toast('密码已修改');
      }
    };

    $('pfBackup').onclick = function(){
      const data = JSON.stringify({ students: students, shopGoods: shopGoods, redeemLogs: redeemLogs, homeworks: homeworks, notices: notices }, null, 2);
      const blob = new Blob([data], { type:'application/json' });
      const a = document.createElement('a');
      a.href = URL.createObjectURL(blob);
      a.download = '班级数据备份_' + new Date().toLocaleDateString().replace(/[\/\\]/g,'-') + '.json';
      a.click();
      setTimeout(()=>URL.revokeObjectURL(a.href), 3000);
      toast('备份已导出');
    };

    $('pfRestore').onclick = function(){
      jsonInput.value = '';
      jsonInput.click();
    };

    $('pfClear').onclick = async function(){
      if(!confirm('警告：将清空本账号所有学生、积分、作业、商城数据，且不可恢复，继续？')) return;
      students = []; shopGoods = []; redeemLogs = []; homeworks = []; notices = '';
      renderAll();
      await pushToCloud();
      localStorage.setItem('class_backup_' + currentUser, JSON.stringify({ students, shopGoods, redeemLogs, homeworks, notices }));
      closeModal();
      toast('已清空');
    };

    $('pfLogout').onclick = function(){
      currentUser = '';
      $('loginPass').value = '';
      $('loginUser').value = '';
      appView.classList.add('hidden');
      loginView.classList.remove('hidden');
      closeModal();
    };
  };

  /* ================= 导出报表 ================= */
  $('btnExport').onclick = function(){
    if(students.length === 0){ toast('没有数据可导出'); return; }
    let csv = '\ufeff==================================================\n';
    csv += '            班级全能管理系统 - 详细报表\n';
    csv += '            导出时间：' + nowStr() + '\n';
    csv += '==================================================\n\n';

    csv += '【第一部分：总积分排行榜】\n排名,姓名,小组,职务,当前总积分\n';
    const sortedStu = [...students].sort((a,b)=>(b.score||0)-(a.score||0));
    sortedStu.forEach((s,i)=>{
      csv += (i+1) + ',' + s.name + ',' + (s.group || '未分组') + ',' + (s.duty || '-') + ',' + (s.score||0) + '\n';
    });

    csv += '\n\n【第二部分：按小组分块明细】\n';
    const groupMap = {};
    students.forEach(s=>{
      const g = s.group || '未分组';
      if(!groupMap[g]) groupMap[g] = [];
      groupMap[g].push(s);
    });

    Object.keys(groupMap).sort().forEach(groupName=>{
      const groupStudents = groupMap[groupName].sort((a,b)=>(b.score||0)-(a.score||0));
      csv += '\n==================================================\n';
      csv += '★ 小组：【' + groupName + '】（共 ' + groupStudents.length + ' 人）\n';
      csv += '==================================================\n';

      groupStudents.forEach(s=>{
        const logs = s.logs || [];
        csv += '\n    >>> 姓名：' + s.name + ' | 职务：' + (s.duty || '无') + ' | 当前总分：' + (s.score||0) + ' 分\n';
        if(logs.length === 0){
          csv += '        （暂无加减分记录）\n';
        }else{
          csv += '        时间,变动分值,原因/备注\n';
          [...logs].reverse().forEach(l=>{
            const reason = (l.reason || '').indexOf(',') >= 0 ? '"' + l.reason + '"' : (l.reason || '');
            csv += '        ' + l.time + ',' + (l.delta > 0 ? '+' + l.delta : l.delta) + ',' + reason + '\n';
          });
        }
        csv += '    ----------------------------------------------\n';
      });
    });

    csv += '\n\n【第三部分：六科成绩表】\n姓名,学年榜,语文,数学,英语,物理,化学,生物,总分\n';
    [...students].sort((a,b)=>examTotal(b.exam)-examTotal(a.exam)).forEach(s=>{
      const e = s.exam || {};
      const yv = (s.year === null || s.year === undefined || s.year === '') ? '' : s.year;
      csv += s.name + ',' + yv + ',' + (e.ch||0) + ',' + (e.ma||0) + ',' + (e.en||0) + ',' + (e.ph||0) + ',' + (e.chm||0) + ',' + (e.bio||0) + ',' + examTotal(e) + '\n';
    });

    const blob = new Blob([csv], { type: 'text/csv;charset=utf-8;' });
    const a = document.createElement('a');
    a.href = URL.createObjectURL(blob);
    a.download = '班级报表_' + new Date().toLocaleDateString().replace(/[\/\\]/g, '-') + '.csv';
    a.click();
    setTimeout(()=>URL.revokeObjectURL(a.href), 3000);
  };

  /* ================= 考试倒计时 ================= */
  function getExamDate(){
    const v = localStorage.getItem('class_exam_date');
    if(v){
      const t = new Date(v).getTime();
      if(!isNaN(t)) return t;
    }
    const d = new Date();
    d.setDate(d.getDate() + 60);
    d.setHours(0,0,0,0);
    return d.getTime();
  }

  function updateCountdown(){
    const el = $('examCountdown');
    if(!el) return;
    const dist = getExamDate() - Date.now();
    el.textContent = (dist <= 0 ? '0' : Math.ceil(dist / 86400000)) + ' 天';
  }

  function initCountdown(){
    updateCountdown();
    if(countdownTimer) clearInterval(countdownTimer);
    countdownTimer = setInterval(updateCountdown, 60000);
  }

  $('examCountdown').addEventListener('click', function(){
    const cur = localStorage.getItem('class_exam_date') || '';
    const input = prompt('设置考试日期（格式：2027-06-07）', cur);
    if(input === null) return;
    const t = new Date(input.trim()).getTime();
    if(isNaN(t)){ toast('日期格式不正确'); return; }
    localStorage.setItem('class_exam_date', input.trim());
    updateCountdown();
    toast('考试日期已更新');
  });

  $('examName').addEventListener('blur', function(){
    localStorage.setItem('class_exam_name', (this.textContent || '').trim() || '期末考试');
  });

  (function loadExamName(){
    const v = localStorage.getItem('class_exam_name');
    if(v && $('examName')) $('examName').textContent = v;
    updateCountdown();
  })();

  /* ================= CSV 批量导入 ================= */
  const fileInput = document.createElement('input');
  fileInput.type = 'file';
  fileInput.id = 'fileCsv';
  fileInput.accept = '.csv,.txt';
  fileInput.style.display = 'none';
  document.body.appendChild(fileInput);

  $('btnOpenCsv').onclick = function(){
    fileInput.value = '';
    fileInput.click();
  };

  fileInput.onchange = function(e){
    const file = e.target.files && e.target.files[0];
    if(!file) return;
    const reader = new FileReader();
    reader.onload = function(ev){
      try{
        let text = String(ev.target.result || '');
        text = text.replace(/^\ufeff/, '');
        const rows = text.split(/\r?\n/).filter(r=>r.trim());
        if(rows.length === 0){ toast('文件为空'); return; }

        let start = 0;
        if(/姓名|name/i.test(rows[0])) start = 1;

        let added = 0;
        for(let i=start; i<rows.length; i++){
          const parts = rows[i].split(',');
          const name = (parts[0] || '').trim();
          if(!name) continue;
          const gender = (parts[1] || '').trim();
          let group = (parts[2] || '').trim();
          if(/^\d+$/.test(group)) group = '第' + group + '组';
          students.push({
            id: Date.now() + i,
            name: name,
            gender: gender,
            group: group,
            duty: (parts[3] || '').trim(),
            score: Number((parts[4] || '').trim()) || 0,
            logs: [],
            exam: { ch:0, ma:0, en:0, ph:0, chm:0, bio:0 },
            attend: ''
          });
          added++;
        }
        renderAll();
        scheduleSave();
        toast('成功导入 ' + added + ' 名学生');
      }catch(err){
        console.warn(err);
        toast('导入失败，请检查文件格式');
      }
      e.target.value = '';
    };
    reader.onerror = function(){ toast('文件读取失败'); };
    reader.readAsText(file, 'UTF-8');
  };

  /* ================= JSON 备份恢复 ================= */
  const jsonInput = document.createElement('input');
  jsonInput.type = 'file';
  jsonInput.accept = '.json';
  jsonInput.style.display = 'none';
  document.body.appendChild(jsonInput);

  jsonInput.onchange = function(e){
    const file = e.target.files && e.target.files[0];
    if(!file) return;
    const reader = new FileReader();
    reader.onload = function(ev){
      try{
        const obj = JSON.parse(String(ev.target.result || ''));
        if(!obj || typeof obj !== 'object') throw new Error('格式错误');
        if(!confirm('导入备份将覆盖当前账号的数据，继续？')){ e.target.value = ''; return; }
        students = obj.students || [];
        shopGoods = obj.shopGoods || [];
        redeemLogs = obj.redeemLogs || [];
        homeworks = obj.homeworks || [];
        notices = obj.notices || '';
        renderAll();
        scheduleSave();
        closeModal();
        toast('导入成功');
      }catch(err){
        toast('备份文件无法识别');
      }
      e.target.value = '';
    };
    reader.readAsText(file, 'UTF-8');
  };

  /* ================= 点击遮罩关闭弹窗 ================= */
  $('modalBack').addEventListener('click', function(e){
    if(e.target === this) closeModal();
  });

  /* ================= 首次渲染 ================= */
  renderAll();
});
</script>
</body>
</html>
