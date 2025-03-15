## 💻 Web Developer | Python Specialist👋

# 💻 برنامه‌نویس وب | متخصص پایتون

🌐 **طراحی و توسعه وب‌های پویا**  
📚 **همیشه در حال یادگیری!**  
**"کد، زبان من است!"** 🧑‍💻  

---

## 🚀 پروژه‌های من

### برنامه‌های ما در مایکت:

۱. **مترجم فارسی**:  
   [دانلود از مایکت](https://myket.ir/app/com.w_18248975)  

۲. **تبدیل متن به خطوط باستانی**:  
   [دانلود از مایکت](https://myket.ir/app/com.w_18170834)  

۳. **چت با هوش مصنوعی بارد**:  
   [دانلود از مایکت](https://myket.ir/app/com.w_18254252)  

---

### سایت‌های آنلاین ما:

- **راه هدایت**:  
  [بازدید از سایت](https://flask-u0m653.chbk.app)  

- **ناشناس اختصاصی خودمان**:  
  [بازدید از سایت](https://flask-sh0hv8.chbk.app)  

- **چت با هوش مصنوعی همه‌کاره (با Streamlit)**:  
  [بازدید از سایت](https://huggingface.co/spaces/chatbotamirhossin/chatbot)  

---
سایت روزمه ما :
https://static-1nljmg.chbk.app/
---

## 🐍 کد نمونه با Flask

در اینجا یک نمونه کد ساده با استفاده از فریمورک **Flask** آورده شده است که نشان می‌دهد چگونه می‌توان یک وب‌اپ ساده ایجاد کرد:

```python
from flask import Flask, render_template, request

app = Flask(__name__)

@app.route('/')
def home():
    """
    صفحه اصلی وب‌اپلیکیشن.
    """
    return render_template('index.html', title="خانه")

@app.route('/greet', methods=['POST'])
def greet():
    """
    صفحه خوش‌آمدگویی به کاربر.
    """
    name = request.form.get('name')
    return f"سلام {name}! به وب‌سایت ما خوش آمدید! 🎉"

if __name__ == '__main__':
    app.run(debug=True)



