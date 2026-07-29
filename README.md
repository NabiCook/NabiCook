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

The idea of PaladinsCat sparked while investigating a server-sided skin ID integer overflow issue that had been known for more than three years but remained unaddressed within the community. The developers assigned skin IDs larger than 32,767 but have set the API response to take the value as Int16. As a result, any matches that includes the skin over the limit returns null data with the error message. Unfortunately, the company have dropped the support for the game and have dismissed the dev team - leaving no ways to fix this.
However, the AI assisted investigation traced to one undocumented API endpoint which enabled me to develop an alternative route to solve the issue. The traditional way was using the match detail endpoint which returns the skin IDs - subject to int overflow errors. The undocumented endpoint was match player endpoint which only returns the player IDs within the match. I leveraged this to lookup the player history for each 10 individual players within the match, then used the match history of each player to reconstruct a full match detail payload. 

This finding became PaladinsCat's technical breakthrough and the starting point for the platform itself. No other platforms have addressed this problem, returns an incomplete match result with missing players or shows an error message saying that the match does not exist. The service quickly became the mainstream within the gaming community which the players use it on a daily basis to check their stats and match results. 
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
