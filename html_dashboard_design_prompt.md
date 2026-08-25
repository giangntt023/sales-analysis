# MASTER FRONT-END ARCHITECTURE & DATA VISUALIZATION PROMPT

# PROJECT TITLE: Xóm Data Dashboard — Executive HR Performance Analytics & Strategic AI Intelligence

---

## SECTION I: SYSTEM OVERVIEW & ARCHITECTURAL PHILOSOPHY

### 1.1 Executive Summary

You are an elite Creative Front-End Architect, UI/UX Designer, and Senior Data Visualization Engineer. Your mission is to construct a production-ready, zero-dependency single-file web application named `index.html` titled **"Xóm Data Dashboard — Executive HR Performance & Strategic AI Intelligence"**.

The application serves as an interactive executive briefing dashboard summarizing a 3-year longitudinal HR and operational performance dataset (2022–2024) across 7,500 employees, 9 corporate/retail departments, and 50 store locations. The visual identity follows a **Luminous Light Glassmorphism** design aesthetic featuring a light-mode WebGL fluid shader canvas, refined typography, and 11 scroll-driven data storytelling modules powered by Chart.js, GSAP ScrollTrigger, and Lenis smooth scrolling.

### 1.2 Core Architectural Principles

* **Single-File Encapsulation:** Zero external build steps, package managers, or bundlers. The entire application resides in a single `index.html` file.
* **Declarative Data Storytelling:** Every visualization is accompanied by explicit business context, root-cause diagnostics, key quantitative insights, and strategic action plans.
* **Perceptual Performance Optimization:** Hardware-accelerated WebGL shader background, 60fps smooth scroll interpolation via Lenis, and deferred chart rendering via GSAP ScrollTrigger.
* **Strict Light-Mode Aesthetic:** Pristine off-white backdrop (`#f8fafc`), luminous glass cards (`rgba(255, 255, 255, 0.82)`), high-contrast slate typography (`#0f172a`), and vibrant accent palettes (`#0284c7`, `#10b981`, `#6366f1`, `#f59e0b`, `#ef4444`).

---

## SECTION II: STRICT MANDATORY EXECUTION RULES

### 2.1 Rule 1 — Single File Constraint

* The final output MUST be a standalone file located at `index.html`.
* You MUST NOT create secondary `.css`, `.js`, or `.json` files.
* You MUST NOT use NPM packages, Node.js scripts, or build frameworks (React, Vue, Angular, Svelte, Vite, Webpack, Parcel).

### 2.2 Rule 2 — Allowed CDN Imports

All external assets MUST be loaded via CDN script tags and CSS import statements in the HTML `<head>`:

```html
<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Xóm Data Dashboard — Executive HR Performance Analytics</title>

<!-- Font Imports: Playfair Display (Serif Title) & Plus Jakarta Sans (UI Body) -->
<style>
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,600;0,700;0,800;1,600&family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&display=swap');
</style>

<!-- Import Map for Three.js (r0.160) -->
<script type="importmap">
{
  "imports": {
    "three": "https://unpkg.com/three@0.160.0/build/three.module.js"
  }
}
</script>

<!-- Vendor CDN Libraries -->
<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/gsap.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/ScrollTrigger.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/@studio-freight/lenis@1.0.34/dist/lenis.min.js"></script>
</head>
```

### 2.3 Rule 3 — Design System Standards

* **Page Base Background:** `#f8fafc` (Light Off-White Slate).
* **Glass Cards Container:**
  * `background: rgba(255, 255, 255, 0.82);`
  * `border: 1px solid rgba(226, 232, 240, 0.9);`
  * `backdrop-filter: blur(24px); -webkit-backdrop-filter: blur(24px);`
  * `border-radius: 24px;`
  * `padding: 48px;`
  * `box-shadow: 0 20px 40px -15px rgba(15, 23, 42, 0.06), 0 0 20px rgba(255, 255, 255, 0.9) inset;`
* **Card Hover Highlight:** Top border glow line via `::before` pseudo-element:
  * `background: linear-gradient(90deg, transparent, #0284c7, transparent);`
  * `transition: left 0.6s ease;`
* **Typography Palette:**
  * Title Font: `'Playfair Display', serif`, color `#0f172a`, weight `700` or `800`.
  * Body Font: `'Plus Jakarta Sans', sans-serif`, color `#334155`, weight `400` or `500`.
  * Highlight Text / Badges: `#047857` (Emerald), `#0284c7` (Sky Blue), `#6366f1` (Indigo).

### 2.4 Rule 4 — Hardcoded Analytical Data Integrity

* Every numerical data point, department percentage, financial sum, and manager score MUST match the empirical python analysis notebook output.
* NO mock randomizers (`Math.random()`) or dummy text (`Lorem Ipsum`) are permitted.

### 2.5 Rule 5 — Structure of Storytelling Cards

Every storytelling module from Section 01 to Section 11 MUST maintain the following DOM layout structure:

```html
<div class="glass-card card-half"> <!-- or card-wide -->
    <h2 class="card-title">XX. Section Title</h2>
    <div class="story-content">
        <p class="story-insight">Insight: [Key Core Quantitative Metric & Finding]</p>
        <p class="story-detail">[2-3 sentences explaining business context, root causes, and empirical evidence]</p>
        <ul class="story-action">
            <li>[Strategic Directive 1]</li>
            <li>[Strategic Directive 2]</li>
        </ul>
    </div>
    <div class="chart-container"><canvas id="chart-id"></canvas></div>
</div>
```

---

## SECTION III: DEEP DOMAIN CONTEXT & EMPIRICAL BACKSTORY (11 SECTIONS)

### 3.1 Section 01 — The Turnover Crisis (Tỷ lệ Nghỉ việc theo Bộ phận)

* **Empirical Scope:** 7,500 total active/exited workforce records (2022–2024). Active employees = 6,009 (80.12%), Exited employees = 1,491 (**3-Year Cumulative Attrition Rate = 19.88%**).
* **Department Breakdown (9 Departments in exact empirical order):**
  * **HR:** 22.22% attrition rate (50 exits / 225 total staff).
  * **Logistics/Warehousing:** 22.20% attrition rate (333 exits / 1,500 total staff).
  * **Marketing:** 20.67% attrition rate (31 exits / 150 total staff).
  * **Fresh Produce:** 20.36% attrition rate (229 exits / 1,125 total staff).
  * **Store Operations:** 18.93% attrition rate (568 exits / 3,000 total staff - largest absolute volume).
  * **Meat/Fish & Bakery:** 18.89% attrition rate (170 exits / 900 total staff).
  * **Customer Service:** 18.67% attrition rate (28 exits / 150 total staff).
  * **Finance:** 18.67% attrition rate (42 exits / 225 total staff).
  * **IT:** 17.78% attrition rate (40 exits / 225 total staff).
* **Root-Cause Analysis:**
  1. *Logistics:* Physical exhaustion from manual sorting, heavy pallet lifting, and strict SLA shipping deadlines in non-climate-controlled warehouses.
  2. *Store Operations:* High customer-facing stress, rigid weekend shift rotations, and low relative pay.
* **Business Impact:** High turnover in frontline units creates severe operational friction, inflates replacement recruitment costs (~$4,500 per retail worker), and increases error rates in store restocking.
* **Action Plan:**
  * Deploy automated material handling equipment in logistics hubs.
  * Implement algorithmic flexible shift scheduling for retail store staff.

### 3.2 Section 02 — Compensation Matrix Paradox (Ma trận Lương & Paradox Nghỉ việc)

* **Empirical Scope:** Base salary evaluation across corporate job levels.
  * Executive Level: ~$108,000 / year
  * Senior Manager Level: ~$82,000 / year
  * Manager Level: ~$64,000 / year
  * Supervisor Level: ~$48,000 / year
  * Associate Level: ~$34,000 / year
  * Entry-Level: ~$22,600 / year
* **Departmental Average Base Salaries (9 Departments):**
  * HR: $42,674 / yr
  * Logistics/Warehousing: $37,645 / yr
  * Fresh Produce: $32,306 / yr
  * Finance: $27,694 / yr
  * Customer Service: $27,429 / yr
  * IT: $22,692 / yr
  * Store Operations: $22,627 / yr
  * Meat/Fish & Bakery: $22,591 / yr
  * Marketing: $22,572 / yr
* **Statistical Finding:** Pearson correlation coefficient between Annual Base Salary and Attrition status is moderate negative ($r = -0.3407$).
* **The Marketing Paradox:**
  * IT workers receive lower average base pay ($22,692) but maintain low attrition (17.78%).
  * Marketing staff receive competitive base pay relative to market rates, yet attrition reaches **20.67%**.
* **Root-Cause Analysis:** Compensation is a hygiene factor, not a sole motivator. Creative roles like Marketing experience turnover when career progression visibility is low and creative autonomy is restricted.
* **Action Plan:**
  * Avoid across-the-board wage increases.
  * Establish clear merit-based promotion tracks and creative project ownership in Marketing.
  * Enhance healthcare and lifestyle benefit coverage for low-base retail roles in Store Operations.

### 3.3 Section 03 — Performance Central Tendency Bias (Hiện tượng Nén Điểm Hiệu suất)

* **Empirical Scope:** Monthly performance logs (~200,000 evaluations over 36 consecutive months from 2022 to 2024).
* **Monthly Cycle Patterns:**
  * Performance ratings peak predictably in **December 2024 (3.738 / 5.0)** and **January 2022 (3.729 / 5.0)** due to year-end sprint momentum and annual KPI completion bonuses.
* **Empirical Anomaly:** Annual average ratings stay compressed within an extraordinarily narrow band (**3.68 to 3.74** across all departments).
* **Root-Cause Analysis:** **Central Tendency Bias** — Department managers assign safe, average ratings (~3.7) to avoid interpersonal conflict, employee grievances, and compensation distribution disputes. This obscures true high performers and hides chronically poor workers.
* **Action Plan:**
  * Transition from single-manager annual reviews to 360-degree multi-rater feedback loops.
  * Institute forced distribution rating curves (e.g., Top 15%, Core 70%, Bottom 15%) for department teams larger than 15 members.

### 3.4 Section 04 — The Elite Leadership Formula (Công thức Quản lý Xuất sắc)

* **Empirical Scope:** Comparative analysis between teams managed by the Top 10 Managers (led by *Miranda Murray* rating 3.81, *Lisa Wagner* rating 3.79, *Tiffany Phillips* rating 3.78) versus lower-tier managers.
* **Top 10 Managers Roster:**
  1. Miranda Murray (3.81 avg team rating)
  2. Lisa Wagner (3.79 avg team rating)
  3. Tiffany Phillips (3.78 avg team rating)
  4. Amanda Wright (3.76 avg team rating)
  5. Lauren Thompson (3.75 avg team rating)
  6. Patricia Hale (3.75 avg team rating)
  7. Lisa Perez (3.74 avg team rating)
  8. Victoria Marshall (3.74 avg team rating)
  9. Angelica Simpson (3.73 avg team rating)
  10. Cory Hale (3.72 avg team rating)
* **Comparative Performance Metrics:**
  * **Team Attrition Rate:** 18.08% under Top 10 Managers vs 20.30% under general managers.
  * **Average Productivity Index:** 1.389 under Top 10 Managers vs 1.334 under general managers.
  * **Monthly Training Hours:** 3.029 hours/month under Top Managers vs 2.781 hours/month under general managers.
  * **Overtime Hours:** Virtually identical (~8.169 hrs/mo Top Managers vs ~7.756 hrs/mo general managers).
* **Root-Cause Analysis:** Elite managers succeed through superior operational planning, structured skill training, and clear communication — NOT by forcing employee overtime burnout.
* **Action Plan:**
  * Document the operational workflows of Top 10 Managers into an enterprise "Management Playbook".
  * Create an internal Executive Mentorship Program pairing struggling managers with Top 10 leaders.

### 3.5 Section 05 — The Baseline Effect in Training (Hiệu ứng Nền trong Đào tạo)

* **Empirical Scope:** Bivariate analysis between Monthly Training Hours (`Training_Hours`) and Employee Performance Rating (`Performance_Rating`).
* **Statistical Finding:** Pearson correlation coefficient is positive ($r = 0.2394$), indicating training increases employee performance by **+9.3%** across 0 to 5+ training hours per month.
* **Managerial Baseline Effect (Comparative Curve):**
  * *Under Top 10 Managers:* Employee rating starts at **3.665** (0 hrs training) $\rightarrow$ **3.742** (1-2 hrs) $\rightarrow$ **3.851** (3-4 hrs) $\rightarrow$ **3.987** (5+ hrs).
  * *Under General Managers:* Employee rating starts at **3.577** (0 hrs training) $\rightarrow$ **3.651** (1-2 hrs) $\rightarrow$ **3.764** (3-4 hrs) $\rightarrow$ **3.910** (5+ hrs).
* **Root-Cause Analysis:** Excellent managers provide a permanent **+0.08 to +0.09 performance boost** at EVERY training duration level. Training spent on staff supervised by weak managers yields lower overall baseline efficiency.
* **Action Plan:**
  * Shift 40% of general employee training budget toward mandatory Managerial Competency & Leadership Training.

### 3.6 Section 06 — Superstore Revenue Illusion (Ảo tưởng Doanh thu Cửa hàng)

* **Empirical Scope:** Financial outcome matching between `business_outcomes.csv` and `stores.csv` across 50 retail store locations.
* **Top 5 Revenue Stores (All Superstore Formats in Major Metro Hubs):**
  1. Superstore NYC ($1.82M avg monthly sales)
  2. Superstore Los Angeles ($1.74M avg monthly sales)
  3. Superstore Houston ($1.65M avg monthly sales)
  4. Superstore Chicago ($1.58M avg monthly sales)
  5. Superstore Phoenix ($1.49M avg monthly sales)
* **Bottom 5 Revenue Stores (Standard/Express Formats in Rural/Suburban Areas):**
  * Range: $310,000 to $420,000 avg monthly sales.
* **Operational Quality Parity:** Customer Net Promoter Score (NPS ~78.2), inventory waste percentage (~2.4%), employee satisfaction, and on-time delivery rates show **less than 1% variance** between Top 5 and Bottom 5 stores.
* **Root-Cause Analysis:** Store revenue differences are **80% driven by real estate location, population density, and store footprint size**, rather than superior store management execution.
* **Action Plan:**
  * Maintain standardized store operating procedures (since service quality is uniformly high).
  * Prioritize AI-assisted real estate Site Selection models for future store expansion.

### 3.7 Section 07 — Departmental Satisfaction & Wellbeing (Chỉ số Hạnh phúc Bộ phận)

* **Empirical Scope:** Average employee satisfaction score (`Satisfaction`) across 9 departments on a 1.0 to 10.0 scale.
* **Department Ranking:**
  1. Store Operations: **7.31 / 10**
  2. Customer Service: **7.25 / 10**
  3. HR: **7.23 / 10**
  4. Finance: **7.20 / 10**
  5. IT: **7.19 / 10**
  6. Marketing: **7.19 / 10**
  7. Fresh Produce: **7.19 / 10**
  8. Meat/Fish & Bakery: **7.18 / 10**
  9. Logistics/Warehousing: **7.11 / 10** (Lowest)
* **Root-Cause Analysis:** Logistics staff experience physical exhaustion from heavy lifting, continuous warehouse movement, strict shipping deadlines, and uncomfortable temperature conditions.
* **Action Plan:**
  * Upgrade warehouse equipment (motorized pallet jacks, hydraulic lifts, ergonomic sorting stations).
  * Institute quarterly attendance wellness bonuses and scheduled fatigue relief breaks.

### 3.8 Section 08 — Middle-Management Bottleneck (Điểm nghẽn Quản lý Trung gian)

* **Empirical Scope:** Average Productivity Index (`Productivity_Index`) evaluated by job role (`Job_Role`).
* **Role Productivity Rankings:**
  * Fresh Foods Director: **1.56** (Highest)
  * Vice President: **1.51**
  * Meat/Fish & Bakery Director: **1.45**
  * Marketing Supervisor: **1.43**
  * Supply Chain Director: **1.41**
  * Chief Financial Officer: **1.41**
  * Deli Manager: **1.40**
  * Senior Sales Associate: **1.40**
  * IT Director: **1.11** (Lowest)
  * Finance Manager: **1.10** (Lowest)
* **Root-Cause Analysis:** Executive and Director roles aggregate output across whole divisions. Middle managers (Finance Manager, IT Director) are bottlenecked by manual document approvals, legacy reporting, compliance checks, and non-productive administrative meetings.
* **Action Plan:**
  * Implement Robotic Process Automation (RPA) for financial reporting and invoice matching.
  * Adopt enterprise e-signature tools to streamline document approvals.

### 3.9 Section 09 — Flight Risk: Unrecognized Talent (Nhân tài Chưa được Thăng chức)

* **Empirical Scope:** Data filter identifying high-performing employees (`Performance_Rating > 4.5`, high satisfaction) who have NEVER been promoted (`Promoted_Before == False`).
* **High-Risk Employee Candidates:**
  1. *Phạm Minh Tuấn* (Store Operations, Performance 4.82/5.0, Status: Flight Risk High)
  2. *Nguyễn Thị Thu Hà* (Logistics/Warehousing, Performance 4.78/5.0, Status: Flight Risk High)
  3. *Trần Hoàng Nam* (Fresh Produce, Performance 4.75/5.0, Status: Flight Risk High)
  4. *Lê Thị Bích Ngọc* (Customer Service, Performance 4.71/5.0, Status: Flight Risk High)
* **Root-Cause Analysis:** Outstanding contributors whose work is unrewarded by promotion represent the company's highest statistical Flight Risk. Loss of these core workers causes severe operational knowledge drain.
* **Action Plan:**
  * HR must immediately place these flagged employees into the upcoming promotion cycle or assign them paid project leadership responsibilities.

### 3.10 Section 10 — Myth of Age & Performance (Định kiến Tuổi tác & Hiệu suất)

* **Empirical Scope:** Employee age group distribution (20–29, 30–39, 40–49, 50–65 years) evaluated against performance ratings.
* **Statistical Finding:** Pearson correlation between Age and Performance is practically zero ($r = 0.0039$).
* **Age Bracket Performance Ratings:**
  * 20–29 Years: **3.71 / 5.0**
  * 30–39 Years: **3.72 / 5.0**
  * 40–49 Years: **3.71 / 5.0**
  * 50–65 Years: **3.72 / 5.0**
* **Root-Cause Analysis:** Age has zero bearing on employee performance. Younger workers bring technological agility, while mature workers bring domain expertise, reliability, and emotional composure.
* **Action Plan:**
  * Maintain age-neutral hiring practices.
  * Form cross-generational pairing teams to blend technical speed with institutional knowledge.

### 3.11 Section 11 — AI Integration & Strategic Workforce Restructuring (Chiến lược Cắt giảm & Tái đầu tư AI)

* **Empirical Scope:** Identifying redundant frontline roles susceptible to automation (`Job_Role == 'Cashier'`) with low performance (`Performance_Rating < 3.5`) and low productivity (`Productivity_Index < 1.3`).
* **Capital Recovery Financial Projection:**
  * Laying off 343 underperforming cashiers (Performance < 3.5, Productivity < 1.3) releases **$7.81 Million ($7,809,561.34) in annual base salary capital**.
* **3-Tier Workforce Restructuring Strategy:**
  1. **Group A (Restructure & Layoff):** 343 low-performing cashiers (Performance < 3.5, Productivity < 1.3). Terminate contracts to immediately recover $7.81M payroll capital for AI Self-checkout CapEx.
  2. **Group B (Reskill & Retain):** 657 high-performing cashiers (Performance >= 3.5, Productivity >= 1.3). Retrain them into high-touch *Personal Customer Advisors* and *Self-checkout Area Supervisors*.
  3. **Group C (Augment with AI):** 350 middle managers (Finance/IT). Deploy Agentic AI / RPA software to automate administrative reporting and workflow approvals.
* **4-Phase Rollout Plan:**
  * *Phase 1:* Restructure Group A cashiers to unlock capital.
  * *Phase 2:* Pilot Self-checkout kiosks in high-density urban Superstores.
  * *Phase 3:* Execute reskilling programs for Group B cashiers into customer consultation roles.
  * *Phase 4:* Deploy enterprise AI Agents to streamline middle-management administrative tasks.

---

## SECTION IV: COMPLETE SYSTEM SOURCE CODE SPECIFICATIONS

### 4.1 HTML Document Layout

```html
<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Xóm Data Dashboard — HR & Strategic Analytics</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,600;0,700;0,800;1,600&family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&display=swap');

/* CSS STYLESHEET GOES HERE */
</style>
<script type="importmap">
{
  "imports": {
    "three": "https://unpkg.com/three@0.160.0/build/three.module.js"
  }
}
</script>
<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/gsap.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/ScrollTrigger.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/@studio-freight/lenis@1.0.34/dist/lenis.min.js"></script>
</head>
<body>

<div class="cursor-inner"></div>
<div class="cursor-outer"></div>
<canvas id="webgl-bg"></canvas>

<div class="ui-layer">
    <!-- Header -->
    <div class="main-header">
        <div class="slide-subtitle">Báo Cáo Phân Tích Hiệu Suất & Chiến Lược AI (2022–2024)</div>
        <h1 class="slide-title">Xóm Data Dashboard</h1>
    </div>

    <!-- 01. Turnover -->
    <div class="glass-card card-half">
        <h2 class="card-title">01. The Turnover Crisis</h2>
        <div class="story-content">
            <p class="story-insight">Insight: Khối HR (22.22%) và Logistics (22.20%) đang dẫn đầu về làn sóng rời bỏ tổ chức.</p>
            <p class="story-detail">Dù Store Operations có tỷ lệ nghỉ việc thấp hơn (18.93%), nhưng với quy mô nhân sự khổng lồ, bộ phận này đã mất đi tới 568 người trong 3 năm. Sự đứt gãy ở cấp độ vận hành tạo ra lỗ hổng khổng lồ về chi phí tuyển dụng thay thế.</p>
            <ul class="story-action">
                <li>Tập trung cải thiện môi trường kho bãi (Logistics) khắc nghiệt.</li>
                <li>Thiết lập chính sách ca kíp linh hoạt cho bộ phận cửa hàng (Store Ops).</li>
            </ul>
        </div>
        <div class="chart-container"><canvas id="chart-attrition"></canvas></div>
    </div>

    <!-- 02. Salary -->
    <div class="glass-card card-half">
        <h2 class="card-title">02. Compensation Matrix Paradox</h2>
        <div class="story-content">
            <p class="story-insight">Insight: Lương cao làm giảm tỷ lệ nghỉ việc ở khối IT, nhưng hoàn toàn vô tác dụng ở khối Marketing.</p>
            <p class="story-detail">Mức lương phân cấp rõ rệt theo hình kim tự tháp (Executive đạt ~$108k/năm, Entry đạt ~$22.6k/năm). Bộ phận Marketing có mức lương khá cao nhưng tỷ lệ nghỉ việc vẫn chạm mốc 20.67%, cho thấy tiền bạc không phải là yếu tố giữ chân duy nhất.</p>
            <ul class="story-action">
                <li>Không tăng lương đồng loạt. Thiết kế lộ trình phát triển nghề nghiệp rõ ràng cho khối Marketing.</li>
            </ul>
        </div>
        <div class="chart-container"><canvas id="chart-salary"></canvas></div>
    </div>

    <!-- 03. Peak Performance -->
    <div class="glass-card card-wide">
        <h2 class="card-title">03. Performance Central Tendency Bias</h2>
        <div class="story-content">
            <p class="story-insight">Insight: Đỉnh hiệu suất luôn rơi vào Tháng 12, nhưng biên độ dao động cả năm lại hẹp đến mức bất thường (3.68 - 3.74).</p>
            <p class="story-detail">Hiệu suất đạt đỉnh vào cuối năm do hiệu ứng "chạy nước rút" KPI. Tuy nhiên, sự biến động quá nhỏ của điểm số phản ánh Lỗi trung bình hóa (Central Tendency Bias) — quản lý đang chấm điểm an toàn cho mọi người, gây khó khăn cho việc nhận diện nhân tài thực sự.</p>
            <ul class="story-action">
                <li>Áp dụng đánh giá 360 độ hoặc phương pháp phân phối chuẩn bắt buộc (forced distribution) cho các nhóm quy mô lớn.</li>
            </ul>
        </div>
        <div class="chart-container" style="height: 350px;"><canvas id="chart-peak-perf"></canvas></div>
    </div>

    <!-- 04. Top Managers -->
    <div class="glass-card card-wide">
        <h2 class="card-title">04. The Elite Leadership Formula</h2>
        <div class="story-content">
            <p class="story-insight">Insight: Top 10 Quản lý xuất sắc nhất không "bóc lột" nhân viên bằng cách ép tăng ca.</p>
            <p class="story-detail">Nhóm nhân sự dưới quyền Top 10 Quản lý (đứng đầu là Miranda Murray và Lisa Wagner) có tỷ lệ nghỉ việc cực thấp (18.08%), năng suất vượt trội (1.389) và giờ làm thêm không tăng đáng kể. Họ chiến thắng nhờ việc tối ưu hóa quy trình và thời lượng đào tạo (3.029 giờ/tháng).</p>
            <ul class="story-action">
                <li>Xây dựng chương trình Mentorship nội bộ, nhân rộng "Management Playbook" từ Top 10 Quản lý này.</li>
            </ul>
        </div>
        <div class="chart-container" style="height: 450px;"><canvas id="chart-top-managers"></canvas></div>
    </div>

    <!-- 05. Training (Baseline) -->
    <div class="glass-card card-wide">
        <h2 class="card-title">05. The Baseline Effect in Training</h2>
        <div class="story-content">
            <p class="story-insight">Insight: Đào tạo nâng tầm nhân sự đồng đều (+9.3%), nhưng "Hiệu ứng Quản lý" mới là yếu tố tạo ra cách biệt vĩnh viễn.</p>
            <p class="story-detail">Dữ liệu cho thấy dưới quyền quản lý giỏi, nhân viên luôn có điểm xuất phát (baseline) hiệu suất cao hơn từ 0.08 - 0.09 điểm ở MỌI MỨC độ đào tạo. Việc đổ tiền đào tạo nhân viên sẽ lãng phí nếu quản lý trực tiếp có năng lực kém.</p>
            <ul class="story-action">
                <li>Dịch chuyển ngân sách sang đào tạo Kỹ năng Quản trị (Management Training) song song với chuyên môn nghiệp vụ.</li>
            </ul>
        </div>
        <div class="chart-container" style="height: 450px;"><canvas id="chart-training"></canvas></div>
    </div>

    <!-- 06. Stores -->
    <div class="glass-card card-wide">
        <h2 class="card-title">06. Superstore Revenue Illusion</h2>
        <div class="story-content">
            <p class="story-insight">Insight: Doanh thu khổng lồ của Top 5 cửa hàng không đến từ chất lượng dịch vụ vượt trội.</p>
            <p class="story-detail">Top 5 cửa hàng tại các siêu đô thị (New York, LA) có doanh thu gấp 3-4 lần nhóm dưới. Tuy nhiên, các chỉ số chất lượng dịch vụ (NPS, độ hài lòng) giữa nhóm cao nhất và thấp nhất gần như tương đồng tuyệt đối (chênh lệch dưới 1%).</p>
            <ul class="story-action">
                <li>Ưu tiên nguồn lực cho phân tích địa điểm (Site Selection) thay vì thay đổi quy trình vận hành đang rất ổn định.</li>
            </ul>
        </div>
        <div class="chart-container" style="height: 400px;"><canvas id="chart-stores"></canvas></div>
    </div>

    <!-- 07. Satisfaction -->
    <div class="glass-card card-half">
        <h2 class="card-title">07. Departmental Satisfaction</h2>
        <div class="story-content">
            <p class="story-insight">Insight: Hậu cần (Logistics) là tâm điểm của sự kiệt sức.</p>
            <p class="story-detail">Ngược lại với mức lương thấp nhất nhưng điểm hạnh phúc cao nhất của khối Store Ops (7.31), khối Logistics ghi nhận mức độ hài lòng chạm đáy (7.11) do đặc thù công việc nặng nhọc và môi trường khắc nghiệt.</p>
            <ul class="story-action">
                <li>Đầu tư công cụ nâng hạ hiện đại và các gói thưởng chuyên cần ngắn hạn cho nhân sự kho bãi.</li>
            </ul>
        </div>
        <div class="chart-container"><canvas id="chart-satisfaction"></canvas></div>
    </div>

    <!-- 08. Productivity -->
    <div class="glass-card card-half">
        <h2 class="card-title">08. Middle-Management Bottleneck</h2>
        <div class="story-content">
            <p class="story-insight">Insight: Quản lý cấp trung (Finance/IT) đang bị nghẽn năng suất nghiêm trọng bởi công việc hành chính.</p>
            <p class="story-detail">Trong khi Fresh Foods Director (1.56) dẫn đầu về năng suất, thì Finance Manager (1.10) lại tụt hậu. Quản lý cấp trung đang tốn quá nhiều thời gian cho việc phê duyệt thủ công và báo cáo phi sản xuất.</p>
            <ul class="story-action">
                <li>Triển khai hệ thống RPA (Robotic Process Automation) và chữ ký số E-signature để giải phóng thời gian.</li>
            </ul>
        </div>
        <div class="chart-container"><canvas id="chart-productivity"></canvas></div>
    </div>

    <!-- 09. Promotions -->
    <div class="glass-card card-half">
        <h2 class="card-title">09. Flight Risk: Unrecognized Talent</h2>
        <div class="story-content">
            <p class="story-insight">Insight: Tổ chức đang bỏ quên những nhân sự cốt lõi có điểm hiệu suất tiệm cận tuyệt đối (4.6 - 4.8).</p>
            <p class="story-detail">Danh sách những cá nhân có điểm tích hợp hiệu suất - gắn kết tốt nhất nhưng chưa TỪNG được thăng chức. Đây là nhóm có nguy cơ rời bỏ tổ chức (Flight Risk) cao nhất.</p>
            <table class="promo-table">
                <thead>
                    <tr><th>Họ và Tên</th><th>Bộ Phận</th><th>Điểm Đánh Giá</th><th>Trạng Thái</th></tr>
                </thead>
                <tbody>
                    <tr><td>Phạm Minh Tuấn</td><td>Store Operations</td><td>4.82 / 5.0</td><td><span class="promo-badge">Flight Risk Cao</span></td></tr>
                    <tr><td>Nguyễn Thị Thu Hà</td><td>Logistics/Warehousing</td><td>4.78 / 5.0</td><td><span class="promo-badge">Flight Risk Cao</span></td></tr>
                    <tr><td>Trần Hoàng Nam</td><td>Fresh Produce</td><td>4.75 / 5.0</td><td><span class="promo-badge">Flight Risk Cao</span></td></tr>
                    <tr><td>Lê Thị Bích Ngọc</td><td>Customer Service</td><td>4.71 / 5.0</td><td><span class="promo-badge">Flight Risk Cao</span></td></tr>
                </tbody>
            </table>
        </div>
    </div>

    <!-- 10. Age -->
    <div class="glass-card card-half">
        <h2 class="card-title">10. Myth of Age & Performance</h2>
        <div class="story-content">
            <p class="story-insight">Insight: Tuổi tác hoàn toàn KHÔNG liên quan đến hiệu suất làm việc (r = 0.0039).</p>
            <p class="story-detail">Sự phân phối hiệu suất đồng đều ở mọi nhóm tuổi phá vỡ định kiến về nhân sự lớn tuổi. Kinh nghiệm và sự ổn định của họ bù đắp hoàn hảo cho sự nhạy bén công nghệ của giới trẻ.</p>
            <ul class="story-action">
                <li>Tiếp tục duy trì chính sách lao động đa thế hệ và xây dựng "Cross-generational teams".</li>
            </ul>
        </div>
        <div class="chart-container"><canvas id="chart-age"></canvas></div>
    </div>

    <!-- 11. AI Strategy -->
    <div class="glass-card card-wide">
        <h2 class="card-title">11. AI Integration & Restructuring</h2>
        <div class="story-content">
            <p class="story-insight">Insight: Tinh giản 343 Thu ngân kém hiệu quả để giải phóng dòng vốn $7.81M ($7,809,561.34) đầu tư cho AI Self-checkout.</p>
            <p class="story-detail">Chiến lược chia khối Thu ngân thành 3 nhóm: Nhóm A (Hiệu suất < 3.5) sẽ bị tinh giản ngay lập tức để thu hồi vốn. Nhóm B và C (Hiệu suất cao) được giữ lại để đào tạo chuyển đổi (Reskill) thành vai trò Chăm sóc khách hàng hoặc Giám sát quầy tự động.</p>
            <ul class="story-action">
                <li>Giai đoạn 1: Lắp đặt Self-checkout tại các siêu đô thị lớn.</li>
                <li>Giai đoạn 2: Tích hợp AI Agents tự động hóa báo cáo cho khối Finance/IT.</li>
            </ul>
        </div>
        <div class="chart-container" style="height: 450px;"><canvas id="chart-ai"></canvas></div>
    </div>
</div>

<script type="module">
/* JAVASCRIPT LOGIC GOES HERE */
</script>
</body>
</html>
```

### 4.2 Complete CSS Stylesheet

```css
/* Reset & Base Setup */
* { margin: 0; padding: 0; box-sizing: border-box; user-select: none; cursor: none !important; }
html, body { 
    width: 100%; 
    background-color: #f8fafc; 
    color: #0f172a; 
    font-family: 'Plus Jakarta Sans', -apple-system, BlinkMacSystemFont, sans-serif; 
    overflow-x: hidden; 
    -ms-overflow-style: none; 
    scrollbar-width: none; 
}
::-webkit-scrollbar { display: none; width: 0; }

/* Canvas Background */
#webgl-bg { 
    position: fixed; 
    top: 0; 
    left: 0; 
    width: 100%; 
    height: 100%; 
    z-index: 1; 
    pointer-events: none; 
}

/* Custom Accent Cursor */
.cursor-inner { 
    position: fixed; top: 0; left: 0; width: 6px; height: 6px; 
    background: #0284c7; border-radius: 50%; 
    transform: translate(-50%, -50%); pointer-events: none; z-index: 9999; 
}
.cursor-outer { 
    position: fixed; top: 0; left: 0; width: 44px; height: 44px; 
    border: 1.5px solid rgba(2, 132, 199, 0.4); border-radius: 50%; 
    transform: translate(-50%, -50%); pointer-events: none; z-index: 9998; 
    transition: width 0.2s, height 0.2s, background 0.2s; 
}

/* Layout Grid System */
.ui-layer { 
    position: relative; z-index: 10; width: 100%; max-width: 1400px; 
    margin: 0 auto; padding: 100px 40px; 
    display: grid; grid-template-columns: repeat(12, 1fr); gap: 40px; 
}

/* Main Header Typography */
.main-header { grid-column: span 12; margin-bottom: 80px; text-align: center; }
.slide-title { 
    font-family: 'Playfair Display', serif; font-size: 84px; font-weight: 800; 
    color: #0f172a; letter-spacing: -1.5px; line-height: 1.1; margin-bottom: 20px; 
}
.slide-subtitle { 
    font-size: 15px; font-weight: 800; letter-spacing: 5px; text-transform: uppercase; 
    background: linear-gradient(135deg, #0284c7, #6366f1); 
    -webkit-background-clip: text; -webkit-text-fill-color: transparent; 
}

/* Glassmorphic Card Components */
.glass-card { 
    background: rgba(255, 255, 255, 0.82); 
    border: 1px solid rgba(226, 232, 240, 0.9);
    backdrop-filter: blur(24px); -webkit-backdrop-filter: blur(24px);
    border-radius: 24px; padding: 48px; 
    box-shadow: 0 20px 40px -15px rgba(15, 23, 42, 0.06), 0 0 20px rgba(255, 255, 255, 0.9) inset;
    opacity: 0; transform: translateY(70px);
    position: relative; overflow: hidden;
    transition: transform 0.4s cubic-bezier(0.16, 1, 0.3, 1), box-shadow 0.4s ease;
}
.glass-card::before {
    content: ''; position: absolute; top: 0; left: -100%; width: 50%; height: 2px;
    background: linear-gradient(90deg, transparent, #0284c7, transparent);
    transition: left 0.6s ease;
}
.glass-card:hover { 
    transform: translateY(-4px); 
    box-shadow: 0 30px 60px -20px rgba(14, 165, 233, 0.15); 
}
.glass-card:hover::before { left: 100%; }

.card-wide { grid-column: span 12; }
.card-half { grid-column: span 6; }
.card-title { 
    font-family: 'Playfair Display', serif; font-size: 32px; color: #0f172a; 
    margin-bottom: 22px; font-weight: 700; 
}
.chart-container { position: relative; width: 100%; height: 400px; margin-top: 25px; }

/* Storytelling Formatting Classes */
.story-content { display: flex; flex-direction: column; gap: 14px; margin-bottom: 25px; }
.story-insight { 
    font-size: 16.5px; color: #047857; font-weight: 700; line-height: 1.5; 
    border-left: 4px solid #10b981; padding: 8px 12px 8px 16px; 
    background: rgba(16, 185, 129, 0.06); border-radius: 0 8px 8px 0; 
}
.story-detail { font-size: 15.5px; color: #334155; line-height: 1.7; font-weight: 400; }
.story-action { list-style: none; padding-left: 0; margin-top: 8px; }
.story-action li { 
    font-size: 14.5px; color: #475569; margin-bottom: 10px; 
    display: flex; align-items: flex-start; font-weight: 500; 
}
.story-action li::before { 
    content: '→'; color: #0284c7; margin-right: 10px; font-weight: 800; font-size: 16px; 
}

/* Table Formatting for Promotion Targets */
.promo-table { width: 100%; border-collapse: collapse; margin-top: 15px; }
.promo-table th { text-align: left; padding: 12px; color: #0284c7; font-size: 13px; text-transform: uppercase; letter-spacing: 1px; border-bottom: 2px solid #e2e8f0; }
.promo-table td { padding: 12px; font-size: 14.5px; color: #1e293b; border-bottom: 1px solid #f1f5f9; }
.promo-badge { background: #fee2e2; color: #dc2626; padding: 4px 10px; border-radius: 12px; font-size: 12px; font-weight: 700; }

/* Responsive Adjustments */
@media (max-width: 1024px) {
    .ui-layer { padding: 60px 20px; gap: 24px; }
    .card-wide, .card-half { grid-column: span 12 !important; }
    .slide-title { font-size: 52px !important; }
    .glass-card { padding: 32px 20px; }
}

@media (hover: none) and (pointer: coarse) {
    .cursor-inner, .cursor-outer { display: none !important; }
    * { cursor: auto !important; }
}
```

### 4.3 Complete JavaScript Application Logic

```javascript
import * as THREE from 'three';

// 1. Lenis Smooth Scroll Engine
const lenis = new Lenis({ duration: 1.2, easing: (t) => Math.min(1, 1.001 - Math.pow(2, -10 * t)) });
function raf(time) { lenis.raf(time); requestAnimationFrame(raf); }
requestAnimationFrame(raf);

// 2. Interactive Pointer Tracking
const cursorInner = document.querySelector('.cursor-inner');
const cursorOuter = document.querySelector('.cursor-outer');
let mouseX = 0, mouseY = 0;
window.addEventListener('mousemove', (e) => {
    mouseX = e.clientX; mouseY = e.clientY;
    cursorInner.style.left = `${mouseX}px`;
    cursorInner.style.top = `${mouseY}px`;
    gsap.to(cursorOuter, { left: mouseX, top: mouseY, duration: 0.15, ease: 'power2.out' });
});

// 3. Three.js WebGL Light Luminous Fluid Shader
const canvas = document.getElementById('webgl-bg');
const scene = new THREE.Scene();
const camera = new THREE.OrthographicCamera(-1, 1, 1, -1, 0, 1);
const renderer = new THREE.WebGLRenderer({ canvas, antialias: true, alpha: true });
renderer.setSize(window.innerWidth, window.innerHeight);
renderer.setPixelRatio(Math.min(window.devicePixelRatio, 2));

const shaderUniforms = {
    uTime: { value: 0 },
    uScroll: { value: 0 },
    uMouse: { value: new THREE.Vector2(0, 0) }
};

const vertexShader = `
varying vec2 vUv;
void main() {
    vUv = uv;
    gl_Position = vec4(position, 1.0);
}
`;

const fragmentShader = `
uniform float uTime;
uniform float uScroll;
uniform vec2 uMouse;
varying vec2 vUv;

vec3 mod289(vec3 x) { return x - floor(x * (1.0 / 289.0)) * 289.0; }
vec4 mod289(vec4 x) { return x - floor(x * (1.0 / 289.0)) * 289.0; }
vec4 permute(vec4 x) { return mod289(((x*34.0)+1.0)*x); }
vec4 taylorInvSqrt(vec4 r) { return 1.79284291400159 - 0.85373472095314 * r; }

float snoise(vec3 v) {
  const vec2 C = vec2(1.0/6.0, 1.0/3.0);
  const vec4 D = vec4(0.0, 0.5, 1.0, 2.0);
  vec3 i  = floor(v + dot(v, C.yyy));
  vec3 x0 = v - i + dot(i, C.xxx);
  vec3 g = step(x0.yzx, x0.xyz);
  vec3 l = 1.0 - g;
  vec3 i1 = min(g.xyz, l.zxy);
  vec3 i2 = max(g.xyz, l.zxy);
  vec3 x1 = x0 - i1 + C.xxx;
  vec3 x2 = x0 - i2 + C.yyy;
  vec3 x3 = x0 - D.yyy;
  i = mod289(i);
  vec4 p = permute(permute(permute(
             i.z + vec4(0.0, i1.z, i2.z, 1.0))
           + i.y + vec4(0.0, i1.y, i2.y, 1.0))
           + i.x + vec4(0.0, i1.x, i2.x, 1.0));
  float n_ = 0.142857142857;
  vec3  ns = n_ * D.wyz - D.xzx;
  vec4 j = p - 49.0 * floor(p * ns.z * ns.z);
  vec4 x_ = floor(j * ns.z);
  vec4 y_ = floor(j - 7.0 * x_);
  vec4 x = x_ *ns.x + ns.yyyy;
  vec4 y = y_ *ns.x + ns.yyyy;
  vec4 h = 1.0 - abs(x) - abs(y);
  vec4 b0 = vec4(x.xy, y.xy);
  vec4 b1 = vec4(x.zw, y.zw);
  vec4 s0 = floor(b0)*2.0 + 1.0;
  vec4 s1 = floor(b1)*2.0 + 1.0;
  vec4 sh = -step(h, vec4(0.0));
  vec4 a0 = b0.xzyw + s0.xzyw*sh.xxyy;
  vec4 a1 = b1.xzyw + s1.xzyw*sh.zzww;
  vec3 p0 = vec3(a0.xy,h.x);
  vec3 p1 = vec3(a0.zw,h.y);
  vec3 p2 = vec3(a1.xy,h.z);
  vec3 p3 = vec3(a1.zw,h.w);
  vec4 norm = taylorInvSqrt(vec4(dot(p0,p0), dot(p1,p1), dot(p2, p2), dot(p3,p3)));
  p0 *= norm.x; p1 *= norm.y; p2 *= norm.z; p3 *= norm.w;
  vec4 m = max(0.6 - vec4(dot(x0,x0), dot(x1,x1), dot(x2,x2), dot(x3,x3)), 0.0);
  m = m * m;
  return 42.0 * dot(m*m, vec4(dot(p0,x0), dot(p1,x1), dot(p2,x2), dot(p3,x3)));
}

void main() {
    vec2 uv = vUv;
    float time = uTime * 0.08;
  
    vec2 warpedUv = uv * 2.5;
    float scrollDeform = uScroll * 1.2;
    float mouseDeformX = uMouse.x * 0.3;
    float mouseDeformY = uMouse.y * 0.3;

    float n = snoise(vec3(warpedUv.x + time + mouseDeformX, warpedUv.y - time + mouseDeformY, scrollDeform));
    float lines = sin(n * 12.0 + uScroll * 8.0) * 0.5 + 0.5;
    lines = pow(lines, 2.5);
  
    vec3 cBase = vec3(0.97, 0.98, 0.99); 
    vec3 cFluid1 = vec3(0.88, 0.95, 1.0);  
    vec3 cFluid2 = vec3(0.82, 0.98, 0.94);  
    vec3 highlight = mix(vec3(0.02, 0.52, 0.78), vec3(0.96, 0.62, 0.04), uScroll);
  
    vec3 color = mix(cBase, cFluid1, uv.y + n * 0.25);
    color = mix(color, cFluid2, lines * 0.35);
    color += highlight * lines * 0.15;
  
    float vignette = 1.0 - dot(uv - 0.5, uv - 0.5) * 0.6;
    gl_FragColor = vec4(color * vignette, 1.0);
}
`;

const bgGeometry = new THREE.PlaneGeometry(2, 2);
const bgMaterial = new THREE.ShaderMaterial({ vertexShader, fragmentShader, uniforms: shaderUniforms, depthWrite: false });
scene.add(new THREE.Mesh(bgGeometry, bgMaterial));

const clock = new THREE.Clock();
function animate() {
    shaderUniforms.uTime.value = clock.getElapsedTime();
    shaderUniforms.uScroll.value = window.scrollY / (document.body.scrollHeight - window.innerHeight || 1);
    shaderUniforms.uMouse.value.set(mouseX / window.innerWidth, mouseY / window.innerHeight);
    renderer.render(scene, camera);
    requestAnimationFrame(animate);
}
animate();

window.addEventListener('resize', () => {
    renderer.setSize(window.innerWidth, window.innerHeight);
});

// 4. Hardcoded Data Payload (Matching Empirical Notebook Outputs Exactly)
const DATA = {
    q1_turnover: {
        labels: ["HR", "Logistics/Warehousing", "Marketing", "Fresh Produce", "Store Operations", "Meat/Fish & Bakery", "Customer Service", "Finance", "IT"],
        data: [22.22, 22.20, 20.67, 20.36, 18.93, 18.89, 18.67, 18.67, 17.78]
    },
    q2_salary: {
        labels: ["HR", "Logistics/Warehousing", "Fresh Produce", "Finance", "Customer Service", "IT", "Store Operations", "Meat/Fish & Bakery", "Marketing"],
        data: [42674, 37645, 32306, 27694, 27429, 22692, 22627, 22591, 22572]
    },
    q3_peak: {
        labels: ["T1", "T2", "T3", "T4", "T5", "T6", "T7", "T8", "T9", "T10", "T11", "T12"],
        y2022: [3.729, 3.691, 3.705, 3.684, 3.712, 3.715, 3.720, 3.722, 3.725, 3.728, 3.730, 3.735],
        y2024: [3.710, 3.712, 3.708, 3.695, 3.715, 3.718, 3.722, 3.726, 3.731, 3.733, 3.735, 3.738]
    },
    q4_managers: {
        labels: ["Miranda Murray", "Lisa Wagner", "Tiffany Phillips", "Amanda Wright", "Lauren Thompson", "Patricia Hale", "Lisa Perez", "Victoria Marshall", "Angelica Simpson", "Cory Hale"],
        data: [3.81, 3.79, 3.78, 3.76, 3.75, 3.75, 3.74, 3.74, 3.73, 3.72]
    },
    q5_training: {
        labels: ["0 Giờ", "1-2 Giờ", "3-4 Giờ", "5+ Giờ"],
        topManagers: [3.665, 3.742, 3.851, 3.987],
        avgManagers: [3.577, 3.651, 3.764, 3.910]
    },
    q6_stores: {
        top5Stores: ["Superstore NYC", "Superstore LA", "Superstore Houston", "Superstore Chicago", "Superstore Phoenix"],
        top5Sales: [1.82, 1.74, 1.65, 1.58, 1.49]
    },
    q7_satisfaction: {
        labels: ["Store Operations", "Customer Service", "HR", "Finance", "IT", "Marketing", "Fresh Produce", "Meat/Fish & Bakery", "Logistics/Warehousing"],
        data: [7.31, 7.25, 7.23, 7.20, 7.19, 7.19, 7.19, 7.18, 7.11]
    },
    q8_productivity: {
        labels: ["Fresh Foods Dir.", "Vice President", "Meat/Bakery Dir.", "Marketing Supv.", "Supply Chain Dir.", "CFO", "Deli Manager", "Senior Sales Assoc.", "IT Director", "Finance Manager"],
        data: [1.56, 1.51, 1.45, 1.43, 1.41, 1.41, 1.40, 1.40, 1.11, 1.10]
    },
    q10_age: {
        labels: ["20-29 Tuổi", "30-39 Tuổi", "40-49 Tuổi", "50-65 Tuổi"],
        perf: [3.71, 3.72, 3.71, 3.72]
    },
    q11_ai: {
        labels: ["Nhóm A: Thu ngân kém (Sa thải 343 người)", "Nhóm B: Thu ngân giỏi (Reskill CSKH 657 người)", "Nhóm C: Quản lý (AI Augment 350 người)"],
        headcount: [343, 657, 350]
    }
};

// 5. Chart.js Global Initialization & 11 Explicit Instantiations
Chart.defaults.color = '#475569';
Chart.defaults.font.family = "'Plus Jakarta Sans', sans-serif";
Chart.defaults.font.weight = '600';

function createGradient(ctx, colorStart, colorEnd) {
    const grad = ctx.createLinearGradient(0, 0, 0, 300);
    grad.addColorStop(0, colorStart);
    grad.addColorStop(1, colorEnd);
    return grad;
}

const defaultOptions = {
    responsive: true,
    maintainAspectRatio: false,
    plugins: {
        legend: { labels: { color: '#0f172a', font: { size: 13, weight: '700' } } },
        tooltip: {
            backgroundColor: '#0f172a',
            titleColor: '#ffffff',
            bodyColor: '#cbd5e1',
            borderColor: '#334155',
            borderWidth: 1,
            padding: 12,
            cornerRadius: 8
        }
    },
    scales: {
        x: { grid: { color: 'rgba(226, 232, 240, 0.6)' }, ticks: { color: '#475569' } },
        y: { grid: { color: 'rgba(226, 232, 240, 0.6)' }, ticks: { color: '#475569' } }
    }
};

// Chart 1: Attrition Rate by Department
const ctx1 = document.getElementById('chart-attrition').getContext('2d');
new Chart(ctx1, {
    type: 'bar',
    data: {
        labels: DATA.q1_turnover.labels,
        datasets: [{ label: 'Tỷ lệ nghỉ việc (%)', data: DATA.q1_turnover.data, backgroundColor: createGradient(ctx1, 'rgba(239, 68, 68, 0.85)', 'rgba(239, 68, 68, 0.2)'), borderColor: '#ef4444', borderWidth: 2, borderRadius: 6 }]
    },
    options: defaultOptions
});

// Chart 2: Average Salary Matrix
const ctx2 = document.getElementById('chart-salary').getContext('2d');
new Chart(ctx2, {
    type: 'bar',
    data: {
        labels: DATA.q2_salary.labels,
        datasets: [{ label: 'Lương trung bình ($/năm)', data: DATA.q2_salary.data, backgroundColor: createGradient(ctx2, 'rgba(2, 132, 199, 0.85)', 'rgba(2, 132, 199, 0.2)'), borderColor: '#0284c7', borderWidth: 2, borderRadius: 6 }]
    },
    options: defaultOptions
});

// Chart 3: Peak Performance Cycle
const ctx3 = document.getElementById('chart-peak-perf').getContext('2d');
new Chart(ctx3, {
    type: 'line',
    data: {
        labels: DATA.q3_peak.labels,
        datasets: [
            { label: 'Năm 2022', data: DATA.q3_peak.y2022, borderColor: '#6366f1', tension: 0.4, fill: false },
            { label: 'Năm 2024', data: DATA.q3_peak.y2024, borderColor: '#10b981', tension: 0.4, fill: false }
        ]
    },
    options: { ...defaultOptions, scales: { ...defaultOptions.scales, y: { min: 3.5, max: 3.8 } } }
});

// Chart 4: Elite Managers Performance
const ctx4 = document.getElementById('chart-top-managers').getContext('2d');
new Chart(ctx4, {
    type: 'bar',
    data: {
        labels: DATA.q4_managers.labels,
        datasets: [{ label: 'Điểm hiệu suất trung bình nhóm', data: DATA.q4_managers.data, backgroundColor: createGradient(ctx4, 'rgba(16, 185, 129, 0.85)', 'rgba(16, 185, 129, 0.2)'), borderColor: '#10b981', borderWidth: 2, borderRadius: 6 }]
    },
    options: { ...defaultOptions, indexAxis: 'y' }
});

// Chart 5: Training Baseline Effect
const ctx5 = document.getElementById('chart-training').getContext('2d');
new Chart(ctx5, {
    type: 'line',
    data: {
        labels: DATA.q5_training.labels,
        datasets: [
            { label: 'Nhóm Top 10 Quản lý', data: DATA.q5_training.topManagers, borderColor: '#0284c7', backgroundColor: 'rgba(2, 132, 199, 0.1)', fill: true, tension: 0.3 },
            { label: 'Nhóm Quản lý khác', data: DATA.q5_training.avgManagers, borderColor: '#f59e0b', backgroundColor: 'rgba(245, 158, 11, 0.1)', fill: true, tension: 0.3 }
        ]
    },
    options: defaultOptions
});

// Chart 6: Store Sales Revenue
const ctx6 = document.getElementById('chart-stores').getContext('2d');
new Chart(ctx6, {
    type: 'bar',
    data: {
        labels: DATA.q6_stores.top5Stores,
        datasets: [{ label: 'Doanh thu hàng tháng (Triệu USD)', data: DATA.q6_stores.top5Sales, backgroundColor: createGradient(ctx6, 'rgba(99, 102, 241, 0.85)', 'rgba(99, 102, 241, 0.2)'), borderColor: '#6366f1', borderWidth: 2, borderRadius: 6 }]
    },
    options: defaultOptions
});

// Chart 7: Department Satisfaction
const ctx7 = document.getElementById('chart-satisfaction').getContext('2d');
new Chart(ctx7, {
    type: 'bar',
    data: {
        labels: DATA.q7_satisfaction.labels,
        datasets: [{ label: 'Điểm hài lòng (Thang 10)', data: DATA.q7_satisfaction.data, backgroundColor: createGradient(ctx7, 'rgba(14, 165, 233, 0.85)', 'rgba(14, 165, 233, 0.2)'), borderColor: '#0ea5e9', borderWidth: 2, borderRadius: 6 }]
    },
    options: { ...defaultOptions, scales: { ...defaultOptions.scales, y: { min: 6.8, max: 7.5 } } }
});

// Chart 8: Role Productivity Bottleneck
const ctx8 = document.getElementById('chart-productivity').getContext('2d');
new Chart(ctx8, {
    type: 'bar',
    data: {
        labels: DATA.q8_productivity.labels,
        datasets: [{ label: 'Chỉ số Năng suất (Productivity Index)', data: DATA.q8_productivity.data, backgroundColor: createGradient(ctx8, 'rgba(245, 158, 11, 0.85)', 'rgba(245, 158, 11, 0.2)'), borderColor: '#f59e0b', borderWidth: 2, borderRadius: 6 }]
    },
    options: { ...defaultOptions, indexAxis: 'y' }
});

// Chart 10: Age vs Performance Correlation
const ctx10 = document.getElementById('chart-age').getContext('2d');
new Chart(ctx10, {
    type: 'bar',
    data: {
        labels: DATA.q10_age.labels,
        datasets: [{ label: 'Hiệu suất trung bình', data: DATA.q10_age.perf, backgroundColor: createGradient(ctx10, 'rgba(16, 185, 129, 0.85)', 'rgba(16, 185, 129, 0.2)'), borderColor: '#10b981', borderWidth: 2, borderRadius: 6 }]
    },
    options: { ...defaultOptions, scales: { ...defaultOptions.scales, y: { min: 3.5, max: 3.8 } } }
});

// Chart 11: AI Restructuring Doughnut Chart
const ctx11 = document.getElementById('chart-ai').getContext('2d');
new Chart(ctx11, {
    type: 'doughnut',
    data: {
        labels: DATA.q11_ai.labels,
        datasets: [{ data: DATA.q11_ai.headcount, backgroundColor: ['#ef4444', '#10b981', '#0284c7'], borderColor: '#ffffff', borderWidth: 3 }]
    },
    options: {
        responsive: true,
        maintainAspectRatio: false,
        plugins: { legend: { position: 'bottom', labels: { color: '#0f172a', font: { size: 13, weight: '700' } } } }
    }
});

// 6. GSAP ScrollTrigger Animations
gsap.registerPlugin(ScrollTrigger);

gsap.to('.slide-title', {
    scrollTrigger: { trigger: '.main-header', start: 'top 80%' },
    opacity: 1, duration: 1
});

gsap.utils.toArray('.glass-card').forEach((card) => {
    gsap.to(card, {
        scrollTrigger: { trigger: card, start: 'top 85%' },
        opacity: 1, y: 0, duration: 0.8, ease: 'power3.out'
    });
});
```

---

## SECTION V: QUALITY ASSURANCE & VERIFICATION CHECKLIST

Before final sign-off, verify that `index.html` satisfies every requirement:

1. [X] **File Structure:** Delivered as a single file `index.html` exceeding 850 lines of comprehensive documentation, code, and context.
2. [X] **Title & Identity:** Title reads **"Xóm Data Dashboard — Executive HR Performance Analytics"**.
3. [X] **Theme Fidelity:** Luminous light mode glassmorphism (`#f8fafc` base, `#0f172a` headers, frosted cards, light fluid Three.js shader).
4. [X] **Empirical Accuracy:** All 11 analytical questions contain exact quantitative findings matching `Employee Performance Analytics.ipynb` and `Bao_Cao_Tong_Hop_Hieu_Suat_Nhan_Su.md` (9 departments, exact percentages, 343 layoffs, $7.81M savings).
5. [X] **Zero Errors:** No missing HTML closing tags, broken JS module imports, or unhandled Chart.js canvas contexts.
