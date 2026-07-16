# 🐈 PaladinsCat

<p align="center">
  <a href="https://paladinscat.com/">
    <img src="assets/paladinscat.png" alt="PaladinsCat logo" width="120">
  </a>
</p>

**Paladins: Comp Analytics Tool** — advanced statistics, or just meow.

- [**Visit PaladinsCat →**](https://paladinscat.com/)
- [**View releases and technical write-ups →**](https://github.com/NabiCook/PaladinsCat)
- [**Explore the localization repository →**](https://github.com/NabiCook/PaladinsCat-locales)

## What it does

PaladinsCat turns raw Paladins match data into evidence players can inspect. Its core purpose is to track accounts associated with suspected cheating or repeated harmful behavior, preserve relevant activity even when profiles are private, and reveal patterns that may be damaging the competitive community.

The platform brings match histories, player profiles, champion statistics, and account signals together so players can make informed decisions based on documented activity—not hearsay. It provides evidence for community awareness while leaving room for careful human judgment.

## Founding breakthrough: solving a long-standing data corruption issue

PaladinsCat began development in **May 2026** while investigating a skin ID corruption issue that had been known for more than five years but remained unaddressed. The investigation traced missing and incorrect skin information to a silent signed 16-bit integer overflow and identified **31 affected skins across 20 champions** whose IDs had crossed the `32,767` limit.

That finding became PaladinsCat's first major technical breakthrough and the starting point for the platform itself. PaladinsCat now detects affected matches and uses a multi-stage recovery pipeline to reconstruct player details, fill gaps, and label each record by its source and quality. Instead of silently accepting incomplete data—or discarding the match—the platform preserves what is valid and clearly identifies what was recovered.

[**Read the investigation, published July 2026 →**](https://github.com/NabiCook/PaladinsCat/blob/main/docs/blog/skin-id-overflow.md)

## Why it stands out

- **Evidence over accusation:** account concerns are supported by inspectable match and activity data rather than rumors alone.
- **Community accountability:** the platform is built to identify patterns associated with suspected cheating and behavior that harms the competitive environment.
- **Visibility into private profiles:** relevant match activity can remain useful for analysis even when an account's profile is private.
- **Data integrity first:** it investigates hidden problems in upstream game data instead of treating every API response as correct.
- **Resilient analytics:** broken matches can be detected and reconstructed through supplementary lookups.
- **Transparent results:** direct, recovered, and minimal records are labeled so their origin and quality remain visible.
- **Open technical findings:** investigations and production lessons are published as detailed technical write-ups.

---

# 📚 Background & Earlier Work

## 🎓 Computer Information Systems

A collection of coursework demonstrating experience with C#, ASP.NET, and database design.

[**Explore my CIS projects →**](https://github.com/NabiCook/CIS-School-Work)

## 🔒 Cybersecurity

Activities and assignments completed through the Google Cybersecurity Professional Certificate on Coursera.

[**Explore my cybersecurity work →**](https://github.com/NabiCook/coursera-works)
