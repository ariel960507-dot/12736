@charset "UTF-8";
/* ==========================================================================
   css/hw07.css: 大二影展專題「這一站，青春」作業專用外部樣式表
   學號: D1445977 | 姓名: 張儷馨 | 編輯時間: 2026/11/10
   ========================================================================== */

/* 全域基礎設定 (文青復古風) */
:root {
    --bg-paper: #F7F5F0;
    --text-ink: #2C2A29;
    --accent-red: #A8382E;
    --accent-green: #3F5E4F;
    --border-retro: #D3CEBD;
}

body {
    font-family: "Noto Sans TC", "Microsoft JhengHei", sans-serif;
    background-color: var(--bg-paper);
    color: var(--text-ink);
    margin: 0;
    padding: 0;
    line-height: 1.7;
}

.font-serif-tc {
    font-family: "Noto Serif TC", "PMingLiu", serif;
}

/* 宣紙紋理背景 */
.paper-texture {
    background-color: #F7F5F0;
    background-image: radial-gradient(#E8E3D5 0.75px, transparent 0.75px);
    background-size: 16px 16px;
}

/* 導覽列與標頭 */
header {
    background-color: var(--bg-paper);
    border-bottom: 2px solid var(--text-ink);
    position: sticky;
    top: 0;
    z-index: 50;
}

nav ul {
    list-style: none;
    padding: 0;
    margin: 0;
    display: flex;
    gap: 1.5rem;
}

nav a {
    color: var(--text-ink);
    text-decoration: none;
    font-weight: 500;
    transition: color 0.2s;
}

nav a:hover, nav a:focus-visible {
    color: var(--accent-red);
}

/* 區塊卡片與排版 */
.retro-card {
    background-color: #FFFFFF;
    border: 1px solid var(--border-retro);
    box-shadow: 3px 3px 0px rgba(44, 42, 41, 0.08);
    border-radius: 0.5rem;
    padding: 1.5rem;
    margin-bottom: 1.5rem;
}

/* 題目指引要求的特定類別遷移 (對應 HW07 作業規範) */
.reading-focus {
    background-color: #f6df9d;
    color: #3e351c;
    padding: 2px 6px;
    border-radius: 2px;
}

.route-note {
    border-left: 4px solid var(--accent-red);
    padding-left: 1rem;
    margin: 1rem 0;
    background-color: #FFFDF9;
}

.report-disclaimer {
    font-style: italic;
    color: #666666;
    font-size: 0.875rem;
}

/* 表格專用樣式 (保留 CSS 框線及表頭背景) */
.retro-table {
    width: 100%;
    border-collapse: collapse;
    border: 1px solid var(--border-retro);
    margin: 1rem 0;
}

.retro-table th, .retro-table td {
    border: 1px solid var(--border-retro);
    padding: 0.75rem;
    text-align: left;
}

.retro-table th {
    background-color: #E8E3D5;
    color: var(--text-ink);
}

.retro-table td {
    background-color: #FFFFFF;
}

/* 復古徽章與裝飾 */
.stamp-badge {
    display: inline-block;
    border: 2px solid var(--accent-red);
    color: var(--accent-red);
    padding: 2px 8px;
    font-weight: 700;
    transform: rotate(-1deg);
    font-size: 0.75rem;
    background-color: #FFFDF9;
}

/* RWD 窄視窗與媒體查詢 */
@media (max-width: 768px) {
    nav ul {
        flex-direction: column;
        gap: 0.5rem;
    }
}