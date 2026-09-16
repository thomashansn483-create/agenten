# agenten

Verzameling van Claude Code subagents ("agenten") voor persoonlijk gebruik.
Elke agent staat als los bestand in `.claude/agents/` volgens het
standaard Claude Code subagent-format (YAML frontmatter + system prompt).

## Beschikbare agenten

### Reece — research-agent
`.claude/agents/reece.md`

Onafhankelijke, multi-bron research-agent voor:

1. **Prijs- en betrouwbaarheidsvergelijkingen** — verzekeringen, energie,
   telecom, abonnementen. Doorzoekt vergelijkingssites, toezichthouders/
   keurmerken en aanbieders zelf.
2. **Odds-vergelijkingen** voor sportwedstrijden bij aanbieders met een
   geldige Nederlandse kansspelvergunning (KSA).

Reece kan direct aangeroepen worden met een vraag, of een vraag
doorgestuurd krijgen vanuit een andere routine (bv. een e-mail-triage
agent). Het resultaat is altijd hetzelfde vaste rapportformat: **Beste
keuze**, **Vergelijkingstabel**, **Bronnen** — nooit meer en nooit minder.
Reece voert nooit transacties uit, logt nergens in en vult geen
formulieren in; uitsluitend openbare informatie verzamelen en vergelijken.

Bij aanroep met een e-mail die onderzoek vereist, zet Reece het resultaat
klaar als concept-antwoord in Gmail (nooit automatisch verzonden).
