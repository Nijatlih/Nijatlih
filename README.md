## Nijat

Full-stack AI engineer in Bremen. My work is taking an AI product the whole
way — from a model call to something running behind a health check in
production — usually alone.

Right now that product is **Soundra**: AI music generation with a
copyright-provenance layer, so a generated track carries a verifiable,
offline-checkable proof of origin. That provenance part is the piece I find
genuinely unsolved elsewhere.

**How the code actually looks.** soundra's CI gate runs 1,639 backend, 146
frontend-unit and 484 end-to-end tests before anything merges. The deploy job
is designed to migrate the database before serving traffic and roll itself
back on a failed health check — implemented and CI-tested, not yet run
against a live host. Not a demo repo — the plumbing you build once you mean
to operate the thing.

Backend is home ground — FastAPI + async SQLAlchemy on the Python side,
Spring Boot 3.5 / Java 21 on the JVM side, both with real migrations (Alembic,
Flyway) contract-tested against a live database rather than mocks. The MLOps
capstone that closed my training runs on MLflow + Prefect + Evidently +
Prometheus/Grafana, Docker-Compose'd, CI on Ruff + pytest.

**Path.** Java/Spring foundation via bootcamp and self-built projects
(2022–2023) → Data Science, then ML Engineering / MLOps training at neue fische
(2026) → building AI products since.

**A note on this profile.** Most of my 2026 code lives in private repositories
while the products are pre-launch — over 1,100 of ~1,270 commits this year are
private. The pinned repos are the parts I can show openly; happy to walk
through the rest in a conversation.

📍 Bremen, Germany · English & Deutsch · 📧 108176479+Nijatlih@users.noreply.github.com

---

## Auf Deutsch

Full-Stack-AI-Engineer aus Bremen. Meine Arbeit: ein KI-Produkt den ganzen
Weg bringen — vom Modell-Call bis zu etwas, das hinter einem Health-Check in
Produktion läuft, meist allein.

Aktuell heißt dieses Produkt **Soundra** — KI-Musikgenerierung mit einer
Copyright-Provenienz-Schicht: Ein generierter Track trägt einen überprüfbaren,
offline verifizierbaren Herkunftsnachweis. Genau dieser Teil ist anderswo
bisher ungelöst.

**Wie der Code wirklich aussieht.** soundras CI-Gate lässt vor jedem Merge
1.639 Backend-, 146 Frontend-Unit- und 484 End-to-End-Tests laufen. Der
Deploy-Job ist so gebaut, dass er die Datenbank migriert, bevor Traffic
angenommen wird, und bei fehlgeschlagenem Health-Check automatisch
zurückrollt — implementiert und CI-getestet, aber noch nicht gegen einen
echten Host gelaufen.

Zu Hause vor allem im Backend — FastAPI + async SQLAlchemy auf der Python-,
Spring Boot 3.5 / Java 21 auf der JVM-Seite, beide mit echten Migrationen
(Alembic, Flyway), contract-getestet gegen eine laufende Datenbank statt gegen
Mocks. Das abschließende MLOps-Capstone läuft auf MLflow + Prefect + Evidently
+ Prometheus/Grafana, per Docker-Compose, CI mit Ruff + pytest.

**Weg.** Java/Spring-Grundlage über Bootcamp und eigene Projekte (2022–2023)
→ Data Science, dann ML Engineering / MLOps bei neue fische (2026) → seitdem
Bau eigener KI-Produkte.

**Hinweis zu diesem Profil.** Der Großteil meines 2026er-Codes liegt in
privaten Repositories, solange die Produkte vor dem Launch stehen. Die
angepinnten Repos sind der Teil, den ich offen zeigen kann — den Rest gern im
Gespräch.

📍 Bremen · 📧 108176479+Nijatlih@users.noreply.github.com
