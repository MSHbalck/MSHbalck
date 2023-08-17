- 👋 Hi, I’m @MSHbalck
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
MSHbalck/MSHbalck is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
python
python
import matplotlib.pyplot as plt
import numpy as np

#قم بتعيين قيم المعادلتين لخط القلب
x = np.linspace(-2, 2, 1000)
y1 = np.sqrt(1 - (abs(x) - 1) ** 2)
y2 = -3 * np.sqrt(1 - np.sqrt(abs(x) / 2))

# قم بتعيين قيم المعادلة لحرف "Z"
z_x = np.array([-1, 1])
z_y = np.array([2, -2])

# رسم قلب
plt.plot(x, y1, color='red', linewidth=2)
plt.plot(x, y2, color='red', linewidth=2)
plt.fill_between(x, y1, y2, color='red', alpha=0.3)

# رسم حرف "Z"
plt.plot(z_x, z_y, color='blue', linewidth=4)

# ضبط نطاق المحاور
plt.xlim(-2, 2)
plt.ylim(-3, 3)

# إعداد عنوان الرسمة
plt.title('حرف Z داخل قلب')

# عرض الرسمة
plt.show()




