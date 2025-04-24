---
title: "Leonard M. I. Mensah - Cybersecurity Portfolio"
style: |
  body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    line-height: 1.6;
    background-color: #f4f4f4;
    color: #333;
    padding: 2rem;
  }
  h1, h2, h3 {
    color: #0a3d62;
  }
  .experience, .education, .certifications, .volunteer, .projects, .quiz {
    margin-bottom: 2rem;
    background: #fff;
    border-left: 6px solid #0a3d62;
    padding: 1rem;
    border-radius: 5px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
  }
  .section-title {
    display: flex;
    align-items: center;
    gap: 10px;
  }
  .section-title img {
    height: 32px;
  }
  .quiz-button {
    background-color: #0a3d62;
    color: white;
    border: none;
    padding: 0.5rem 1rem;
    margin: 0.3rem;
    cursor: pointer;
    border-radius: 5px;
    font-weight: bold;
  }
  .quiz-button:hover {
    background-color: #3c6382;
  }
script: |
  const quizQuestions = [
    {q: "Which port is used by HTTPS?", a: ["443", "80"], c: 0},
    {q: "What does SIEM stand for?", a: ["Security Info and Event Management", "Simple Internet Event Monitoring"], c: 0},
    {q: "Which OSI layer is IP in?", a: ["Network", "Data Link"], c: 0},
    {q: "Tool used for pen testing?", a: ["Metasploit", "Excel"], c: 0},
    {q: "What is 2FA?", a: ["Password + OTP", "Just password"], c: 0}
  ];
  let quizContainer = document.getElementById('quiz');
  quizQuestions.forEach((q, i) => {
    let qEl = document.createElement('div');
    qEl.innerHTML = `<p><strong>${i+1}. ${q.q}</strong></p>` + q.a.map((a, j) => `<button class='quiz-button' onclick='alert("${j === q.c ? 'Correct ✔' : 'Incorrect ✘'}")'>${a}</button>`).join('');
    quizContainer.appendChild(qEl);
  });
---

# ![Logo](https://img.icons8.com/ios-filled/50/000000/hacker.png) Leonard M. I. Mensah

**Cybersecurity Analyst | Systems Administrator | IT Strategist**
St. John's, NL, A1B 2J3 | +1 709 213-3807 | leomaximensah@gmail.com | [LinkedIn](https://linkedin.com/leonardmensah)

## 👨‍💻 Professional Summary
Versatile and detail-oriented cybersecurity professional with 10+ years of success in IT operations, security, training, and digital innovation. Demonstrated record in safeguarding systems, managing IT infrastructure, and training thousands in secure tech.

## 🧠 Skills & Technologies
- **Cybersecurity**: SIEM, IDS/IPS, Nmap, Nessus, Splunk, GDPR, ISO 27001, Vulnerability Management
- **Systems & Networks**: Active Directory, Windows Server, Linux (Ubuntu/CentOS), VMware, Azure
- **Languages**: Python, PowerShell, Bash, JavaScript, SQL
- **Soft Skills**: Critical Thinking, Problem-Solving, Communication, Leadership

## 🎓 Education & Certifications
- Cyber Security Analyst Diploma – Willis College (2025)
- Adv. Diploma in Software Engineering – APTECH (2012)
- Certifications: CompTIA Security Analytics, Security+, A+, Google Cybersecurity, PMP

## 💼 Professional Experience
### 🔹 AVASO Technology Solutions (2024 - Present)
- Provided onsite Level 1/2 support, imaging, patching, staging, and field tech support.
- Diagnosed/resolved software issues, created custom documentation.
- Supported enterprise rollouts, office relocations, remote hands-on troubleshooting.

### 🔹 Atunwa Digital (2023 - 2024)
- Led penetration testing, SIEM alerting, and user training programs.
- Reduced security incidents by 30% via access control and MFA policies.

### 🔹 Pellucid Technology (2014 - 2023)
- Delivered 42+ custom apps, secured IT systems for 30+ clients.
- Oversaw network security tools like Lansweeper, SolarWinds, Zendesk.

### 🔹 Open Learning Exchange (2017 – 2021)
- Built Android-based LMS for 60K+ students.
- Supervised 15+ global interns, automated security audits and Raspberry Pi deployments.

### 🔹 Jhpiego (2015 – 2017)
- Trained 2,000+ tutors on eLearning tools.
- Set up health data systems and automated SMS for 5+ projects.

## 🏆 Projects & Labs
- Pen Testing (Kali/Metasploitable), AWS S3 + CloudFront, SQL DB Security
- Network Topology Design, GPO Setup, Linux Scripting, Windows Server Deployment

## 🙌 Volunteer
**Tech Lead**, Church of Pentecost (2023 – Present) | **Tech Support**, Golden Chapter Foundation (2021 – 2023)

## 🎮 Interactive Cyber Quiz
<div id="quiz"></div>
