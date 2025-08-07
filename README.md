# 🤝 Social Network Recommendation System (Pure Python)

## 📌 Overview
This project implements a simple **"People You May Know"** or **"Pages You Might Like"** feature using **pure Python** — without using any external machine learning libraries. The logic is based on analyzing friends, mutual connections, or common interests to recommend other users or pages.

## 💡 Core Features
- Recommend people you may know based on:
  - Mutual friends
  - Friends-of-friends logic
- Recommend pages you might like based on:
  - Common likes
  - User interaction similarity

## 🛠️ Technologies Used
- Pure Python
- No external libraries (except for `json` or `csv` if data is loaded)
- Simple data structures (lists, sets, dictionaries)

## 📂 Project Structure
```
├── data/
│   └── social_network.json        # Sample user data with friends & likes
├── people_you_may_know.py         # Recommendation logic for users
├── pages_you_might_like.py        # Recommendation logic for pages
├── utils.py                       # Utility functions (e.g., mutual friends)
├── main.py                        # Entry point to run recommendation system
├── README.md                      # Project documentation
```

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/social-recommendation-python.git
   cd social-recommendation-python
   ```

2. Run the program:
   ```bash
   python main.py
   ```

3. Output:
   - Suggested users/pages will be printed based on sample input

## 📘 Sample Input (JSON)
```json
{
  "users": [
    {"id": 1, "name": "Alice", "friends": [2, 3], "likes": ["PageA", "PageB"]},
    {"id": 2, "name": "Bob", "friends": [1, 3], "likes": ["PageB", "PageC"]},
    {"id": 3, "name": "Charlie", "friends": [1], "likes": ["PageA", "PageD"]}
  ]
}
```

## 🧠 Logic Behind Recommendations
- **People You May Know**:
  - Suggest users with the highest number of mutual friends not already connected.
- **Pages You Might Like**:
  - Suggest pages liked by friends but not yet liked by the user.

## 📌 Future Enhancements
- Add a simple GUI or web interface (e.g., Tkinter, Flask)
- Add data persistence (saving recommendations)
- Visualize friend graphs

## 🙋‍♂️ Author
- Name: **Abdur Rafay**
- GitHub: [a6dur](https://github.com/your-a6dur)
