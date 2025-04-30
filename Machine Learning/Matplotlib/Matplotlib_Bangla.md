1. **লাইন গ্রাফ (Line Plot)**: 
   লাইন গ্রাফটি ডেটার মধ্যে সম্পর্ক দেখানোর জন্য ব্যবহার করা হয়, যেখানে X অক্ষের উপর মান এবং Y অক্ষের উপর অন্য মানের সম্পর্ক প্রদর্শিত হয়।
   
   ```python
   import matplotlib.pyplot as plt
   x = [1, 2, 3, 4, 5]
   y = [1, 4, 9, 16, 25]
   plt.plot(x, y)
   
   plt.show()
   ```

2. **স্ক্যাটার প্লট (Scatter Plot)**: 
   স্ক্যাটার প্লটটি প্রতিটি ডেটা পয়েন্টের জন্য X এবং Y এর মান ব্যবহার করে পয়েন্ট গুলি প্রদর্শন করে।
   
   ```python
   plt.scatter(x, y)
   plt.show()
   ```

3. **বার গ্রাফ (Bar Graph)**: 
   বার গ্রাফটি শ্রেণীভিত্তিক ডেটার তুলনা দেখানোর জন্য ব্যবহৃত হয়।
   
   ```python
   categories = ['A', 'B', 'C', 'D']
   values = [10, 20, 15, 25]
   plt.bar(categories, values)
   plt.show()
   ```

4. **হিস্টোগ্রাম (Histogram)**: 
   এটি সংখ্যার ডিস্ট্রিবিউশন দেখানোর জন্য ব্যবহার করা হয়।
   
   ```python
   data = [1, 2, 2, 3, 3, 3, 4, 4, 4, 4, 5, 5, 5, 5, 5]
   plt.hist(data, bins=5)
   plt.show()
   ```

5. **পাই চার্ট (Pie Chart)**: 
   পাই চার্টটি একাধিক অংশের আপেক্ষিক তুলনা দেখাতে ব্যবহার করা হয়।
   
   ```python
   sizes = [15, 30, 45, 10]
   labels = ['A', 'B', 'C', 'D']
   plt.pie(sizes, labels=labels, autopct='%1.1f%%')
   plt.show()
   ```

6. **বক্স প্লট (Box Plot)**: 
   বক্স প্লটটি ডেটার ভেরিয়েশন এবং আউটলায়ার দেখতে সাহায্য করে।
   
   ```python
   data = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
   plt.boxplot(data)
   plt.show()
   ```

7. **হিটম্যাপ (Heatmap)**: 
   হিটম্যাপটি ম্যাট্রিক্স ডেটা এবং এর মানের তুলনা প্রদর্শন করে।
   
   ```python
   import numpy as np
   data = np.random.rand(10,10)
   plt.imshow(data, cmap='hot', interpolation='nearest')
   plt.show()
   ```

8. **স্টেপ প্লট (Step Plot)**: 
   স্টেপ প্লটটি ডেটা পয়েন্টের মধ্যে পদক্ষেপ সঙ্কেত দেয়, সাধারণত ডিসক্রিট ডেটা দেখানোর জন্য ব্যবহৃত হয়।
   
   ```python
   plt.step(x, y)
   plt.show()
   ```

9. **ফিল্ড প্লট (Filled Plot)**: 
   এটি লাইন গ্রাফের নিচের অংশ ভরাট করে, যা অঞ্চলগুলি স্পষ্টভাবে দেখানোর জন্য ব্যবহৃত হয়।
   
   ```python
   plt.fill_between(x, y)
   plt.show()
   ```

10. **স্ট্যাকড বার গ্রাফ (Stacked Bar Graph)**: 
    এটি একাধিক শ্রেণীর জন্য বারগুলির স্ট্যাক প্রদর্শন করে।
    
    ```python
    A = [10, 20, 30, 40]
    B = [15, 25, 35, 45]
    plt.bar(categories, A, label="A")
    plt.bar(categories, B, bottom=A, label="B")
    plt.legend()
    plt.show()
    ```
