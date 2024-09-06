### **Project Name**
**"British Airways Customer Review Analysis"**

---

### **Overview**
This project involves analyzing customer reviews of British Airways to gain insights into customer sentiments and uncover key themes and topics. By leveraging Natural Language Processing (NLP) techniques, we aimed to identify the underlying sentiments and frequently discussed topics in these reviews to better understand customer experiences.

---

### **Objective**
- Perform sentiment analysis on British Airways customer reviews.
- Uncover key topics discussed by customers using topic modeling.
- Visualize customer sentiment distribution and frequent words/themes in the reviews.

---

### **Challenges**
- Scraping and handling unstructured review data from a web source.
- Dealing with noise in the text data, such as unwanted characters and stopwords.
- Ensuring that topic models provide meaningful insights into customer feedback.

---

### **Solution**
To address these challenges, we implemented the following steps:

---

### **Steps Taken**

1. **Web Scraping**  
   - Scraped customer reviews using **BeautifulSoup** and **Requests** from the British Airways review page.
   - Collected review data and stored it in a DataFrame using **Pandas**.

2. **Data Cleaning**  
   - Removed irrelevant columns and cleaned the text data by:
     - Removing unwanted characters (e.g., punctuation).
     - Converting all words to lowercase for consistency.
     - Removing stopwords using **spaCy** to further clean the text.

3. **Sentiment Analysis**  
   - Conducted sentiment analysis using **TextBlob** to classify reviews as positive, negative, or neutral.
   - Visualized the sentiment distribution with bar plots using **Matplotlib** and **Seaborn**.

4. **Topic Modeling**  
   - Utilized **CountVectorizer** to tokenize reviews and create a document-term matrix.
   - Applied **Latent Dirichlet Allocation (LDA)** for topic modeling to identify major topics discussed by customers.
   - Visualized the topics to gain insights into recurring themes in customer feedback.

5. **Word Cloud**  
   - Created a **WordCloud** to visualize the most frequently used words in the reviews.

---

### **Technologies and Tools Used**
- **Python**: Programming language for the project.
- **BeautifulSoup & Requests**: For web scraping.
- **Pandas**: For data manipulation and cleaning.
- **spaCy**: For advanced text preprocessing.
- **TextBlob**: For sentiment analysis.
- **CountVectorizer & LDA**: For topic modeling.
- **Matplotlib & Seaborn**: For data visualization.
- **WordCloud**: For visualizing the most frequent words.

---

### **Results and Insights**

#### **Sentiment Analysis:**

![Sentiment Distribution](British-Airways-Customer-Review-Analysis/sentiment%20analysis.png)

- **Negative Reviews**: 500 reviews.
- **Positive Reviews**: Over 1,000 reviews.
- **Neutral Reviews**: Over 400 reviews.

The analysis shows that British Airways has received a significantly higher number of positive reviews compared to negative and neutral ones. Neutral reviews reflect an experience that met expectations but wasn’t exceptional.

#### **Topic Modeling:**

![Topic Modeling](British-Airways-Customer-Review-Analysis/topic%20modelling.png)

We identified five key topics discussed by customers:

1. **Luggage Handling**  
   - Words like “baggage,” “luggage,” “suitcase,” and “ticket” suggest feedback related to handling luggage, including lost or delayed baggage.

2. **Flight Experience**  
   - Featuring words like “good,” “flight,” “crew,” “food,” and “seat,” this topic covers customer experiences regarding crew service, seat comfort, and food quality.

3. **Booking & Onboard Service**  
   - Includes words like “seat,” “service,” “airline,” and “crew,” representing feedback on the booking process and onboard service.

4. **Business Class Service**  
   - Words such as “class,” “business,” “service,” and “food” highlight the experiences of passengers in business class.

5. **Flight Scheduling & Delays**  
   - Words like “flight,” “hour,” “service,” and “delay” address issues related to flight schedules, delays, and check-in processes.

#### **Word Cloud Visualization:**

![Word Cloud](British-Airways-Customer-Review-Analysis/word%20clouds.png)

- The word cloud highlights frequent words such as "British," "Airways," "flight," "London," and "Heathrow," indicating that these terms are central themes in customer feedback.
  
---

### **General Insights**
1. **Positive Sentiment Dominates**  
   - The majority of reviews are positive, indicating a generally satisfactory customer experience with British Airways.

2. **Key Topics Identified**  
   - Luggage handling, flight experience, booking/onboard service, business class service, and flight scheduling/delays were key areas discussed by customers.

3. **Frequent Terms in Feedback**  
   - The word cloud emphasized terms like "British Airways," "flight," and "Heathrow," suggesting these were central to customer experiences.

---

### **Conclusion**
The analysis reveals that British Airways generally receives positive feedback from its customers. However, issues with luggage handling and flight scheduling are critical areas for improvement. By addressing these, British Airways can enhance customer satisfaction and maintain its positive reputation.
