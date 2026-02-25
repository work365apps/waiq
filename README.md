# Work 365 AI Quotient (WAIQ)

WAIQ (Work 365 AI Quotient) is an open-source Power Platform solution designed to measure, track, and improve organizational AI maturity using a structured, weighted assessment model.

WAIQ helps teams move beyond ad-hoc AI experimentation by introducing:

- A standardized AI maturity framework  
- Recurring assessment cadence  
- Weighted scoring across maturity dimensions  
- Actionable initiatives tied to improvement cycles  
- Historical tracking of AI capability growth  

---

## 🚀 What Problem WAIQ Solves

Many organizations experiment with AI but struggle to:

- Measure maturity consistently
- Align departments around a common scale
- Translate assessment insights into structured action
- Track improvement over time

WAIQ provides a repeatable system that links **measurement → action → reassessment → improvement**.

---

## 🧠 Core Concepts

### 1️⃣ Assessment

An **Assessment** represents a defined evaluation period (e.g., monthly or quarterly).

Each assessment:
- Captures maturity ratings across defined dimensions
- Applies a weighted scoring model
- Produces an overall AI maturity score
- Includes initiatives to improve the next cycle’s results

Assessments create accountability and cadence.

---

### 2️⃣ Dimensions

Dimensions represent major AI maturity areas, such as:

- Strategy & Leadership
- Data Readiness
- Technology & Infrastructure
- Governance & Risk
- Skills & Culture
- Automation & Adoption

Each dimension contributes to the overall score based on its assigned weight.

---

### 3️⃣ Weighted Score Model

Overall maturity score is calculated using:


Σ (Dimension Rating × Dimension Weight)


This ensures strategic priorities influence the total maturity rating appropriately.

---

### 4️⃣ Initiatives (Actions)

Each assessment contains initiatives:

- Target specific maturity gaps
- Have defined owners
- Are time-bound
- Aim to improve the next assessment score

This converts measurement into operational improvement.

---

## 📦 Repository Structure


/solution → Unpacked Power Platform solution artifacts (source-controlled)
/build → Prebuilt solution .zip file for import
README.md → Documentation
LICENSE → License terms


- `/solution` contains the unpacked Dataverse solution files.
- `/build` contains the ready-to-import unmanaged solution `.zip`.

---

## 🛠 Installation Guide

### Prerequisites

- Microsoft Power Platform environment (Dataverse enabled)
- System Administrator or Environment Maker role
- Permissions to import solutions

---

### Option 1 — Import Prebuilt Solution (Recommended)

1. Go to https://make.powerapps.com
2. Select your target environment
3. Navigate to **Solutions**
4. Click **Import**
5. Upload the `.zip` file from:


/build/<WAIQ_Solution_Name>.zip


6. Follow the import wizard
7. Resolve connection references if prompted
8. Publish all customizations

The application will now be available in your environment.

---

### Option 2 — Build from Source (For Contributors)

If you are contributing or customizing:

#### 1. Clone the repository


git clone https://github.com/work365apps/waiq.git
cd waiq


#### 2. Install Power Platform CLI

https://learn.microsoft.com/power-platform/developer/cli/introduction

#### 3. Pack the solution


pac solution pack
--folder solution
--zipfile build/WAIQ.zip
--packagetype Unmanaged


#### 4. Import the generated zip into your environment

---

## 🔁 How to Use WAIQ

### Step 1 — Define Your Cadence

Choose a recurring schedule:

- Monthly
- Quarterly
- Bi-annual

Consistency is critical for maturity tracking.

---

### Step 2 — Create an Assessment

For each cycle:

1. Create a new Assessment record
2. Select the department or scope
3. Enter ratings for each maturity dimension
4. Review the calculated weighted score

---

### Step 3 — Review Results

Analyze:

- Strong dimensions
- Weak dimensions
- Score changes vs previous cycles
- Emerging trends

Focus on direction, not perfection.

---

### Step 4 — Define Initiatives

For each improvement area:

1. Create initiative records
2. Assign an owner
3. Define a timeframe
4. Link to the relevant dimension

Initiatives should be realistic, measurable, and actionable.

---

### Step 5 — Reassess

At the next cadence:

- Create a new assessment
- Compare scores
- Evaluate initiative impact
- Plan the next improvement cycle

AI maturity is iterative.

---

## 📊 Best Practices

- Keep your scoring model stable across cycles  
- Limit score changes to evidence-backed shifts  
- Tie initiatives to measurable business outcomes  
- Track trend lines over time  
- Ensure leadership visibility  

---

## 🔐 Governance & Security

- Use Dataverse security roles to control access
- Restrict editing of scores to authorized users
- Maintain historical assessments for auditability
- Avoid storing sensitive AI model data in maturity records

---

## 🏗 Extending WAIQ

You can extend WAIQ with:

- Custom maturity dimensions
- Different weighting strategies
- Power BI dashboards
- Automated reminders for assessment cadence
- Integration with project management tools
- Department-specific scoring overlays

---

## 🤝 Contributing

We welcome community contributions.

### Contribution Guidelines

1. Fork the repository
2. Create a feature branch
3. Make changes inside `/solution`
4. Test in a sandbox environment
5. Submit a pull request

Please ensure:

- No environment-specific values are committed
- No credentials are included
- Schema changes are documented
- Changes are backward-compatible where possible

---

## 📜 License

This project is licensed under the terms defined in the `LICENSE` file in this repository.

---

## 🎯 Vision

WAIQ exists to help organizations:

- Move from AI experimentation to operational maturity  
- Create transparency around AI capability  
- Drive structured improvement cycles  
- Align AI initiatives with measurable impact  

If you use WAIQ, star the repository and share improvements with the community.
