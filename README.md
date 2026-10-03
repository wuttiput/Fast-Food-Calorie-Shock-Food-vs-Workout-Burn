# Fast-Food-Calorie-Shock-Food-vs-Workout-Burn
โครงงานวิเคราะห์ระหว่างสารอาหารฟาสฟู๊ดกับการออกกำลังกายเผาผลาญด้วยเทคนิค Machine Learning สำหรับวิชา 1145 201 Mathematics for Data Science

📊 สรุปภาพรวมโครงงาน (Project Summary)

CLO1 (Linear Algebra Analysis - PCA): จากการใช้วิธีพีชคณิตเชิงเส้นแบบคำนวณมือโดยตรง (Eigen-decomposition) พบว่ามิติข้อมูลขนาด 15 มิติ สามารถลดรูปมาเหลือเพียง 2 แกนหลัก (PC1 และ PC2) ซึ่งอธิบายรูปแบบความแปรปรวนสะสมของข้อมูล (Cumulative Variance) ได้สูงถึง 77.15% ทำให้เข้าใจความสัมพันธ์ของข้อมูลทางสรีระและสารอาหารได้ง่ายขึ้นโดยไม่สูญเสียลักษณะเฉพาะ
CLO2 (Statistical Learning & Bias-Variance): จากการวิเคราะห์ค่าความสัมพันธ์พบว่า total_calories มีสหสัมพันธ์เชิงบวกกับปริมาณแคลอรีส่วนเกินสูงสุด (r = 0.999) และเมื่อทดสอบโมเดลด้วย Polynomial Degree ต่างๆ พบว่าระดับพหุนามดีกรี 1 (Linear Relation) มีประสิทธิภาพที่ยอดเยี่ยมที่สุด โดยไม่มีพฤติกรรม Overfitting ซึ่งสอดคล้องกับหลักการจัดสรรความซับซ้อนของโมเดลที่สมดุลพอดี (Optimal Bias-Variance Trade-off)
CLO3 (Model Building): ในส่วนของโครงสร้างการทำนายด้วยวิธีแบบ Regression พบว่า Model 2 (Multiple Linear Regression) ให้ผลลัพธ์แม่นยำสูงสุดอย่างเด่นชัด โดยมีค่า  R2=1.0000  และค่า MSE เข้าใกล้ 0.0000 ทั้งบนชุดข้อมูล Train และ Test
CLO4 (Model Selection): ผลลัพธ์จากการทำ 5-Fold Cross-Validation ตอกย้ำว่า Multiple Linear Regression เป็นระบบการทำนายที่ดีที่สุด โดยมีค่าเฉลี่ยความคลาดเคลื่อนสะสม (Mean CV MSE) ต่ำสุดที่เข้าใกล้  0  อย่างมีนัยสำคัญ บ่งชี้ว่าโมเดลมีการเรียนรู้ที่เสถียรและพร้อมใช้งานกับข้อมูลชุดใหม่โดยไร้ปัญหาความแปรปรวนสูง (No High Variance)

📂 สมาชิกกลุ่ม (Group Members)
นายวุฒิภัทร วิริยเสนกุล รหัสนักศึกษา 68114540605

Acknowledgements: แหล่งข้อมูลสาธารณะจาก Kaggle Dataset และระบบประมวลผล Google Colab
