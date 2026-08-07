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

## Founding breakthrough: solving a long-standing data corruption issue

The idea of PaladinsCat sparked while investigating a server-sided skin ID integer overflow issue that had been known for more than three years but remained unaddressed within the community. The developers assigned skin IDs larger than 32,767 but have set the API response to take the value as Int16. As a result, any matches that includes the skin over the limit returns null data with the error message. Unfortunately, the company have dropped the support for the game and have dismissed the dev team - leaving no ways to fix this.
However, the AI assisted investigation traced to one undocumented API endpoint which enabled me to develop an alternative route to solve the issue. The traditional way was using the match detail endpoint which returns the skin IDs - subject to int overflow errors. The undocumented endpoint was the match player endpoint which only returns the player IDs within the match. I leveraged this to build a full stack service to serve the community with full match data. 

[**Read the investigation, published July 2026 →**](https://github.com/NabiCook/PaladinsCat/blob/main/docs/blog/skin-id-overflow.md)

---

# 📚 Background & Earlier Work

## 🎓 Computer Information Systems

A collection of coursework demonstrating experience with C#, ASP.NET, and database design.

[**Explore my CIS projects →**](https://github.com/NabiCook/CIS-School-Work)

## 🔒 Cybersecurity

Activities and assignments completed through the Google Cybersecurity Professional Certificate on Coursera.

[**Explore my cybersecurity work →**](https://github.com/NabiCook/coursera-works)
