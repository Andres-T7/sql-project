# Digital Book Market Analysis — SQL + Python

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=for-the-badge&logo=sqlalchemy&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

## Description
Exploratory data analysis on a competitor's database in the digital book application market, covering over 1,000 titles, 179 publishers, and thousands of user ratings. The project is rooted in the post-pandemic context, where digital book consumption grew significantly, creating a market opportunity for the launch of a new product in this space.

## Objective
Extract key insights from the catalog and user behavior to support strategic decision-making in the design of a new book app, identifying relevant publishers, top-rated authors, and user engagement patterns.

## Project Files
- `Proyecto_Ebooks_SQL.ipynb` — Main notebook with the full analysis
- `images/` — Data structure diagram
- `.env.example` — Environment variables template

## Key Findings
1. **80% of the catalog (819 out of 1,000 books)** were published after the year 2000, reflecting an offering aligned with current reader interests.
2. **Penguin Books** has the largest presence in the catalog with **42 books** exceeding 50 pages, positioning it as a potential strategic partner.
3. **J.K. Rowling/Mary GrandPré** achieved the highest average rating (**4.28/5.0**) among authors with at least 50 ratings, indicating strong user engagement on titles with a significant review volume.
4. The most active users rate a large number of books but generate few text reviews, representing an opportunity to incentivize more qualitative participation.

## Business Conclusions & Recommendations
- Prioritize authors and books with high ratings and significant review volume in the app's recommendation system.
- Establish strategic partnerships with Penguin Books given its catalog weight and strong user perception.
- Implement incentive mechanisms to encourage text reviews among the most active users, improving the quality of information available to other readers.

## Data Description
The client provided a database containing information from a market competitor. The dataset integrates books, publishers, and authors data, along with user ratings and reviews, structured across the following tables:

| Table        | Description                                              |
| ------------ | -------------------------------------------------------- |
| `books`      | Book details: title, page count, publication date        |
| `authors`    | Author ID and name                                       |
| `publishers` | Publisher ID and name                                    |
| `ratings`    | Numerical ratings per book and user                      |
| `reviews`    | Text reviews per book and user                           |

## Requirements
`pandas` · `sqlalchemy` · `psycopg2-binary` · `python-dotenv`
```bash
pip install -r requirements.txt
```
