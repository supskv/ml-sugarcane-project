# ml-sugarcane-project


วิธีใช้

จาก Ex1 จะมีฟังชั่นไว้ คัดแยก X, y ทั้ง Level1 และ Level 2 สำเร็จรูปวิธใช้แสนจะง่าย

1. สำหรับ Level 1 ให้ import lib+functions แล้ว ทำ step 1 และ 2.1 จากนั้น ใช้ X, y ได้เลย
2. สำหรับ Level 2 ให้ import lib+functions แล้ว ทำ step 1 และ 2.2 จากนั้น เราจะได้ X,y ของ plant และ X,y ของ Ratoon ใช้ได้เลย

สำหรับการนำไปใช้ในโมเดล shape ของ X มันจะเป็น (batch, seq_len, embedsize) ถ้าเป็น RNN ก็ใช้ได้เลย แต่ถ้าเป็น CNN อาจต้อง เพิ่ม input channel เป็น axis ใหม่แล้ว reshape (ใช้ np.permute ก็ได้) เป็น (batch, 1, height(embedsize), width (seq_len)) แทน

ปล. X,y ที่ได้มา ทำตามขั้นตอนแล้วใช้ได้เลยนะ
