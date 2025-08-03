<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8" />
  <title>تسجيل حضور الطلاب - مدرسة حفص بن راشد</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      direction: rtl;
      background-color: #f9f9f9;
      padding: 30px;
      text-align: center;
    }
    input, button {
      padding: 10px;
      font-size: 18px;
      margin: 10px;
    }
    ul {
      list-style: none;
      padding: 0;
      max-width: 400px;
      margin: 20px auto 0;
      text-align: right;
    }
    li {
      background-color: #d0f0fd;
      margin: 5px 0;
      padding: 10px;
      border-radius: 5px;
    }
  </style>
</head>
<body>
  <h1>تسجيل حضور الطلاب</h1>
  <form id="attendanceForm">
    <input type="text" id="studentName" placeholder="اكتب اسم الطالب" required />
    <button type="submit">تسجيل</button>
  </form>

  <ul id="attendanceList"></ul>

  <script>
    const form = document.getElementById('attendanceForm');
    const list = document.getElementById('attendanceList');

    form.addEventListener('submit', e => {
      e.preventDefault();
      const name = document.getElementById('studentName').value.trim();
      if (name) {
        const li = document.createElement('li');
        const now = new Date();
        const time = now.toLocaleTimeString('ar-EG', { hour: '2-digit', minute: '2-digit' });
        li.textContent = `${name} - حاضر ✅ (${time})`;
        list.appendChild(li);
        form.reset();
      }
    });
  </script>
</body>
</html>
