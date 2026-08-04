# Portfolio Case Studies & Voice Card

## Voice Card
> **Direct, warm, plain, no buzzwords.**

---

## Before / After Comparison
* **Generic AI Line (Before):** 
  > *"Leveraged cutting-edge machine learning methodologies and dynamic search ranking algorithms to optimize data pipelines, driving high-impact analytical results through synergistic feature engineering."*
* **My Edited Version (After):** 
  > *"I built an automated search-ranking pipeline using Python and Pandas that processes query-document pairs, verifies data integrity, and passes CI/CD checks without throwing pipeline errors."*

---

## Case Study: ML Search Ranking Lab & Automated CI/CD Pipeline

### 1. The Problem
When setting up a machine learning workflow for search ranking, code execution often breaks silently due to missing raw datasets, unmonitored data leaks, or failing GitHub Actions runners. Standard templates are either too theoretical or fail to connect raw CSV inputs to a verifiable, repeatable pipeline process.

### 2. What I Did (And What I Decided)
* **Structured the data ingestion:** Integrated `content_refresh_anonymized.csv` directly into the repository structure so the pipeline has a reliable local source of truth.
* **Enforced strict validation:** Configured data verification checks to spot anomalies and handle missing files cleanly with explicit exit codes (`sys.exit(1)`).
* **Automated continuous integration:** Set up GitHub Actions workflow files (`smoke-test.yml`) to run automatic checks on every push, ensuring data leak prevention and script success before merging.

### 3. What Came of It
* A fully functioning, green-status CI/CD pipeline hosted on GitHub that successfully runs script checks, tests data paths, and validates preprocessing steps automatically without manual intervention.

---

## Bio and Contact / CTA

### Bio
Hi, I'm Aditya Upadhyay, a B.Tech student and machine learning engineering intern building practical, reliable data pipelines and intelligent systems. I focus on clean code, automated testing, and solving real-world engineering problems without the jargon.

### Get in Touch
* **GitHub:** [upadhyayaditya7](https://github.com/upadhyayaditya7)
* **Call to Action:** Looking to collaborate on machine learning projects or discuss tech engineering? Check out my repositories or reach out directly!
