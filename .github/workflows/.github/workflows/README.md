Daily PM/PO Lead Sweep (GitHub Actions)

    Runs every day at 8 AM CT (13:00 UTC).
    GH Actions -> OpenRouter (gpt-4o:online) -> 4 markdown tables -> Gmail SMTP.

    Required secrets

    • OPENROUTER_API_KEY
    • GMAIL_APP_PASSWORD

    Manual trigger

    GitHub -> Actions -> "Daily PM/PO Leads" -> Run workflow.

    Files

    • .github/workflows/daily-leads.yml (active)
    • .github/workflows/daily-leads-hermes.yml (disabled, Plan A for when Docker is healthy)
    • scripts/sweep.py
    • scripts/prompt.md
    • leads/ (archive)
